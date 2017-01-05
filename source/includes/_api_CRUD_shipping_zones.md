## <span class="jumptarget"> List Shipping Zones </span>

Gets all shipping zones.

*   OAuth
`GET /api/v2/shipping/zones`  

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
[
  {
    "id": 1,
    "name": "United States",
    "type": "country",
    "locations": [
      {
        "id": 2,
        "country_iso2": "US"
      }
    ],
    "free_shipping": {
      "enabled": true,
      "minimum_sub_total": "10.0000",
      "exclude_fixed_shipping_products": false
    },
    "handling_fees": {
      "fixed_surcharge": "0.0000",
      "display_separately": true
    },
    "enabled": true
  },
  {
    "id": 2,
    "name": "Australia",
    "type": "country",
    "locations": [
      {
        "id": 3,
        "country_iso2": "AU"
      }
    ],
    "free_shipping": {
      "enabled": false,
      "minimum_sub_total": "0.0000",
      "exclude_fixed_shipping_products": false
    },
    "handling_fees": {
      "fixed_surcharge": "0.0000",
      "display_separately": true
    },
    "enabled": true
  }
]
```
  
## <span class="jumptarget"> Get a Shipping Zone </span>

Retrieves a specified shipping zone by zone ID.

*   OAuth
`GET /api/v2/shipping/zones/{id}`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* id

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
  "id": 1,
  "name": "United States",
  "type": "country",
  "locations": [
    {
      "id": 2,
      "country_iso2": "US"
    }
  ],
  "free_shipping": {
    "enabled": true,
    "minimum_sub_total": "10.0000",
    "exclude_fixed_shipping_products": false
  },
  "handling_fees": {
    "fixed_surcharge": "0.0000",
    "display_separately": true
  },
  "enabled": true
}
```

## <span class="jumptarget"> Create a Shipping Zone </span>

Creates a new shipping zone.

*   OAuth
`POST /api/v2/shipping/zones`


### <span class="jumptarget"> Request </span>

Example request object:

```json
{
 "name": "UnitedStates-NM",
 "type" : "state",
 "locations": [
   {
     "country_iso2": "US",
     "state_iso2": "NM"
   }
   ],
 "handling_fees": {
   "fixed_surcharge" : 12.00,
   "display_separately" : true
 }
}
```

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```
{
  "id": 2,
  "name": "UnitedStates-NM",
  "type": "state",
  "locations": [
    {
      "id": 2,
      "country_iso2": "US",
      "state_iso2": "NM"
    }
  ],
  "free_shipping": {
    "enabled": false,
    "minimum_sub_total": "0.0000",
    "exclude_fixed_shipping_products": false
  },
  "handling_fees": {
    "fixed_surcharge": "12.0000",
    "display_separately": true
  },
  "enabled": true
}
```

## <span class="jumptarget"> Update a Shipping Zone </span>

Updates an existing shipping zone.

*   OAuth
`PUT /api/v2/shipping/zones/{id}`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* id

### <span class="jumptarget"> Request </span>

Example request object:

```json
{
  "id": 2,
  "name": "UnitedStates-Samoa",
  "type": "state",
  "locations": [
    {
      "id": 5,
      "country_iso2": "US",
      "state_iso2": "AS"
    }
  ],
  "free_shipping": {
    "enabled": false,
    "minimum_sub_total": "0.0000",
    "exclude_fixed_shipping_products": false
  },
  "handling_fees": {
    "fixed_surcharge": "6.0000",
    "display_separately": true
  },
  "enabled": true
}
```

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```
{
  "id": 2,
  "name": "UnitedStates-Samoa",
  "type": "state",
  "locations": [
    {
      "id": 3,
      "country_iso2": "US",
      "state_iso2": "AS"
    }
  ],
  "free_shipping": {
    "enabled": false,
    "minimum_sub_total": "0.0000",
    "exclude_fixed_shipping_products": false
  },
  "handling_fees": {
    "fixed_surcharge": "6.0000",
    "display_separately": true
  },
  "enabled": true
}
```

## <span class="jumptarget"> Delete a Shipping Zone </span>

Deletes a specified shipping zone. (If successful, this will typically return a "204 No Content".)

*   OAuth
`DELETE /api/v2/shipping/zones/{id}`

### <span class="jumptarget"> Requirements </span>

The following properties of the shipping zone are required. The request won't be fulfilled unless these properties are valid.

* id


