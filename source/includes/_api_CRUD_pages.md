|||
|----|-----|
| **Manages** ||
| **OAuth Scopes** | store_v2_content |
||store_v2_content_read_only|

### <span class="jumptarget"> List Pages </span>

Gets the collection of pages. (Default sorting is by published_date, from most-recent to earliest.)

*   OAuth
 `GET /stores/{store_hash}/v2/pages/`
*   Basic Auth
 `GET /api/v2/pages`

#### <span class="jumptarget"> Filters </span>

Filter parameters can be added to the URL query string to select specific pages in the collection.

**[Lawrence: Need filters. The struck-out text below is copied/pasted from the Blog Posts API docs. Thanks.]**

<strike>
| Parameter | Type | Example |
| --- | --- | --- |
| is_published | string | /stores/{store_hash}/v2/blog/posts?is_published={value} |
| url | string | /stores/{store_hash}/v2/blog/posts?url={value} |
</strike>

#### <span class="jumptarget"> Pagination </span>

Parameters can be added to the URL query string to paginate the collection. The maximum limit is 250. If a limit isn’t provided, up to 50 pages are returned by default.

**[Lawrence: Need paginators. The struck-out text below is copied/pasted from the Blog Posts API docs. Thanks.]**

<strike>
| Parameter | Type | Example |
| --- | --- | --- |
| Page | int | /stores/{store_hash}/v2/blog/posts?page={number} |
| Limit | int | /stores/{store_hash}/v2/blog/posts?limit={count} |
</strike>

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

**[Lawrence: Sorry, but I need everything for this one – any read-only properties, any required properties, and any usage notes; plus, a sample Request body and (ideally) a sample JSON Response. Struck-out text below is copied/pasted from Blog Posts API. Thanks.]**

<strike>
#### <span class="jumptarget"> Read-only Properties </span>

The following properties of the page are read-only. If one or more of these properties are included in the request, it will be rejected.

*   id
*   preview_url
*   summary

#### <span class="jumptarget"> Requirements </span>

The following properties of the page are required. The request won’t be fulfilled unless these properties are valid.

*   title
*   body

#### <span class="jumptarget"> Notes </span>

??

#### <span class="jumptarget"> Request </span>

Example request object:

```json
{
  "title": "A Sample Blog Post",
  "body": "<p>This is a blog post.</p>",
  "author": "Author Name",
  "thumbnail_path": "http://cdn.example.com/sample-post.jpg",
  "is_published": true,
  "tags": [
    "Blog",
    "Example"
  ]
}
```
</strike>

### <span class="jumptarget"> Delete a Page </span>

Deletes a page.

*   OAuth
`DELETE /stores/{store_hash}/v2/pages/{id}`
*   Basic Auth
`DELETE /api/v2/pages/{id}`

### <span class="jumptarget"> Delete Multiple Pages </span>

Deletes multiple pages in the collection.

*   OAuth
`DELETE /stores/{store_hash}/v2/pages`
*   Basic Auth
`DELETE /api/v2/blog/pages/`

#### Pagination </span>

**[Lawrence: This section is copied/adapted from the Blog Posts API docs. Kindly correct this to the way  this endpoint is actually paginated. Thanks.]**

Parameters can be added to the URL query string to paginate the collection. The maximum limit is 250. If a limit isn’t provided, up to 50 pages are returned by default.

| Parameter | Type | Example |
| --- | --- | --- |
| Page | int | /api/v2/pages?page={number} |
| Limit | int | /api/v2/pages?limit={count} |
