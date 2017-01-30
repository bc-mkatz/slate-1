# <span class="jumptarget"> Media Types</span>

## <span class="jumptarget"> Introduction to Media Types</span>

The BigCommerce API can accept requests, and respond, in either JSON or XML. You should encode requests using the UTF-8 character set. (Other character sets might have unpredictable results.)

<aside class="warning">
<span class="aside-warning-hd">Restricted XML Support</span><br><br>
The XML media type is deprecated. Our v2 webhooks support JSON only, and Stores API versions after v2 will support JSON only. 
</aside>

## <span class="jumptarget"> Request Content Type</span>

When performing a request that contains a body (eg. `POST` or `PUT`), the type of content you are sending needs to be specified in the `Content-Type` header. The values for this header are specified in the data types below. For example, to send an XML body, the header would be: `Content-Type: application/xml`

## <span class="jumptarget"> Response Content Type</span>

There are several ways in which you can specify the type of content you would like to receive. The first method is by specifying an `Accept` header, the second is by supplying an extension to the resource you are request. Extensions are useful for browser-based testing.

The priority in which these methods are processed is outlined below:

1.  Accept header high-priority types (eg. `Accept: application/xml`) extensions on the resource (e.g.: `customers.xml`).

2.  Accept header low priority types (priorities less than 1, e.g.: `Accept: application/json;q=0.9`).

## <span class="jumptarget"> JSON</span>

JSON has a content type of `application/json`.

### <span class="jumptarget"> Request Structure</span>

The body of a JSON request is simply an object containing a set of key-value pairs. A simple representation of a product object is:

```json
{
     "id": 5,
     "name": "iPod",
     "description": "A portable MP3 music player."
 } 
```

### <span class="jumptarget"> Response Structure</span>

Responses are structured similarly to requests. If a request returns a single object, then the response will contain a single object, containing the fields for that resource.

The response will also contain links to any sub-resource – for example, `images` on the product below:

```json
{
  "id":1,
  "name":"[Sample Product] iPod Shuffle",
  "sku":"IPOD-SHUFFLE",
  "description":"The world’s smallest digital music player, ...",
  "date created":"Mon, 12 Jan 2009 10:22:39 +0000",
  "categories":[
    2,
    3
  ],
  "date modified":"Sun, 28 Aug 2011 23:08:56 +0000",
  "custom url":"\/products\/sample-product-ipod-shuffle.html",
  "brand":{
    "url":"https:\/\/www.example.com\/api\/v2\/brands\/1.json",
    "resource":"\/brands\/1"
  },
  "images":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/images.json",
    "resource":"\/products\/1\/images"
  },
  "discount rules":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/discountrules.json",
    "resource":"\/products\/1\/discountrules"
  },
  "configurable fields":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/configurablefields.json",
    "resource":"\/products\/1\/configurablefields"
  },
  "custom fields":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/customfields.json",
    "resource":"\/products\/1\/customfields"
  },
  "videos":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/videos.json",
    "resource":"\/products\/1\/videos"
  },
  "skus":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/skus.json",
    "resource":"\/products\/1\/skus"
  },
  "rules":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/rules.json",
    "resource":"\/products\/1\/rules"
  },
  "option_set":{
    "url":"https:\/\/www.example.com\/api\/v2\/optionsets\/15.json",
    "resource":"\/optionsets\/15"
  },
  "options":{
    "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/options.json",
    "resource":"\/products\/1\/options"
  },
  "availability":"available"
}
```

If the request returns more than one result, then the response will consist of an array of objects for each result:

```json
[
  {
    "id":1,
    "name":"[Sample Product] iPod Shuffle",
    "sku":"IPOD-SHUFFLE",
    "description":"The world’s smallest digital music player, ...",
    "search_keywords":"",
    "availability_description":"",
    "is_price_hidden":false,
    "price_hidden_label":"",
    "categories":[
      2,
      3
    ],
    "date_modified":"Sun, 28 Aug 2011 23:08:56 +0000",
    "bin_picking_number":"",
    "custom_url":"\/products\/sample-product-ipod-shuffle.html",
    "brand":{
      "url":"https:\/\/www.example.com\/api\/v2\/brands\/1.json",
      "resource":"\/brands\/1"
    },
    "images":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/images.json",
      "resource":"\/products\/1\/images"
    },
    "discount_rules":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/discountrules.json",
      "resource":"\/products\/1\/discountrules"
    },
    "configurable_fields":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/configurablefields.json",
      "resource":"\/products\/1\/configurablefields"
    },
    "custom_fields":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/customfields.json",
      "resource":"\/products\/1\/customfields"
    },
    "videos":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/videos.json",
      "resource":"\/products\/1\/videos"
    },
    "skus":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/skus.json",
      "resource":"\/products\/1\/skus"
    },
    "rules":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/rules.json",
      "resource":"\/products\/1\/rules"
    },
    "option_set":{
      "url":"https:\/\/www.example.com\/api\/v2\/optionsets\/15.json",
      "resource":"\/optionsets\/15"
    },
    "options":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/1\/options.json",
      "resource":"\/products\/1\/options"
    },
    "availability":"available"
  },
  {
    "id":2,
    "name":"[Sample Product] iPod Nano",
    "sku":"",
    "description":"Color isn't the only brilliant new iPod Nano feature. ...",
    "date_created":"Mon, 12 Jan 2009 10:28:58 +0000",
    "brand_id":1,
    "view_count":11,
    "page_title":"",
    "meta_keywords":"",
    "meta_description":"",
    "layout":"product.html",
    "is_price_hidden":false,
    "price_hidden_label":"",
    "categories":[
      3
    ],
    "date_modified":"Thu, 18 Aug 2011 05:42:15 +0000",
    "bin_picking_number":"",
    "custom_url":"\/products\/sample-product-ipod-nano.html",
    "brand":{
      "url":"https:\/\/www.example.com\/api\/v2\/brands\/1.json",
      "resource":"\/brands\/1"
    },
    "images":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/images.json",
      "resource":"\/products\/2\/images"
    },
    "discount_rules":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/discountrules.json",
      "resource":"\/products\/2\/discountrules"
    },
    "configurable_fields":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/configurablefields.json",
      "resource":"\/products\/2\/configurablefields"
    },
    "custom_fields":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/customfields.json",
      "resource":"\/products\/2\/customfields"
    },
    "videos":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/videos.json",
      "resource":"\/products\/2\/videos"
    },
    "skus":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/skus.json",
      "resource":"\/products\/2\/skus"
    },
    "rules":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/rules.json",
      "resource":"\/products\/2\/rules"
    },
    "options":{
      "url":"https:\/\/www.example.com\/api\/v2\/products\/2\/options.json",
      "resource":"\/products\/2\/options"
    },
    "availability":"available"
  }
]
```

## <span class="jumptarget"> XML</span>

XML has a content type of `application/xml`. All XML transactions begin with the standard XML declaration:

```xml
<?xml version="1.0" encoding="UTF-8"?>

```

### <span class="jumptarget"> Request Structure</span>

The body of an XML request should first contain an element that is named according to the resource, in singular form, such as `product` for the `products` resource:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<product> 
</product>

```

The resource element should then contain a set of elements that match the fields described in that resource's documentation:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<product>
    <id>5</id>
    <name>iPod</name>
    <description>A portable MP3 music player.</description>
</product>

```

### <span class="jumptarget"> Response Structure</span>

To receive an XML response, the request URI should include an .xml extension, as shown here:

```
GET /customers/1.xml
```

Here is a corresponding response:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<customer>
  <id>1</id>
  <company>BigCommerce<company>
  <first_name>Mister</first_name>
  <last_name>Big</last_name>
  <email>mister.big@bigcommerce.com</email>
  <phone></phone>
  <date_created>Tue, 16 Aug 2011 23:15:07 +0000</date_created>
  <date_modified>Tue, 16 Aug 2011 23:16:37 +0000</date_modified>
  <store_credit>0.0000</store_credit>
  <registration_ip_address>10.1.1.102</registration_ip_address>
  <customer_group_id>0</customer_group_id>
  <notes>NULL</notes>
  <addresses>
    <link rel="resource" href="https://www.example.com/api/v2/customers/1/addresses.xml">/customers/1/addresses</link>
  </addresses>
</customer>

```

If the request returns more than one result, then the response will consist of an element named according to the resource, in plural form, which contains a set of objects for each result:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<customers>
  <customer>
    <id>1</id>
    <company>BigCommerce</company>
    <first_name>Mister</first_name>
    <last_name>Big</last_name>
    <email>mister.big@bigcommerce.com</email>
    <phone></phone>
    <date_created>Tue, 16 Aug 2011 23:15:07 +0000</date_created>
    <date_modified>Tue, 16 Aug 2011 23:16:37 +0000</date_modified>
    <store_credit>0.0000</store_credit>
    <registration_ip_address>10.1.1.102</registration_ip_address>
    <customer_group_id>0</customer_group_id>
    <notes>NULL</notes>
    <addresses>
      <link rel="resource" href="https://www.example.com/api/v2/customers/1/addresses.xml">/customers/1/addresses</link>
    </addresses>
  </customer>
</customers>

```
