# <span class="jumptarget"> Shipping Methods Reference </span>

The Shipping Methods object and endpoints help manage the shipping of physical items from merchant to shopper.

## <span class="jumptarget"> Shipping Method Object – Properties </span>

A Shipping Method object represents a shipping method enabled within the store.

| Name | Type | Description |
| --- | --- | --- |
| id | int | Shipping-method ID. |
| name | string | Display name for shipping method. |
| type | string | Shipping-method type. The currently supported static/fixed shipping-quote types are [`perorder`](#perorder), [`peritem`](#peritem), [`weight`](#weight), or [`total`](#total). We plan to later add support for these dynamic/real-time shipping-quote types: `auspost`, `canadapost`, `endicia`, `usps`, `fedex`, `royalmail`, `ups`, `upsready`, `upsonline`, or `shipperhq`. |
| settings | object | Depends on the shipping-method `type`. See the supported `settings` object models [here](#settingstypes). |
| enabled | boolean | Whether or not this shipping-zone method is enabled. |
| handling_fees | object | Handling-fee information for this method. This object currently contains the following element: <br> `fixed_surcharge`: the handling fee. |

## <span class="jumptarget" id="settingstypes"> Settings Objects </span>

A shipping method's `type` and `settings` properties can match one of the following models:

### <span class="jumptarget" id="perorder"> perorder Object – Properties </span>

Object model for flat-rate shipping quotes per order.

| Name | Type | Description |
| --- | --- | --- |
| rate | number | Flat rate per order. |

#### <span class="jumptarget" id="perorder-ex"> JSON Example </span>

```json
    {
    "name": "Flat Rate per Order",
    "type": "perorder",
    "settings": {
      "rate": 7
    },
```

### <span class="jumptarget" id="peritem"> peritem Object – Properties </span>

Object model for flat-rate shipping quotes per item ordered.

| Name | Type | Description |
| --- | --- | --- |
| rate | number | Flat rate per item. |

#### <span class="jumptarget" id="peritem-ex"> JSON Example </span>

```json
    {
    "name": "Flat Rate per Item",
    "type": "peritem",
    "settings": {
      "rate": 8
    },
```

### <span class="jumptarget" id="weight"> weight Object – Properties </span>

Object model for shipping quotes by weight.

| Name | Type | Description |
| --- | --- | --- |
| default_cost | number | Default shipping cost, applied either as a percentage of the order's total value or as a fixed amount. |
| default_cost_type | string | How the default shipping cost is calculated. One of: `0:"percentage_of_total"`, or `1:"fixed_amount"`. |
| range | number | Array of [range](#range) objects. The units for these ranges' `lower_limit` and `upper_limit` properties are ounces. |


#### <span class="jumptarget" id="weight-ex"> JSON Example </span>
   
```json
{
"name": "Rate per Weight",
"type": "weight",
"settings": {
     "default_cost": 12,
     "default_cost_type": "fixed_amount",
     "range": [
       {
         "lower_limit": 0,
         "upper_limit": 20,
         "shipping_cost": 8
       },
       {
         "lower_limit": 20,
         "upper_limit": 40,
         "shipping_cost": 12
       }
     ]
   }
}
```

### <span class="jumptarget" id="total"> total Object – Properties </span>

Object model for shipping quotes by order's total value.

| Name | Type | Description |
| --- | --- | --- |
| default_cost | number | Default shipping cost, applied either as a percentage of the order's total value or as a fixed amount. |
| default_cost_type | string | How the default shipping cost is calculated. One of: `0:"percentage_of_total"`, or `1:"fixed_amount"`. |
| include_order_total_taxes | boolean | Whether or not to include taxes on the order's total value in the shipping-cost calculation. |
| range | number | Array of [range](#range) objects. The units for these ranges' `lower_limit` and `upper_limit` properties are values in the stores's currency. |

#### <span class="jumptarget" id="total-ex"> JSON Example </span>

This example sets free shipping above a certain order total:

```json
{
"name": "Per Total or Free",
"type": "total",
"settings": {
     "default_cost": 12,
     "default_cost_type": "fixed_amount",
     "include_order_total_taxes": 0,
     "range": [
       {
         "lower_limit": 0,
         "upper_limit": 5,
         "shipping_cost": 5
       },
       {
         "lower_limit": 5,
         "upper_limit": 10,
         "shipping_cost": 8
       },
       {
         "lower_limit": 10,
         "upper_limit": 20,
         "shipping_cost": 10
       },
       {
         "lower_limit": 20,
         "upper_limit": 49.99,
         "shipping_cost": 15
       },
       {
         "lower_limit": 50,
         "upper_limit": 100000,
         "shipping_cost": 0
       }       
     ]
   }
}
```

### <span class="jumptarget" id="range"> Range Object – Properties </span>

Object model to define ranges for shipping quotes. Units are defined in the calling object.

| Name | Type | Description |
| --- | --- | --- |
| lower_limit | number | Lower limit for order total. |
| upper_limit | number | Upper limit for order total. |
| shipping_cost | number | Shipping cost for orders whose total falls between the lower and upper limits. |

#### <span class="jumptarget" id="range-ex"> JSON Example </span>

```json
       {
         "lower_limit": 0,
         "upper_limit": 20,
         "shipping_cost": 8
       }
```
