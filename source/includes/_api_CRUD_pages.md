|||
|----|-----|
| **Manages** ||
| **OAuth Scopes** | store_v2_content |
||store_v2_content_read_only|

### <span class="jumptarget"> List Pages </span>

Gets the collection of pages. (Default sorting is by auto-generated ID. This usually generates an order of oldest-to-newest)

*   OAuth
 `GET /stores/{store_hash}/v2/pages/`
*   Basic Auth
 `GET /api/v2/pages`

#### <span class="jumptarget"> Pagination </span>

Parameters can be added to the URL query string to paginate the collection. If a limit isn’t provided, up to 50 pages are returned by default.

| Parameter | Type | Example |
| --- | --- | --- |
| Page | int | /stores/{store_hash}/v2/pages?page={number} |
| Limit | int | /stores/{store_hash}/v2/pages?limit={count} |

#### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
[
  {
    "id": 1,
    "name": "RSS Syndication",
    "meta_title": "",
    "body": "%%Syndicate%%",
    "is_visible": true,
    "parent_id": 0,
    "sort_order": 3,
    "meta_keywords": "",
    "type": "page",
    "meta_description": "",
    "is_homepage": false,
    "layout_file": "",
    "is_customers_only": false,
    "search_keywords": "",
    "has_mobile_version": false,
    "mobile_body": "",
    "url": "/mens/"
  },
  {
    "id": 2,
    "name": "Shipping & Returns",
    "meta_title": "",
    "body": "To edit this page, simply log in to the control panel, click the <strong style=\"font-weight: 400\">Website Content</strong> tab, and choose the <strong style=\"font-weight: 400\"> View Web Pages</strong> option. Click <strong style=\"font-weight: 400\">Edit</strong> next to the <strong style=\"font-weight: 400\">Shipping & Returns</strong> page, and you can change this text. A sample returns policy is shown below, which you can edit as needed. <br/><br/> <em style=\"font-style: normal\"><strong>Returns Policy</strong></em><strong style=\"font-weight: 400\"></em></em><em style=\"font-style: normal\"><br/><br/></em>You may return most new, unopened items within 30 days of delivery for a full refund. We'll also pay the return shipping costs if the return is a result of our error (you received an incorrect or defective item, etc.).<br/><br/>You should expect to receive your refund within four weeks of giving your package to the return shipper, however, in many cases you will receive a refund more quickly. This time period includes the transit time for us to receive your return from the shipper (5 to 10 business days), the time it takes us to process your return once we receive it (3 to 5 business days), and the time it takes your bank to process our refund request (5 to 10 business days).<br/><br/>If you need to return an item, please <a href=\"/contact-us/\">Contact Us</a> with your order number and details about the product you would like to return. We will respond quickly with instructions for how to return items from your order.<br/><br/></strong><strong>Shipping</em></em></em></strong><strong style=\"font-weight: 400\"><em style=\"font-style: normal\"><br/><br/></em>We can ship to virtually any address in the world. Note that there are restrictions on some products, and some products cannot be shipped to international destinations.<br/><br/>When you place an order, we will estimate shipping and delivery dates for you based on the availability of your items and the shipping options you choose. Depending on the shipping provider you choose, shipping date estimates may appear on the shipping quotes page.<br/><br/>Please also note that the shipping rates for many items we sell are weight-based. The weight of any such item can be found on its detail page. To reflect the policies of the shipping companies we use, all weights will be rounded up to the next full pound.</strong><br/>",
    "is_visible": true,
    "parent_id": 0,
    "sort_order": 2,
    "meta_keywords": "",
    "type": "page",
    "meta_description": "",
    "is_homepage": false,
    "layout_file": "page.html",
    "is_customers_only": false,
    "search_keywords": "",
    "has_mobile_version": false,
    "mobile_body": "",
    "url": "/shoes/"
  },
  {
    "id": 3,
    "name": "Blog",
    "is_visible": true,
    "parent_id": 0,
    "sort_order": 2,
    "type": "blog_index",
    "is_homepage": false,
    "is_customers_only": false
  },
  {
    "id": 4,
    "name": "Contact Us",
    "meta_title": "",
    "email": "",
    "body": "We're happy to answer questions or help you with returns.<br/>Please fill out the form below if you need assistance.",
    "is_visible": true,
    "parent_id": 0,
    "sort_order": 1,
    "meta_keywords": "",
    "type": "contact_form",
    "contact_fields": "fullname,phone,orderno",
    "meta_description": "",
    "is_homepage": false,
    "layout_file": "page.html",
    "is_customers_only": false,
    "search_keywords": "",
    "has_mobile_version": false,
    "mobile_body": "",
    "url": "/contact-us/"
  },
  {
  "id": 5,
  "name": "Raw Test Page",
  "body": "<html><head><title>Raw Page</title></head><body>This page type can store raw HTML</body></html>",
  "is_visible": true,
  "parent_id": 0,
  "sort_order": 3,
  "type": "raw",
  "is_homepage": false,
  "is_customers_only": false,
  "search_keywords": "",
  "has_mobile_version": true,
  "mobile_body": "<html><head><title>Page</title></head><body>Mobile Content can be raw as well</body></html>",
  "url": "/Raw-Body-Test-Page/"
  }
]
```

### <span class="jumptarget"> Get a Page </span>

Gets a page.

*   OAuth
`GET /stores/{store_hash}/v2/pages/{id}`
*   Basic Auth
`GET /api/v2/pages/{id}`

#### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
  "id": 3,
  "name": "Blog",
  "is_visible": true,
  "parent_id": 0,
  "sort_order": 2,
  "type": "blog_index",
  "is_homepage": false,
  "is_customers_only": false
}
```

### <span class="jumptarget"> Create a Page </span>

Creates a new page.

*   OAuth
`POST /stores/{store_hash}/v2/pages`
*   Basic Auth
`POST /api/v2/pages`

#### <span class="jumptarget"> Read-only Properties </span>

The following property of the page is read-only. If it is included in the request, the request will be rejected:

*   id

#### <span class="jumptarget"> Requirements </span>

The following properties of the page are required. The request won’t be fulfilled unless these properties are valid:

*   type
*   name
*   link (for a page of `type: link`)
*   feed (for a page of `type: rss_feed`)
*   body (for a page of `type: raw`)

#### <span class="jumptarget"> Notes </span>

Although the `is_homepage` property is writeable, setting it to `true` does not (currently) reset other instances of this property. When setting this property, please keep this known issue in mind.

#### <span class="jumptarget"> Request </span>

Example request object:

```json
{
   "type": "raw",
   "name": "404 Page for Cats",
   "url": "/404-meow/",
   "body": "<html><head><title>Hairball! Not Found</title></head><body>Sorry! You can not haz cheeseburger.</body></html>",
   "mobile_body": "",
   "has_mobile_version": false,
   "is_visible": true,
   "is_homepage": false,
   "is_customers_only": false,
   "sort_order": 12,
   "search_keywords": "dead, missing, broken"
}
```

#### <span class="jumptarget"> Response </span>

Example JSON returned in the response:

```json
{
 "id": 12,
 "name": "404 Page for Cats",
 "body": "<html><head><title>Hairball! Not Found</title></head><body>Sorry! You can not haz cheeseburger.</body></html>",
 "is_visible": true,
 "parent_id": 0,
 "sort_order": 12,
 "type": "raw",
 "is_homepage": false,
 "is_customers_only": false,
 "search_keywords": "dead, missing, broken",
 "has_mobile_version": false,
 "mobile_body": "",
 "url": "/404-meow/"
}
```

### <span class="jumptarget"> Delete a Page </span>

Deletes a page.

*   OAuth
`DELETE /stores/{store_hash}/v2/pages/{id}`
*   Basic Auth
`DELETE /api/v2/pages/{id}`
