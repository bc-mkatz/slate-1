## <span class="jumptarget"> Shipments </span>

Tracks a package consignment from an order that is shipped from the seller to the buyer.

### <span class="jumptarget"> Shipment Object – Properties </span>

| Name | Type | Description |
| --- | --- | --- |
| id | int | Shipment ID. |
| order_id | int | ID of the order associated with this shipment. |
| customer_id | int | ID of this order's customer. |
| order_address_id | int | ID of the associated order address. |
| date_created | date | Creation date for the shipment. |
| tracking_number | string | Tracking number of the shipment. |
| shipping_method | string | Extra detail to describe the shipment, with values like: `Standard`, <br> `My Custom Shipping Method Name`, etc. Can also be used for live quotes from some shipping providers. |
| shipping_provider | string | Enum of the BigCommerce shipping-carrier integration/module. <br>  (<strong>Note:</strong> This property should be included in a POST request to create a shipment object. If it is omitted from the request, the property's value will default to `custom`, and no tracking link will be generated in the email. To avoid this behavior, you can pass the property as an empty string.) |
| tracking_carrier | string | Enum of the delivery service fulfilling the shipment. |
| comments | text | Comments the shipper wishes to add. |
| billing_address | object | Billing address for this order's customer. |
| shipping_address | object | Shipping address for this order's customer. |
| items | object_array | The items in the shipment. This object has the following members, all integer: `order_product_id` (required), `quantity` (required), `product_id` (read-only). A sample `items` value might be: `[ {"order_product_id":16,"product_id": 0,"quantity":2} ]` |
