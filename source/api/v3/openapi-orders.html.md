---
title: BigCommerce Orders API v3.0.0
layout: "apitwocolumn"
language_tabs:
  - ''
toc_footers: []
includes: []
search: true
highlight_theme: darkula
---

# BigCommerce Orders API v3.0.0

A Swagger Document for the BigCommmerce API V3.

Base URL = https://api.bigcommerce.com/stores/{{store_id}}/v3

<a href="http://www.bigcommerce.com/terms">Terms of service</a>



# Orders

BigCommerce Orders API Definition.

## getTransactions

> Code samples

`GET /orders/{order_id}/transactions`

Returns a paginated collection of `Transaction` objects related to a BigCommerce Order.


### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
order_id|path|number|true|The ID of the `Order` to which the transactions belong.



##### order_id
The ID of the `Order` to which the transactions belong.

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|An array of transactions.

204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No content found to fulfill request.

404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|The resource was not found.


> Example responses

````json
{
  "data": [
    {
      "id": 0,
      "order_id": "string",
      "event": "purchase",
      "method": "credit_card",
      "amount": 0,
      "currency": "string",
      "gateway": "2checkout",
      "gateway_transaction_id": "string",
      "date_created": "string",
      "test": true,
      "status": "ok",
      "fraud_review": true,
      "avs_result": [
        {
          "code": "string",
          "message": "string",
          "street_match": "string",
          "postal_match": "string"
        }
      ],
      "cvv_result": [
        {
          "code": "string",
          "message": "string"
        }
      ],
      "credit_card": [
        {
          "card_type": "string",
          "card_iin": "string",
          "card_last4": "string"
        }
      ],
      "gift_certificate": [
        {
          "code": "string",
          "original_balance": "string",
          "starting_balance": "string",
          "remaining_balance": "string",
          "status": "active"
        }
      ],
      "store_credit": [
        {
          "remaining_balance": "string"
        }
      ],
      "offline": [
        {
          "display_name": "string"
        }
      ],
      "custom": [
        {
          "payment_method": "string"
        }
      ]
    }
  ],
  "meta": {
    "total": 0,
    "count": 0,
    "per_page": 0,
    "current_page": 0,
    "total_pages": 0,
    "links": {
      "previous": "string",
      "current": "string",
      "next": "string"
    }
  }
}
````
````json
{
  "status": 0,
  "title": "string",
  "type": "string",
  "instance": "string"
}
````
````json
{
  "status": 0,
  "title": "string",
  "type": "string",
  "instance": "string"
}
````
<aside class="success">
This operation does not require authentication
</aside>

