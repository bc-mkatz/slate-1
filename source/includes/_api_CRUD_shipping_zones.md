## <span class="jumptarget"> List Shipping Zones </span>

Gets all shipping zones.

*   OAuth
`GET /api/v2/shipping/zones`  

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
    {
      "currencies": {
        "currency": [
          {
            "id": 3,
            "is_default": "false",
            "date_created": "Thu, 11 Sep 2014 17:10:12 +0000",
            "date_modified": "Thu, 08 Jan 2015 15:12:48 +0000",
            "country_iso2": "AU",
            "currency_code": "AUD",
            "currency_exchange_rate": "1.3885600000",
            "auto_update": "false",
            "location": "left",
            "token": "$",
            "decimal_token": ".",
            "thousands_token": ",",
            "decimal_places": 2
          },
          {
            "id": 4,
            "is_default": "false",
            "date_created": "Thu, 11 Sep 2014 17:10:12 +0000",
            "date_modified": "Thu, 08 Jan 2015 15:12:48 +0000",
            "country_iso2": "US",
            "currency_code": "USD",
            "currency_exchange_rate": "1.0000000000",
            "auto_update": "false",
            "location": "left",
            "token": "$",
            "decimal_token": ".",
            "thousands_token": ",",
            "decimal_places": 2
          },
          {
            "id": 5,
            "is_default": "false",
            "date_created": "Thu, 11 Sep 2014 17:10:12 +0000",
            "date_modified": "Thu, 08 Jan 2015 15:12:48 +0000",
            "country_iso2": "CA",
            "currency_code": "CAD",
            "currency_exchange_rate": "0.7500000000",
            "auto_update": "false",
            "location": "left",
            "token": "$",
            "decimal_token": ".",
            "thousands_token": ",",
            "decimal_places": 2
          }
        ]
      }
    }
```
  
## <span class="jumptarget"> Get a Currency </span>

Retrieves a specified currency.

*   OAuth
`GET /stores/{store_hash}/v2/currencies/{id}`
*   Basic Auth
`GET /api/v2/currencies/{id}`

### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
    "id": 3,
    "is_default": "false",
    "date_created": "Thu, 11 Sep 2014 17:10:12 +0000",
    "date_modified": "Thu, 08 Jan 2015 15:12:48 +0000",
    "country_iso2": "AU",
    "currency_code": "AUD",
    "currency_exchange_rate": "1.3885600000",
    "auto_update": "false",
    "location": "left",
    "token": "$",
    "decimal_token": ".",
    "thousands_token": ",",
    "decimal_places": 2
}
```

## <span class="jumptarget"> Create a Currency </span>

Creates a new currency.

*   OAuth
`POST /stores/{store_hash}/v2/currencies`
*   Basic Auth
`POST /api/v2/currencies`

### <span class="jumptarget"> Read-only Properties </span>

The following properties of the currency are read-only. If one or more of these properties are included in the request, it will be rejected:

* id
* is_default
* date_created
* date_modified

#### <span class="jumptarget"> Notes </span>

The `is_default` property cannot be set programmatically. To change the store's default currency via the BigCommerce control panel, please see [this support article](https://support.bigcommerce.com/articles/Public/Managing-Currencies/?q=currency&l=en_US&fs=Search&pn=1#default).


### <span class="jumptarget"> Requirements </span>

The following properties of the currency are required. The request won't be fulfilled unless these properties are valid.

* country_iso2
* currency_code
* currency_exchange_rate
* auto_update
* location
* token
* decimal_token
* thousands_token
* decimal_places


### <span class="jumptarget"> Request </span>

Example request object:

```json
{
    "country_iso2": "AU",
    "currency_code": "AUD",
    "currency_exchange_rate": "1.3885600000",
    "auto_update": "false",
    "location": "left",
    "token": "$",
    "decimal_token": ".",
    "thousands_token": ",",
    "decimal_places": 2
}
```


## <span class="jumptarget"> Update a Currency </span>

Updates an existing currency.

*   OAuth
`PUT /stores/{store_hash}/v2/currencies/{ID}`
*   Basic Auth
`PUT /api/v2/currencies/{ID}`

### <span class="jumptarget"> Read-only Properties </span>

The following properties of the currency are read-only. If one or more of these properties are included in the request, it will be rejected:

* id
* is_default
* date_created
* date_modified


### <span class="jumptarget"> Request </span>

Example request object:

```json
{
    "country_iso2": "AU",
    "currency_code": "AUD",
    "currency_exchange_rate": "1.3885600000",
    "auto_update": "false",
    "location": "left",
    "token": "$",
    "decimal_token": ".",
    "thousands_token": ",",
    "decimal_places": 2
}
```

## <span class="jumptarget"> Delete a Currency </span>

Deletes a specified currency. (If successful, this will typically return a "204 No Content".)

*   OAuth
`DELETE /stores/{store_hash}/v2/currencies/{id}`
*   Basic Auth
`DELETE /api/v2/currencies/{id}`

## <span class="jumptarget"> Delete All Currencies </span>

Deletes all currencies associated with the store. (If successful, this will typically return a "204 No Content".)

*   OAuth
`DELETE /stores/{store_hash}/v2/currencies`
*   Basic Auth
`DELETE /api/v2/currencies` 
