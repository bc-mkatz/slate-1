# <span class="jumptarget"> Marketing Reference </span>

Marketing APIs support demand generation and loyalty programs. They include Coupons, Banners, and Gift Certificates.

## <span class="jumptarget"> Coupons </span>

Category or product discounts that can be applied to orders for customers who enter a given code.

### <span class="jumptarget"> Coupon Object – Properties </span>

| Name | Type | Description |
| --- | --- | --- |
| id | int | The coupon's ID. |
| name | string | The name of the coupon. |
| type | enum | Acceptable values for this enumerated field are: `per_item_discount`, `per_total_discount`, `shipping_discount`, `free_shipping`, or `percentage_discount`. |
| amount | decimal | The discount to apply to an order, as either an amount or a percentage. This field's usage is determined by the coupon `type`. For example, a `type` of `percentage_discount` would determine a percentage here. |
| min_purchase | decimal | Specifies a minimum value that an order must have before the coupon can be applied to it. |
| expires | date | Specifies when a coupon expires. Coupons need not have an expiry date – you can also control expiry via `max_uses` or `max_uses_per_customer`. If you do use this date field, the value must be in <a href="http://tools.ietf.org/html/rfc2822#section-3.3" target="_blank">RFC 2822</a> format. |
| enabled | boolean | If the coupon is enabled, this field's value is `true`; otherwise, `false`. |
| code | string | The coupon code that customers will use to receive their discounts. Value must be unique. |
| applies_to | object | Allows you to restrict a coupon to an entity type (category or product), and to specific categories/products. A value of `0` represents all categories/products. |
| num_uses | int | Number of times this coupon has been used. This is a read-only field; do not set or modify its value in a POST or PUT request. |
| max_uses | int | Maximum number of times this coupon can be used. |
| max_uses_per_customer | int | Maximum number of times each customer can use this coupon. |
| restricted_to | object | Allows you to restrict coupon usage based on locations, as follows:<br><br> To restrict a coupon by country, retrieve the list of ISO2 country codes  supported by BigCommmerce as described below under [Notes on Location Restrictions](#couponobjnote). Use the resulting ISO2 code as shown in this example: <br>  `"restricted_to": { "countries": ["AU"] }` <br><br> To restrict a coupon by state/province, retrieve BigCommmerce's list of supported state/province codes, indexed by ISO2 country codes, as described below under [Notes on Location Restrictions](#couponobjnote). Use the resulting state/province code as shown in this example: <br> `"restricted_to": { "states": { "AU": ["Australian Capital Territory"] } }` <br><br> To restrict a coupon by ZIP/postal codes, use BigCommerce's supported ZIP/postal-code patterns, which are indexed by ISO2 country codes. Please see <a href="https://support.bigcommerce.com/articles/Public/Adding-a-Shipping-Zone-by-Zip-or-Post-Code" target="_blank">this KB article</a> for an overview, and <a href="https://support.bigcommerce.com/articles/Public/Using-Coupon-Codes#advanced" target="_blank">this KB article</a> for format details. Use the resulting code as shown in this example: <br> `"restricted_to": { "zips": { "AU": ["2000", "20??"] } }` |
| shipping_methods | array | This is a list of shipping-method names. A shipping method must be enabled on the store to use it with a coupon. To check which shipping methods are enabled, please use the [List&#160;Shipping Methods](/api/v2/#list-shipping-methods) endpoint. |

### <span class="jumptarget" id="couponobjnote"> Notes on Location Restrictions </span>

For the `locations` property listed above, you can look up all `country_iso2` codes supported by BigCommerce by using the [List&#160;Countries](/api/v2/#list-countries) endpoint, with a request of the following form: 

```html
https://{store_hash}/api/v2/countries?limit=250
```

To look up all `state_iso2` codes supported by BigCommerce, you can use the [List States](/api/v2/#list-countries) endpoint, with a request of the following form. (To&#160;supply its `{country_id}` parameter, query the [List Countries](/api/v2/#list-states) endpoint as described just above.)

```html
https://{store_hash}/api/v2/countries/{country_id}/states
```   
 
For example, to look up codes for all U.S. states and territories, you would use a request of the following form:
 
```html
https://{store_hash}/api/v2/countries/226/states?limit=100
```
