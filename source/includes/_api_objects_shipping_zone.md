# <span class="jumptarget"> Shipping Zones Reference </span>

The Shipping Zone object and endpoints manage shipping zones within countries.

## <span class="jumptarget"> Shipping Zone Object – Properties </span>

| Name | Type | Description |
|---|---|---|
| id | int | Zone ID. | 
| name | string | Zone name. |
| type | string | Type of zone – one or more countries, a list of states, a list of ZIP/postal codes, or `global`. A value of `global` is treated as "rest of the world". If type is `global`, then `name` and `locations` are not mandatory. | 
| locations |array | Array of zone locations, each of which contains the following elements:<br> `id`: location's ID (integer);<br> `zip`: location's ZIP/postal code (string);<br> `country_iso2`: 2-letter [ISO Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) code for the country (string, see [Notes](#zoneobjnote) below);<br> `state_iso2`: [ISO Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) code for the state (string, see [Notes](#zoneobjnote) below). |
| free_shipping | object | You can limit free shipping to orders exceeding a certain subtotal value. You can make products with fixed-price shipping ineligible for free shipping, but such products' prices will still count toward the minimum order threshold. This object contains the following elements: <br> `enabled`: whether free shipping is enabled for this zone (boolean);<br> `minimum_sub_total`: order subtotal that establishes threshold for free shipping (number);<br> `exclude_fixed_shipping_products`: whether products with a fixed shipping cost are ineligible for free shipping (boolean). |
| handling_fees | object | Handling-fee information for this zone. Contains the following elements: <br> `fixed_surcharge`: the handling fee (number);<br> `display_separately`: whether to display the handling fee separately at checkout (boolean). |
| enabled | boolean | Whether this shipping zone is enabled. |


### <span class="jumptarget" id="zoneobjnote"> Notes </span>

For the `locations` property listed above, you can look up all `country_iso2` codes supported by BigCommerce by using the [List Countries](/api/v2/#list-countries) endpoint, with a request of the following form: 

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