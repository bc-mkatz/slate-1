## <span class="jumptarget"> Pages </span>

A static Web page on the storefront.

### <span class="jumptarget"> Page Object – Properties </span>

| Name | Type | Description |
| --- | --- | --- |
| id | int | Unique ID of this Web page. |
| parent_id | int | ID of any parent Web page. |
| type | enum | Enum identifying this page's type, with the following possible values:<br> `page`: free-text page;<br> `link`: link to another Web address;<br> `rss_feed`: syndicated content from an RSS feed;<br> `contact_form`: a contact form;<br> `raw`: a page that allows for raw HTML to be entered into the body. (Note: No template is used when rendering the page.) |
| contact_fields | object | Where the page's type is a contact form: object whose members are the fields enabled (in the control panel) for storefront display. Possible members are:<br> `fullname`: full name of the customer submitting the form;<br> `phone`: customer's phone number, as submitted on the form;<br> `companyname`: customer's submitted company name;<br> `orderno`: customer's submitted order number;<br> `rma`: customer's submitted RMA (Return Merchandise Authorization) number. |
| email | string | Where the page's type is a contact form: email address that receives messages sent via the form.|
| name | string | Page name, as displayed on the storefront. |
| url | string | Relative URL on the storefront for this page. |
| meta_description | text | Description contained within this page's `<meta>` element. |
| body | text | HTML or variable that populates this page's `<body>` element, in default/desktop view. |
| mobile_body | text | HTML or variable that populates this page's `<body>` element, in mobile view. |
| has_mobile_version | boolean | If `true`, this page has a mobile version. |
| is_visible | boolean | If `true`, this page appears in the storefront's navigation menu.|
| is_homepage | boolean | If `true`, this page is the storefront's home page. |
| meta_title | string | Text specified for this page's `<title>` element. (If empty, the value of the `name` property is used.) |
| layout_file | string | Layout template for this page. |
| sort_order | int | Order in which this page should display on the storefront. (Lower integers specify earlier display.) |
| meta_title | string | Text contained within this page's `<title>` element.|
| search_keywords | string | Comma-separated list of keywords that shoppers can use to locate this page when searching the store.|
| meta_keywords | string | Comma-separated list of SEO-relevant keywords to include in the page's `<meta>` element. |
| link | string | Where the page's type is a link: this is the target link. |
| feed | string | Where the page's type is an RSS feed: the feed to syndicate. |
