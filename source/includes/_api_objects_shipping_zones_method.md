## <span class="jumptarget"> Shipping Method Object – Properties </span>

A Shipping Method object represents a shipping method enabled within the store.

| Name | Type | Description |
| --- | --- | --- |
| id | int | Shipping-method ID. |
| name | string | Display name for shipping method. |
| type | string | Shipping-method type. Possible static/fixed shipping quote types are `perorder`, `peritem`, `weight`, or `total`. Possible dynamic/real-time shipping quote types are: `auspost`, `canadapost`, `endicia`, `usps`, `fedex`, `royalmail`, `ups`, `upsready`, `upsonline`, or `shipperhq`. |
| settings | object | [Depends on type.] |
| enabled | boolean | Whether or not this shipping-zone method is enabled. |
| handling_fee | int | Set handling fee for this method, if the zone's handling-fee type is defined as `method`. |
| handling_fees | object | Handling-fee information for this method, if the zone's handling-fee type is _not_ `method`. This object contains the following elements: <br> `fixed_surcharge`: the handling fee;<br> `display_separately`: Whether to display the handling fee separately at checkout. |

<strike> ### <span class="jumptarget"> Note to Reviewers </span>

Undocumented here (so far) are shipper-specific "models" in the Swagger like this one:

![Undocumented objects](ship-zone-method-models-undocumented.png) </strike>