# <span class="jumptarget"> Orders Reference</span>

Orders APIs integrate with point-of-sale, shipping, distribution, and inventory-management systems. They include Orders, Order Coupons, Order Messages, Order Products, Order Shipping Addresses, Order Statuses, Order Taxes, and Shipments.

## <span class="jumptarget"> Orders </span>

The Order object contains a record of the purchase agreement between a shopper and a merchant.

### <span class="jumptarget"> Order Object – Properties </span>

| Name | Type | Description |
| --- | --- | --- |
| id | int | The ID of the order, a read-only value. Do not pass in PUT or POST. |
| customer_id | int | The ID of the customer placing the order; or `0` if it was a guest order. |
| date_created | date | The date this order was created. If not specified, will default to the current time. The date should be in RFC format, e.g.: `Tue, 20 Nov 2012 00:00:00 +0000` |
| date_modified | date | A read-only value representing the last modification of the order. Do not attempt to modify or set this value in a POST or PUT operation. |
| date_shipped | date | A read-only value representing the date of shipment. Do not attempt to modify or set this value in a POST or PUT operation. |
| status_id | int | The status ID. See examples under [Order Statuses](/api/v2/#order-statuses). |
| status | string | The status will include one of the string values defined under [Order Statuses](/api/v2/#order-statuses). This value is read-only. Do not attempt to modify or set this value in a POST or PUT operation. |
| subtotal_ex_tax | decimal | Override value for subtotal excluding tax. If specified, the field `subtotal_inc_tax` is also required. |
| subtotal_inc_tax | decimal | Override value for subtotal including tax. If specified, the field `subtotal_ex_tax` is also required. |
| subtotal_tax | decimal | A read-only value. Do not attempt to set or modify this value in a POST or PUT operation. |
| base_shipping_cost | decimal | The value of the base shipping cost. |
| shipping_cost_ex_tax | decimal | The value of shipping cost, excluding tax. |
| shipping_cost_inc_tax | decimal | The value of shipping cost, including tax. |
| shipping_cost_tax | decimal | A read-only value. Do not attempt to modify or set this value in a POST or PUT operation. |
| shipping_cost_tax_class_id | int | Shipping-cost tax class. A read-only value. Do not attempt to modify or set this value in a POST or PUT operation. (NOTE: Value ignored if automatic tax is enabled on the store.) |
| base_handling_cost | decimal | The value of the base handling cost. |
| handling_cost_ex_tax | decimal | The value of the handling cost, excluding tax. |
| handling_cost_inc_tax | decimal | The value of the handling cost, including tax. |
| handling_cost_tax | decimal | A read-only value. Do not attempt to modify or set this value in a POST or PUT operation. |
| handling_cost_tax_class_id | int | A read-only value. Do not attempt to set or modify this value in a POST or PUT operation. (NOTE: Value ignored if automatic tax is enabled on the store.) |
| base_wrapping_cost | decimal | The value of the base wrapping cost. |
| wrapping_cost_ex_tax | decimal | The value of the wrapping cost, excluding tax. |
| wrapping_cost_inc_tax | decimal | The value of the wrapping cost, including tax. |
| wrapping_cost_tax | decimal | A read-only value. Do not attempt to modify or set this value in a POST or PUT operation. |
| wrapping_cost_tax_class_id | int | A read-only value. Do not attempt to set or modify this value in a POST or PUT operation. (NOTE: Value ignored if automatic tax is enabled on the store.) |
| total_ex_tax | decimal | Override value for the total, excluding tax. If specified, the field `total_inc_tax` is also required. |
| total_inc_tax | decimal | Override value for the total, including tax. If specified, the field `total_ex_tax` is also required. |
| total_tax | decimal | A read-only value. Do not attempt to set or modify this value in a POST or PUT operation. |
| items_total | int | The total number of items in the order. |
| items_shipped | int | The number of items that have been shipped. |
| payment_method | string | The payment method for this order. Can be one of the following: `Manual`, `Credit Card`, `cash`, `Test Payment Gateway`, etc. |
| payment_provider_id | string | The external Transaction ID/Payment ID within this order's payment provider (if a payment provider was used). |
| payment_status | enum | A read-only value. Do not attempt to set or modify this value in a POST or PUT operation. |
| refunded_amount | decimal | The amount refunded from this transaction. |
| order_is_digital | boolean | Whether this is an order for digital products. |
| store_credit_amount | decimal | Represents the store credit that the shopper has redeemed on this individual order. This is a read-only value. Do not pass in a POST or PUT. |
| gift_certificate_amount | decimal | A read-only value. Do not pass in a POST or PUT. |
| ip_address | string | IP Address of the customer, if known. |
| geoip_country | string | The full name of the country where the customer made the purchase, based on the IP. |
| geoip_country_iso2 | string | The country where the customer made the purchase, in ISO2 format, based on the IP. |
| currency_id | int | The ID of the currency being used in this transaction. A read-only value. Do not pass in a POST or PUT. |
| currency_code | string | The currency code of the currency being used in this transaction. A read-only value. Do not pass in a POST or PUT. |
| currency_exchange_rate | decimal | A read-only value. Do not pass in a POST or PUT. |
| default_currency_id | int | A read-only value. Do not pass in a POST or PUT. |
| default_currency_code | string | The currency code of the default currency for this type of transaction. A read-only value. Do not pass in a POST or PUT. |
| staff_notes | text | Any additional notes for staff. |
| customer_message | text | Message that the customer entered into the `Order Comments` box during checkout. |
| discount_amount | decimal | Amount of discount for this transaction. |
| coupon_discount | decimal | A read-only value. Do not pass in a POST or PUT. |
| shipping_address_count | int | The number of shipping addresses associated with this transaction. A read-only value. Do not pass in a POST or PUT. |
| is_deleted | boolean | Indicates whether the order was deleted (archived). A read-only value. Do not pass in a POST or PUT. |
| is_email_opt_in | boolean | Indicates whether the shopper has selected an opt-in check box (on the checkout page) to receive emails. A read-only value. Do not pass in a POST or PUT. |
| ebay_order_id | string | If the order was placed through eBay, the eBay order number will be included. Otherwise, the value will be `0`. |
| billing_address | object | Contains the billing address details for this transaction, specifically: `first_name`, `last_name`, `company`, `street_1`, `street_2`, `city`, `state`, `zip`, `country`, `country_iso2`, `phone`, and `email`. Ensure that state names are spelled out in full, e.g.: `California`. Required for POST operations. |
| order_source | string | Orders submitted via the store's website will include a `www` value. Orders submitted via the API will be set to `external`. A read-only value. Do not pass in a POST or PUT. |
| external_source | string | For orders submitted or modified via the API, using a PUT or POST operation, you can optionally pass in a value identifying the system used to generate the order. For example: `POS`. Otherwise, the value will be null. |
| products | array | Array of [product](/api/v2/#product-object-properties) objects that make up the order. |
| shipping_addresses | array | This is an object array that has different syntax in different operations: <br><br> In PUT or POST operations, you can optionally pass a `shipping_addresses` object array containing one or more shipping addresses. However, if you include more than one address, only the first address will be used, because the API does not currently support shipping to more than one address. If you do not pass a shipping address, the billing address will be used. <br><br> For the full list of available name/value pairs, see the [Order Shipping Addresses](/api/v2/#order-shipping-addresses) object. Not all fields are required. For a syntax example of syntax, see the [Create an Order](/api/v2/#create-an-order) endpoint.<br><br> In GET and other operations, the `shipping_addresses` object will consist of two addresses. The first is the URI of a JSON object containing the shipping address details. The second is a context path that provides an alternate means of retrieving the data (if, for example, you prefer XML). For syntax, refer to the [List Orders](/api/v2/#list-orders) endpoint. |
| coupons | object | This object is read-only. Do not attempt to pass in a PUT or POST. Contains two name/value pairs: <br> The `url` property's value is the fully qualified address of a JSON object array, containing details of any coupon(s) associated with this transaction. <br> The `resource` property's value is the context path to the [Order Coupons](/api/v2/#order-coupons) resource, which provides an alternate means of retrieving the data (if, for example, you prefer XML). |

### <span class="jumptarget"> Order Webhook Events </span>

#### <span class="jumptarget"> Order Created </span>

```
store/order/created
```
Occurs when an order is received from the checkout, or when a manual order is created in the control panel.


#### <span class="jumptarget"> Order Updated </span>

```
store/order/updated
```
Occurs when order details are updated through the control panel, or when an order status is changed from the control panel or the API.

#### <span class="jumptarget"> Order Archived </span>

```
store/order/archived
```
Occurs when an order is archived from the control panel.
