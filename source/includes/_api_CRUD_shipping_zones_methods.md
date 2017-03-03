## <span class="jumptarget"> List Shipping Methods </span>

Gets all configured shipping methods, by `zone_id`. (Default sorting is by shipping-method `id`, from lowest to highest.)

*   OAuth
>`GET /stores/{store_hash}/api/v2/shipping/zones/{zone_id}/methods`
*   Basic Auth
>`GET /api/v2/shipping/zones/{zone_id}/methods`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* zone_id

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
[
  {
    "id": 3,
    "name": "Flat Rate",
    "type": "peritem",
    "settings": {
      "rate": 9
    },
    "enabled": true,
    "handling_fees": {
      "fixed_surcharge": 0
    }
  },
  {
    "id": 4,
    "name": "Ship by Weight",
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
    },
    "enabled": true,
    "handling_fees": {
      "fixed_surcharge": 0
    }
  }
]
```

## <span class="jumptarget"> Get a Shipping Method </span>

Gets a shipping method, specified by `zone_id` and `method_id`.

*   OAuth
>`GET /stores/{store_hash}/api/v2/shipping/zones/{zone_id}/methods/{method_id}`
*   Basic Auth
>`GET /api/v2/shipping/zones/{zone_id}/methods/{method_id}`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* zone_id
* method_id

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
  "id": 3,
  "name": "Flat Rate",
  "type": "peritem",
  "settings": {
    "rate": 9
  },
  "enabled": true,
  "handling_fees": {
    "fixed_surcharge": 0
  }
}
```

## <span class="jumptarget"> Create a Shipping Method </span>

Creates a new method in the specificed shipping zone.

*   OAuth
>`POST /stores/{store_hash}/api/v2/shipping/zones/{zone_id}/methods`
*   Basic Auth
>`POST /api/v2/shipping/zones/{zone_id}/methods`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* zone_id

### <span class="jumptarget"> Request </span>

Example request object:

```json
{
  "name": "Per Order",
  "type": "perorder",
  "settings": {
    "rate": 8
  },
  "enabled": true,
  "handling_fees": {
    "fixed_surcharge": 3
  }
}
```

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
  "id": 5,
  "name": "Per Order",
  "type": "perorder",
  "settings": {
    "rate": 8
  },
  "enabled": true,
  "handling_fees": {
    "fixed_surcharge": 3
  }
}
```

## <span class="jumptarget"> Update a Shipping Method </span>

Updates an existing shipping method.

*   OAuth
>`PUT /stores/{store_hash}/api/v2/shipping/zones/{zone_id}/methods/{method_id}`
*   Basic Auth
>`PUT /api/v2/shipping/zones/{zone_id}/methods/{method_id}`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* zone_id
* method_id

### <span class="jumptarget"> Request </span>

Example request object:

```json
{
  "settings": {
    "rate": 11
  },
  "handling_fees": {
    "fixed_surcharge": 0
  }
}  
```

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
  "id": 5,
  "name": "Per Order",
  "type": "perorder",
  "settings": {
    "rate": 11
  },
  "enabled": true,
  "handling_fees": {
    "fixed_surcharge": 0
  }
}
```

## <span class="jumptarget"> Delete a Shipping Method </span>

Deletes a specified shipping method. (If successful, this will typically return a "204 No Content".)

*   OAuth
>`DELETE /stores/{store_hash}/api/v2/shipping/zones/{zone_id}/methods/{method_id}`
*   Basic Auth
>`DELETE /api/v2/shipping/zones/{zone_id}/methods/{method_id}`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* zone_id
* method_id
