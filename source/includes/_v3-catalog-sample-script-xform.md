<html>
 <head>
  <title>
   Sample Xformation &ndash; BigCommerce v3 Catalog API
  </title>
 </head>
 <body>
  <h1 class="jumptarget">
   Sample Xformation &ndash; v3 Catalog API
  </h1>
  <div class="">
   A Swagger export for the v3 BigCommmerce API.
  </div>
  <h2>
   Access
  </h2>
  <h2>
   <h2 id="__Methods" class="jumptarget"> Methods – Contents </h2>

  [ Jump to <a href="#__Models">Models</a> ]

<h3 class="jumptarget"> <a href="#Catalog">Catalog</a> </h3>

  <ul>
   <li>
    <a href="#catalogSummaryGet">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/summary
     </code>
    </a>
   </li>
   <li>
    <a href="#createBrand">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/brands
     </code>
    </a>
   </li>
   <li>
    <a href="#createBrandImage">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/brands/{brand_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#createBrandMetafield">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/brands/{brand_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#createCategory">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/categories
     </code>
    </a>
   </li>
   <li>
    <a href="#createCategoryImage">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/categories/{category_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#createCategoryMetafield">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/categories/{category_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#createComplexRule">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/complex-rules
     </code>
    </a>
   </li>
   <li>
    <a href="#createModifier">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/modifiers
     </code>
    </a>
   </li>
   <li>
    <a href="#createModifierImage">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/modifiers/{modifier_id}/values/{value_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#createOption">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/options
     </code>
    </a>
   </li>
   <li>
    <a href="#createProduct">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products
     </code>
    </a>
   </li>
   <li>
    <a href="#createProductImage">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/images
     </code>
    </a>
   </li>
   <li>
    <a href="#createProductMetafield">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#createProductVideo">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/videos
     </code>
    </a>
   </li>
   <li>
    <a href="#createVariant">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/variants
     </code>
    </a>
   </li>
   <li>
    <a href="#createVariantImage">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/variants/{variant_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#createVariantMetafield">
     <code>
      <span class="http-method">
       post
      </span>
      /catalog/products/{product_id}/variants/{variant_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteBrandById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/brands/{brand_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteBrandImage">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/brands/{brand_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteBrandMetafieldById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/brands/{brand_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteBrands">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/brands
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteCategories">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/categories
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteCategoryById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/categories/{category_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteCategoryImage">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/categories/{category_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteCategoryMetafieldById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/categories/{category_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteComplexRuleById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/complex-rules/{complex_rule_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteModifierById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/modifiers/{modifier_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteModifierImage">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/modifiers/{modifier_id}/values/{value_id}/image
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteOptionById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/options/{option_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteProductById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteProductImage">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/images/{image_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteProductMetafieldById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteProductVideo">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/videos/{video_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteProducts">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteVariantById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/variants/{variant_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteVariantMetafieldById">
     <code>
      <span class="http-method">
       delete
      </span>
      /catalog/products/{product_id}/variants/{variant_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getBrandById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/brands/{brand_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getBrandMetafieldByBrandId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/brands/{brand_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getBrandMetafieldsByBrandId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/brands/{brand_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#getBrands">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/brands
     </code>
    </a>
   </li>
   <li>
    <a href="#getCategories">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/categories
     </code>
    </a>
   </li>
   <li>
    <a href="#getCategoryById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/categories/{category_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getCategoryMetafieldByCategoryId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/categories/{category_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getCategoryMetafieldsByCategoryId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/categories/{category_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#getCategoryTree">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/categories/tree
     </code>
    </a>
   </li>
   <li>
    <a href="#getComplexRuleById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/complex-rules/{complex_rule_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getComplexRules">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/complex-rules
     </code>
    </a>
   </li>
   <li>
    <a href="#getModifierById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/modifiers/{modifier_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getModifiers">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/modifiers
     </code>
    </a>
   </li>
   <li>
    <a href="#getOptionById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/options/{option_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getOptions">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/options
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductImageById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/images/{image_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductImages">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/images
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductMetafieldByProductId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductMetafieldsByProductId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductVideoById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/videos/{video_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getProductVideos">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/videos
     </code>
    </a>
   </li>
   <li>
    <a href="#getProducts">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products
     </code>
    </a>
   </li>
   <li>
    <a href="#getVariantById">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/variants/{variant_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getVariantMetafieldByProductIdAndVariantId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/variants/{variant_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getVariantMetafieldsByProductIdAndVariantId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/variants/{variant_id}/metafields
     </code>
    </a>
   </li>
   <li>
    <a href="#getVariants">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/variants
     </code>
    </a>
   </li>
   <li>
    <a href="#getVariantsByProductId">
     <code>
      <span class="http-method">
       get
      </span>
      /catalog/products/{product_id}/variants
     </code>
    </a>
   </li>
   <li>
    <a href="#updateBrand">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/brands/{brand_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateBrandMetafield">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/brands/{brand_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateCategory">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/categories/{category_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateCategoryMetafield">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/categories/{category_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateComplexRule">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/complex-rules/{complex_rule_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateModifier">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/modifiers/{modifier_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateOption">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/options/{option_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateProduct">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateProductImage">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/images/{image_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateProductMetafield">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateProductVideo">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/videos/{video_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateVariant">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/variants/{variant_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#updateVariantMetafield">
     <code>
      <span class="http-method">
       put
      </span>
      /catalog/products/{product_id}/variants/{variant_id}/metafields/{metafield_id}
     </code>
    </a>
   </li>
  </ul>
  <h3 class="jumptarget"> <a href="#Customers">Customers</a> </h3>
  <ul>
   <li>
    <a href="#createSubscriber">
     <code>
      <span class="http-method">
       post
      </span>
      /customers/subscribers
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteSubscriberById">
     <code>
      <span class="http-method">
       delete
      </span>
      /customers/subscribers/{subscriber_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#deleteSubscribers">
     <code>
      <span class="http-method">
       delete
      </span>
      /customers/subscribers
     </code>
    </a>
   </li>
   <li>
    <a href="#getSubscriberById">
     <code>
      <span class="http-method">
       get
      </span>
      /customers/subscribers/{subscriber_id}
     </code>
    </a>
   </li>
   <li>
    <a href="#getSubscribers">
     <code>
      <span class="http-method">
       get
      </span>
      /customers/subscribers
     </code>
    </a>
   </li>
   <li>
    <a href="#updateSubscriber">
     <code>
      <span class="http-method">
       put
      </span>
      /customers/subscribers/{subscriber_id}
     </code>
    </a>
   </li>
  </ul>
  <h1>
   <a name="Catalog">
    Catalog
   </a>
  </h1>
  <div class="method">
   <a name="catalogSummaryGet">
   </a>
   <h2 class_="jumptarget" id="catalogSummaryGet">
    Returns a lightweight inventory summary from the BigCommerce Catalog.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/summary
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#CatalogSummaryResponse">
     CatalogSummaryResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "inventory_value" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_count" : 123,
    "primary_category_id" : 123,
    "primary_category_name" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of catalog summary and meta data
   <a href="#CatalogSummaryResponse">
    CatalogSummaryResponse
   </a>
  </div>
  <div class="method">
   <a name="createBrand">
   </a>
   <h2 class_="jumptarget" id="createBrand">
    Create a `Brand` object.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/brands
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Brand
     <a href="#Brand">
      Brand
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Brand` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#BrandResponse">
     BrandResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "meta_description" : "aeiou",
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "name" : "aeiou",
    "id" : 123,
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A brand object
   <a href="#BrandResponse">
    BrandResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   Brand was in conflict with another brand. This is the result of duplicate unique fields such as name.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   Brand was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createBrandImage">
   </a>
   <h2 class_="jumptarget" id="createBrandImage">
    Creates an image on a `Brand`. Publicly accessible URLs and files (form post) are valid parameters.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/brands/{brand_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the image is being attached to.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      multipart/form-data
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Form parameters
   </h3>
   <div class="field-items">
    <div class="param">
     image_file (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Form Parameter
     </span>
     — An image file. Support MIME types include GIF, JPEG, and PNG.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ImageResponse">
     ImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A ResourceImage and meta data
   <a href="#ImageResponse">
    ImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    422
   </h4>
   Image was not valid. This is the result of missing image_file field or incorrect file type. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createBrandMetafield">
   </a>
   <h2 class_="jumptarget" id="createBrandMetafield">
    Create a product `Metafield`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/brands/{brand_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A `Metafield` object
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Metafield` was in conflict with another `Metafield`. This can be the result of duplicate unique key combination of the app's client id, namespace, key, resource_type, and resource_id.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Metafield` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createCategory">
   </a>
   <h2 class_="jumptarget" id="createCategory">
    Creates a `Category` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/categories
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     category
     <a href="#Category">
      Category
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `Category` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#CategoryResponse">
     CategoryResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "is_visible" : true,
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "description" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou",
    "default_product_sort" : "aeiou",
    "meta_description" : "aeiou",
    "layout_file" : "aeiou",
    "parent_id" : 123,
    "name" : "aeiou",
    "id" : 123,
    "sort_order" : 123,
    "views" : 123,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    }
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A category object
   <a href="#CategoryResponse">
    CategoryResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Category` was in conflict with another category. This is the result of duplicate unique values such as name or custom_url.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Category` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createCategoryImage">
   </a>
   <h2 class_="jumptarget" id="createCategoryImage">
    Creates an image on a category. Publically accessible URLs and files (form post) are valid parameters.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/categories/{category_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      multipart/form-data
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Form parameters
   </h3>
   <div class="field-items">
    <div class="param">
     image_file (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Form Parameter
     </span>
     — An image file. Support MIME types include GIF, JPEG, and PNG.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ImageResponse">
     ImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A ResourceImage and meta data
   <a href="#ImageResponse">
    ImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    422
   </h4>
   Image was not valid. This is the result of missing image_file field or incorrect file type. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createCategoryMetafield">
   </a>
   <h2 class_="jumptarget" id="createCategoryMetafield">
    Create a product `Metafield`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/categories/{category_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A `Metafield` object
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Metafield` was in conflict with another `Metafield`. This can be the result of duplicate unique key combination of the app's client id, namespace, key, resource_type, and resource_id.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Metafield` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createComplexRule">
   </a>
   <h2 class_="jumptarget" id="createComplexRule">
    Create a `ComplexRule`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/complex-rules
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `ComplexRule` belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     ComplexRule
     <a href="#ComplexRule">
      ComplexRule
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `ComplexRule` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ComplexRuleResponse">
     ComplexRuleResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "purchasing_hidden" : true,
    "stop" : true,
    "price_adjuster" : {
      "adjuster" : "aeiou",
      "adjuster_value" : 1.3579000000000001069366817318950779736042022705078125
    },
    "image_url" : "aeiou",
    "product_id" : 123,
    "weight_adjuster" : "",
    "id" : 123,
    "purchasing_disabled" : true,
    "purchasing_disabled_message" : "aeiou",
    "conditions" : [ {
      "rule_id" : 123,
      "variant_id" : 123,
      "combination_id" : 123,
      "modifier_id" : 123,
      "modifier_value_id" : 123,
      "id" : 123
    } ],
    "sort_order" : 123,
    "enabled" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A `ComplexRule` object
   <a href="#ComplexRuleResponse">
    ComplexRuleResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `ComplexRule` was in conflict with another `ComplexRule`. This is the result of duplicate conditions.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `ComplexRule` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createModifier">
   </a>
   <h2 class_="jumptarget" id="createModifier">
    Create a `Modifier`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/modifiers
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Modifier
     <a href="#Modifier">
      Modifier
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Modifier` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ModifierResponse">
     ModifierResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "option_values" : [ "" ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    },
    "required" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A modifier object
   <a href="#ModifierResponse">
    ModifierResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Modifier` was in conflict with another option. This is the result of duplicate unique fields such as name.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Modifier` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createModifierImage">
   </a>
   <h2 class_="jumptarget" id="createModifierImage">
    Add an image to a modifier value that will show on the storefront when it’s selected
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/modifiers/{modifier_id}/values/{value_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
    <div class="param">
     modifier_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
    <div class="param">
     value_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      multipart/form-data
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Form parameters
   </h3>
   <div class="field-items">
    <div class="param">
     image_file (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Form Parameter
     </span>
     — An image file. Support MIME types include GIF, JPEG, and PNG.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ImageResponse">
     ImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A ResourceImage and meta data
   <a href="#ImageResponse">
    ImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    422
   </h4>
   Modifier image was not valid. This is the result of missing image_file fields or non-url for image_file field. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createOption">
   </a>
   <h2 class_="jumptarget" id="createOption">
    Create an `Option`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/options
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Option
     <a href="#Option">
      Option
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Option` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#OptionResponse">
     OptionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "option_values" : [ {
      "id" : 123,
      "label" : "aeiou",
      "value_data" : "{}",
      "is_default" : true,
      "sort_order" : 123
    } ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    }
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An option object
   <a href="#OptionResponse">
    OptionResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   Option was in conflict with another option. This is the result of duplicate unique fields such as name.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   Option was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createProduct">
   </a>
   <h2 class_="jumptarget" id="createProduct">
    Creates a `Product` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     product
     <a href="#ProductPost">
      ProductPost
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `Product` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductResponse">
     ProductResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "calculated_price" : 1.3579000000000001069366817318950779736042022705078125,
    "gift_wrapping_options_list" : [ 123 ],
    "page_title" : "aeiou",
    "videos" : [ {
      "product_id" : 123,
      "length" : "aeiou",
      "description" : "aeiou",
      "id" : 123,
      "title" : "aeiou",
      "sort_order" : 123
    } ],
    "is_condition_shown" : true,
    "variants" : [ {
      "image_url" : "aeiou",
      "option_values" : [ {
        "option_display_name" : "aeiou",
        "option_id" : 123,
        "id" : 123,
        "label" : "aeiou"
      } ],
      "weight" : 1.3579000000000001069366817318950779736042022705078125,
      "upc" : "aeiou",
      "bin_picking_number" : "aeiou",
      "sku_id" : 123,
      "purchasing_disabled_message" : "aeiou",
      "inventory_level" : 123,
      "price" : 1.3579000000000001069366817318950779736042022705078125,
      "inventory_warning_level" : 123,
      "product_id" : 123,
      "id" : 123,
      "purchasing_disabled" : true,
      "sku" : "aeiou",
      "cost_price" : 1.3579000000000001069366817318950779736042022705078125
    } ],
    "type" : "aeiou",
    "retail_price" : 1.3579000000000001069366817318950779736042022705078125,
    "layout_file" : "aeiou",
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "warranty" : "aeiou",
    "is_free_shipping" : true,
    "id" : 123,
    "sku" : "aeiou",
    "height" : 1.3579000000000001069366817318950779736042022705078125,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    },
    "images" : [ {
      "url_thumbnail" : "aeiou",
      "product_id" : 123,
      "description" : "aeiou",
      "image_file" : "aeiou",
      "id" : 123,
      "url_standard" : "aeiou",
      "url_zoom" : "aeiou",
      "url_tiny" : "aeiou",
      "sort_order" : 123,
      "is_thumbnail" : true
    } ],
    "custom_fields" : [ {
      "product_id" : 123,
      "name" : "aeiou",
      "id" : 123,
      "value" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "brand_id" : 123,
    "meta_description" : "aeiou",
    "condition" : "aeiou",
    "inventory_level" : 123,
    "name" : "aeiou",
    "inventory_tracking" : "aeiou",
    "preorder_release_date" : "aeiou",
    "description" : "aeiou",
    "bin_picking_number" : "aeiou",
    "availability" : "aeiou",
    "search_keywords" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "is_price_hidden" : true,
    "order_quantity_minimum" : 123,
    "availability_description" : "aeiou",
    "fixed_cost_shipping_price" : 123,
    "categories" : [ 123 ],
    "sort_order" : 123,
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125,
    "order_quantity_maximum" : 123,
    "is_visible" : true,
    "is_preorder_only" : true,
    "date_created" : "aeiou",
    "preorder_message" : "aeiou",
    "tax_class_id" : 123,
    "bulk_pricing_rules" : [ {
      "amount" : 1.3579000000000001069366817318950779736042022705078125,
      "quantity_min" : 123,
      "quantity_max" : 123,
      "id" : 123,
      "type" : "aeiou"
    } ],
    "sale_price" : 1.3579000000000001069366817318950779736042022705078125,
    "product_tax_code" : "aeiou",
    "depth" : 1.3579000000000001069366817318950779736042022705078125,
    "date_modified" : "aeiou",
    "gift_wrapping_options_type" : "aeiou",
    "width" : 1.3579000000000001069366817318950779736042022705078125,
    "price_hidden_label" : "aeiou",
    "is_featured" : true,
    "view_count" : 123
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product
   <a href="#ProductResponse">
    ProductResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   `Product` was in conflict with another product. This is the result of duplicate unique values such as name or SKU; a missing or invalid category id, brand id, or tax_class id; or a conflicting `bulk_pricing_rule`.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   `Product` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createProductImage">
   </a>
   <h2 class_="jumptarget" id="createProductImage">
    Creates an image on a product. Publically accessible URLs and files (form post) are valid parameters.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/images
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the image is being attached to.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     productImage
     <a href="#ProductImage">
      ProductImage
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `ProductImage` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductImageResponse">
     ProductImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "url_thumbnail" : "aeiou",
    "product_id" : 123,
    "description" : "aeiou",
    "image_file" : "aeiou",
    "id" : 123,
    "url_standard" : "aeiou",
    "url_zoom" : "aeiou",
    "url_tiny" : "aeiou",
    "sort_order" : 123,
    "is_thumbnail" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product image
   <a href="#ProductImageResponse">
    ProductImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="createProductMetafield">
   </a>
   <h2 class_="jumptarget" id="createProductMetafield">
    Create a product `Metafield`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A `Metafield` object
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Metafield` was in conflict with another `Metafield`. This can be the result of duplicate unique key combination of the app's client id, namespace, key, resource_type, and resource_id.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Metafield` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createProductVideo">
   </a>
   <h2 class_="jumptarget" id="createProductVideo">
    Creates an video on a product using a video ID from Youtube
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/videos
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the video is being attached to.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     productVideo
     <a href="#ProductVideo">
      ProductVideo
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `ProductVideo` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductVideoResponse">
     ProductVideoResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "length" : "aeiou",
    "description" : "aeiou",
    "id" : 123,
    "title" : "aeiou",
    "sort_order" : 123
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product video
   <a href="#ProductVideoResponse">
    ProductVideoResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="createVariant">
   </a>
   <h2 class_="jumptarget" id="createVariant">
    Create a `Variant` object.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/variants
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Variant
     <a href="#Variant">
      Variant
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Variant` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#VariantResponse">
     VariantResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou",
    "option_values" : [ {
      "option_display_name" : "aeiou",
      "option_id" : 123,
      "id" : 123,
      "label" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "bin_picking_number" : "aeiou",
    "sku_id" : 123,
    "purchasing_disabled_message" : "aeiou",
    "inventory_level" : 123,
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "product_id" : 123,
    "id" : 123,
    "purchasing_disabled" : true,
    "sku" : "aeiou",
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A variant and meta data
   <a href="#VariantResponse">
    VariantResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="createVariantImage">
   </a>
   <h2 class_="jumptarget" id="createVariantImage">
    None
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/variants/{variant_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant`.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      multipart/form-data
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Form parameters
   </h3>
   <div class="field-items">
    <div class="param">
     image_file (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Form Parameter
     </span>
     — An image file. Support MIME types include GIF, JPEG, and PNG.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ImageResponse">
     ImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A ResourceImage and meta data
   <a href="#ImageResponse">
    ImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    422
   </h4>
   Image was not valid. This is the result of missing image_file field or incorrect file type. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="createVariantMetafield">
   </a>
   <h2 class_="jumptarget" id="createVariantMetafield">
    Create a variant `Metafield`.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /catalog/products/{product_id}/variants/{variant_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A `Metafield` object
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Metafield` was in conflict with another `Metafield`. This can be the result of duplicate unique key combination of the app's client id, namespace, key, resource_type, and resource_id.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Metafield` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="deleteBrandById">
   </a>
   <h2 class_="jumptarget" id="deleteBrandById">
    Delete a `Brand` from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/brands/{brand_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` requested
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteBrandImage">
   </a>
   <h2 class_="jumptarget" id="deleteBrandImage">
    Delete a `Brand` image the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/brands/{brand_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the image is being attached to.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   Image cleared for the brand
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteBrandMetafieldById">
   </a>
   <h2 class_="jumptarget" id="deleteBrandMetafieldById">
    Delete a `Metafield`
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/brands/{brand_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteBrands">
   </a>
   <h2 class_="jumptarget" id="deleteBrands">
    Delete one or more `Brand` objects from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/brands
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by name.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by page_title.
    </div>
   </div>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteCategories">
   </a>
   <h2 class_="jumptarget" id="deleteCategories">
    Delete a product or products from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/categories
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by name.
    </div>
    <div class="param">
     parent_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by parent_id.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by page_title.
    </div>
    <div class="param">
     keyword (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by keywords.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_visible.
    </div>
   </div>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteCategoryById">
   </a>
   <h2 class_="jumptarget" id="deleteCategoryById">
    Delete one or more `Category` objects from the BigCommerce catalog.
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/categories/{category_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteCategoryImage">
   </a>
   <h2 class_="jumptarget" id="deleteCategoryImage">
    Delete a `Category` image the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/categories/{category_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteCategoryMetafieldById">
   </a>
   <h2 class_="jumptarget" id="deleteCategoryMetafieldById">
    Delete a `Metafield`
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/categories/{category_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteComplexRuleById">
   </a>
   <h2 class_="jumptarget" id="deleteComplexRuleById">
    Delete a Product's `ComplexRule` based on the product_id and complex_rule_id.
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/complex-rules/{complex_rule_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `ComplexRule` belongs to.
 format: int
    </div>
    <div class="param">
     complex_rule_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `ComplexRule`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteModifierById">
   </a>
   <h2 class_="jumptarget" id="deleteModifierById">
    Delete a Product's `Modifier` based on the product_id and modifier_id.
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/modifiers/{modifier_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
    <div class="param">
     modifier_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteModifierImage">
   </a>
   <h2 class_="jumptarget" id="deleteModifierImage">
    Delete the image applied to show when the modifier value is selected
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/modifiers/{modifier_id}/values/{value_id}/image
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
    <div class="param">
     modifier_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
    <div class="param">
     value_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   Image cleared for the modifier value
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteOptionById">
   </a>
   <h2 class_="jumptarget" id="deleteOptionById">
    Delete a Product's `Option` based on the product_id and option_id.
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/options/{option_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Option` belongs to.
 format: int
    </div>
    <div class="param">
     option_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Option`.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteProductById">
   </a>
   <h2 class_="jumptarget" id="deleteProductById">
    Deletes a `Product` object from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteProductImage">
   </a>
   <h2 class_="jumptarget" id="deleteProductImage">
    Delete a `ProductImage` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/images/{image_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the image is being attached to.
    </div>
    <div class="param">
     image_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Image` that is being operated on.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteProductMetafieldById">
   </a>
   <h2 class_="jumptarget" id="deleteProductMetafieldById">
    Delete a `Metafield`
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteProductVideo">
   </a>
   <h2 class_="jumptarget" id="deleteProductVideo">
    Delete a `ProductVideo` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/videos/{video_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the video is being attached to.
    </div>
    <div class="param">
     video_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Video` the video is being operated on.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteProducts">
   </a>
   <h2 class_="jumptarget" id="deleteProducts">
    Deletes one or more `Product` objects from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by name.
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by sku.
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by price.
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by weight.
    </div>
    <div class="param">
     condition (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by condition.
    </div>
    <div class="param">
     brand_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by brand_id.
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_modified.
 format: data-time
    </div>
    <div class="param">
     date_last_imported (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_last_imported.
 format: data-time
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_visible.
    </div>
    <div class="param">
     is_featured (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_featured.
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by inventory_level.
    </div>
    <div class="param">
     total_sold (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by total_sold.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by type: `physical` or `digital`
    </div>
    <div class="param">
     categories (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by categories.
    </div>
    <div class="param">
     keyword (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by keywords found in the name, description, sku, keywords, brand name.
    </div>
   </div>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteVariantById">
   </a>
   <h2 class_="jumptarget" id="deleteVariantById">
    Delete a `Variant`
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/variants/{variant_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteVariantMetafieldById">
   </a>
   <h2 class_="jumptarget" id="deleteVariantMetafieldById">
    Delete a `Metafield`
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /catalog/products/{product_id}/variants/{variant_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="getBrandById">
   </a>
   <h2 class_="jumptarget" id="getBrandById">
    Gets `Brand` object.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/brands/{brand_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` requested
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#BrandResponse">
     BrandResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "meta_description" : "aeiou",
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "name" : "aeiou",
    "id" : 123,
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A brand object
   <a href="#BrandResponse">
    BrandResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getBrandMetafieldByBrandId">
   </a>
   <h2 class_="jumptarget" id="getBrandMetafieldByBrandId">
    Get a `Metafield` by category_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/brands/{brand_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#Metafield">
     Metafield
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "updated_at" : "2000-01-23T04:56:07.000+00:00",
  "namespace" : "aeiou",
  "resource_type" : "aeiou",
  "description" : "aeiou",
  "resource_id" : 123,
  "created_at" : "2000-01-23T04:56:07.000+00:00",
  "id" : 123,
  "value" : "aeiou",
  "key" : "aeiou",
  "permission_set" : "aeiou"
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield object
   <a href="#Metafield">
    Metafield
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getBrandMetafieldsByBrandId">
   </a>
   <h2 class_="jumptarget" id="getBrandMetafieldsByBrandId">
    Get a `Metafield` object list by category_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/brands/{brand_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetaFieldCollectionResponse">
     MetaFieldCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of meta fields and meta data
   <a href="#MetaFieldCollectionResponse">
    MetaFieldCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getBrands">
   </a>
   <h2 class_="jumptarget" id="getBrands">
    Gets `Brand` objects.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/brands
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by name.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by page_title.
    </div>
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#BrandCollectionResponse">
     BrandCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "meta_description" : "aeiou",
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "name" : "aeiou",
    "id" : 123,
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of brand objects and meta
   <a href="#BrandCollectionResponse">
    BrandCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getCategories">
   </a>
   <h2 class_="jumptarget" id="getCategories">
    Returns a paginated categories collection from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/categories
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by name.
    </div>
    <div class="param">
     parent_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by parent_id.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by page_title.
    </div>
    <div class="param">
     keyword (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by keywords.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_visible.
    </div>
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#CategoryCollectionResponse">
     CategoryCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "is_visible" : true,
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "description" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou",
    "default_product_sort" : "aeiou",
    "meta_description" : "aeiou",
    "layout_file" : "aeiou",
    "parent_id" : 123,
    "name" : "aeiou",
    "id" : 123,
    "sort_order" : 123,
    "views" : 123,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    }
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array category objects and meta data
   <a href="#CategoryCollectionResponse">
    CategoryCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getCategoryById">
   </a>
   <h2 class_="jumptarget" id="getCategoryById">
    Returns a `Category` from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/categories/{category_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#CategoryResponse">
     CategoryResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "is_visible" : true,
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "description" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou",
    "default_product_sort" : "aeiou",
    "meta_description" : "aeiou",
    "layout_file" : "aeiou",
    "parent_id" : 123,
    "name" : "aeiou",
    "id" : 123,
    "sort_order" : 123,
    "views" : 123,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    }
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A category object
   <a href="#CategoryResponse">
    CategoryResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getCategoryMetafieldByCategoryId">
   </a>
   <h2 class_="jumptarget" id="getCategoryMetafieldByCategoryId">
    Get a `Metafield` by category_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/categories/{category_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#Metafield">
     Metafield
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "updated_at" : "2000-01-23T04:56:07.000+00:00",
  "namespace" : "aeiou",
  "resource_type" : "aeiou",
  "description" : "aeiou",
  "resource_id" : 123,
  "created_at" : "2000-01-23T04:56:07.000+00:00",
  "id" : 123,
  "value" : "aeiou",
  "key" : "aeiou",
  "permission_set" : "aeiou"
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield object
   <a href="#Metafield">
    Metafield
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getCategoryMetafieldsByCategoryId">
   </a>
   <h2 class_="jumptarget" id="getCategoryMetafieldsByCategoryId">
    Get a `Metafield` object list by category_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/categories/{category_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetaFieldCollectionResponse">
     MetaFieldCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of meta fields and meta data
   <a href="#MetaFieldCollectionResponse">
    MetaFieldCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getCategoryTree">
   </a>
   <h2 class_="jumptarget" id="getCategoryTree">
    Returns the categories tree, a nested lineage of the categories with parent-&gt;child relationship. The `Category` objects returned are a simplified version of the category objects returned in the rest of this API.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/categories/tree
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#CategoryTreeCollectionResponse">
     CategoryTreeCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "is_visible" : true,
    "children" : [ "" ],
    "parent_id" : 123,
    "name" : "aeiou",
    "id" : 123,
    "url" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A array of nested category tree objects and meta data
   <a href="#CategoryTreeCollectionResponse">
    CategoryTreeCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getComplexRuleById">
   </a>
   <h2 class_="jumptarget" id="getComplexRuleById">
    Get a `ComplexRule` by product_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/complex-rules/{complex_rule_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `ComplexRule` belongs to.
 format: int
    </div>
    <div class="param">
     complex_rule_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `ComplexRule`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ComplexRuleResponse">
     ComplexRuleResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "purchasing_hidden" : true,
    "stop" : true,
    "price_adjuster" : {
      "adjuster" : "aeiou",
      "adjuster_value" : 1.3579000000000001069366817318950779736042022705078125
    },
    "image_url" : "aeiou",
    "product_id" : 123,
    "weight_adjuster" : "",
    "id" : 123,
    "purchasing_disabled" : true,
    "purchasing_disabled_message" : "aeiou",
    "conditions" : [ {
      "rule_id" : 123,
      "variant_id" : 123,
      "combination_id" : 123,
      "modifier_id" : 123,
      "modifier_value_id" : 123,
      "id" : 123
    } ],
    "sort_order" : 123,
    "enabled" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A modifier object
   <a href="#ComplexRuleResponse">
    ComplexRuleResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getComplexRules">
   </a>
   <h2 class_="jumptarget" id="getComplexRules">
    Get an array of `ComplexRule` objects.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/complex-rules
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `ComplexRule` belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ComplexRuleCollectionResponse">
     ComplexRuleCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "purchasing_hidden" : true,
    "stop" : true,
    "price_adjuster" : {
      "adjuster" : "aeiou",
      "adjuster_value" : 1.3579000000000001069366817318950779736042022705078125
    },
    "image_url" : "aeiou",
    "product_id" : 123,
    "weight_adjuster" : "",
    "id" : 123,
    "purchasing_disabled" : true,
    "purchasing_disabled_message" : "aeiou",
    "conditions" : [ {
      "rule_id" : 123,
      "variant_id" : 123,
      "combination_id" : 123,
      "modifier_id" : 123,
      "modifier_value_id" : 123,
      "id" : 123
    } ],
    "sort_order" : 123,
    "enabled" : true
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of `ComplexRule` objects and meta data
   <a href="#ComplexRuleCollectionResponse">
    ComplexRuleCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getModifierById">
   </a>
   <h2 class_="jumptarget" id="getModifierById">
    Get a `Modifier` by product_id and modifier_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/modifiers/{modifier_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
    <div class="param">
     modifier_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ModifierResponse">
     ModifierResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "option_values" : [ "" ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    },
    "required" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A modifier object
   <a href="#ModifierResponse">
    ModifierResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getModifiers">
   </a>
   <h2 class_="jumptarget" id="getModifiers">
    Get an array of `Modifier` objects.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/modifiers
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ModifierCollectionResponse">
     ModifierCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "product_id" : 123,
    "option_values" : [ "" ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    },
    "required" : true
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of modifiers and meta data
   <a href="#ModifierCollectionResponse">
    ModifierCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getOptionById">
   </a>
   <h2 class_="jumptarget" id="getOptionById">
    Gets `Option` object by product id and option id.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/options/{option_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Option` belongs to.
 format: int
    </div>
    <div class="param">
     option_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Option`.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#OptionResponse">
     OptionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "option_values" : [ {
      "id" : 123,
      "label" : "aeiou",
      "value_data" : "{}",
      "is_default" : true,
      "sort_order" : 123
    } ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    }
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A Option object
   <a href="#OptionResponse">
    OptionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getOptions">
   </a>
   <h2 class_="jumptarget" id="getOptions">
    Get an array of `Option` objects.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/options
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#OptionCollectionResponse">
     OptionCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "product_id" : 123,
    "option_values" : [ {
      "id" : 123,
      "label" : "aeiou",
      "value_data" : "{}",
      "is_default" : true,
      "sort_order" : 123
    } ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    }
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of options and meta data
   <a href="#OptionCollectionResponse">
    OptionCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getProductById">
   </a>
   <h2 class_="jumptarget" id="getProductById">
    Returns a `Product` from the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     include (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Include sub-resources on a product with a comma separated list. Valid expansions currently include `variants`, `images`, `custom_fields`, and `bulk_pricing_rules`.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductResponse">
     ProductResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "calculated_price" : 1.3579000000000001069366817318950779736042022705078125,
    "gift_wrapping_options_list" : [ 123 ],
    "page_title" : "aeiou",
    "videos" : [ {
      "product_id" : 123,
      "length" : "aeiou",
      "description" : "aeiou",
      "id" : 123,
      "title" : "aeiou",
      "sort_order" : 123
    } ],
    "is_condition_shown" : true,
    "variants" : [ {
      "image_url" : "aeiou",
      "option_values" : [ {
        "option_display_name" : "aeiou",
        "option_id" : 123,
        "id" : 123,
        "label" : "aeiou"
      } ],
      "weight" : 1.3579000000000001069366817318950779736042022705078125,
      "upc" : "aeiou",
      "bin_picking_number" : "aeiou",
      "sku_id" : 123,
      "purchasing_disabled_message" : "aeiou",
      "inventory_level" : 123,
      "price" : 1.3579000000000001069366817318950779736042022705078125,
      "inventory_warning_level" : 123,
      "product_id" : 123,
      "id" : 123,
      "purchasing_disabled" : true,
      "sku" : "aeiou",
      "cost_price" : 1.3579000000000001069366817318950779736042022705078125
    } ],
    "type" : "aeiou",
    "retail_price" : 1.3579000000000001069366817318950779736042022705078125,
    "layout_file" : "aeiou",
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "warranty" : "aeiou",
    "is_free_shipping" : true,
    "id" : 123,
    "sku" : "aeiou",
    "height" : 1.3579000000000001069366817318950779736042022705078125,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    },
    "images" : [ {
      "url_thumbnail" : "aeiou",
      "product_id" : 123,
      "description" : "aeiou",
      "image_file" : "aeiou",
      "id" : 123,
      "url_standard" : "aeiou",
      "url_zoom" : "aeiou",
      "url_tiny" : "aeiou",
      "sort_order" : 123,
      "is_thumbnail" : true
    } ],
    "custom_fields" : [ {
      "product_id" : 123,
      "name" : "aeiou",
      "id" : 123,
      "value" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "brand_id" : 123,
    "meta_description" : "aeiou",
    "condition" : "aeiou",
    "inventory_level" : 123,
    "name" : "aeiou",
    "inventory_tracking" : "aeiou",
    "preorder_release_date" : "aeiou",
    "description" : "aeiou",
    "bin_picking_number" : "aeiou",
    "availability" : "aeiou",
    "search_keywords" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "is_price_hidden" : true,
    "order_quantity_minimum" : 123,
    "availability_description" : "aeiou",
    "fixed_cost_shipping_price" : 123,
    "categories" : [ 123 ],
    "sort_order" : 123,
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125,
    "order_quantity_maximum" : 123,
    "is_visible" : true,
    "is_preorder_only" : true,
    "date_created" : "aeiou",
    "preorder_message" : "aeiou",
    "tax_class_id" : 123,
    "bulk_pricing_rules" : [ {
      "amount" : 1.3579000000000001069366817318950779736042022705078125,
      "quantity_min" : 123,
      "quantity_max" : 123,
      "id" : 123,
      "type" : "aeiou"
    } ],
    "sale_price" : 1.3579000000000001069366817318950779736042022705078125,
    "product_tax_code" : "aeiou",
    "depth" : 1.3579000000000001069366817318950779736042022705078125,
    "date_modified" : "aeiou",
    "gift_wrapping_options_type" : "aeiou",
    "width" : 1.3579000000000001069366817318950779736042022705078125,
    "price_hidden_label" : "aeiou",
    "is_featured" : true,
    "view_count" : 123
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product
   <a href="#ProductResponse">
    ProductResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getProductImageById">
   </a>
   <h2 class_="jumptarget" id="getProductImageById">
    Gets image on a product.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/images/{image_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the image is being attached to.
    </div>
    <div class="param">
     image_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Image` that is being operated on.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductImageResponse">
     ProductImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "url_thumbnail" : "aeiou",
    "product_id" : 123,
    "description" : "aeiou",
    "image_file" : "aeiou",
    "id" : 123,
    "url_standard" : "aeiou",
    "url_zoom" : "aeiou",
    "url_tiny" : "aeiou",
    "sort_order" : 123,
    "is_thumbnail" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of product images and meta data
   <a href="#ProductImageResponse">
    ProductImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getProductImages">
   </a>
   <h2 class_="jumptarget" id="getProductImages">
    Gets all images on a product.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/images
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the image is being attached to.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductImageCollectionResponse">
     ProductImageCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "url_thumbnail" : "aeiou",
    "product_id" : 123,
    "description" : "aeiou",
    "image_file" : "aeiou",
    "id" : 123,
    "url_standard" : "aeiou",
    "url_zoom" : "aeiou",
    "url_tiny" : "aeiou",
    "sort_order" : 123,
    "is_thumbnail" : true
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   List of product images and meta
   <a href="#ProductImageCollectionResponse">
    ProductImageCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getProductMetafieldByProductId">
   </a>
   <h2 class_="jumptarget" id="getProductMetafieldByProductId">
    Get a `Metafield` by product_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#Metafield">
     Metafield
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "updated_at" : "2000-01-23T04:56:07.000+00:00",
  "namespace" : "aeiou",
  "resource_type" : "aeiou",
  "description" : "aeiou",
  "resource_id" : 123,
  "created_at" : "2000-01-23T04:56:07.000+00:00",
  "id" : 123,
  "value" : "aeiou",
  "key" : "aeiou",
  "permission_set" : "aeiou"
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield object
   <a href="#Metafield">
    Metafield
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getProductMetafieldsByProductId">
   </a>
   <h2 class_="jumptarget" id="getProductMetafieldsByProductId">
    Get a `Metafield` object list by product_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetaFieldCollectionResponse">
     MetaFieldCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of metafields and meta data
   <a href="#MetaFieldCollectionResponse">
    MetaFieldCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getProductVideoById">
   </a>
   <h2 class_="jumptarget" id="getProductVideoById">
    Gets video on a product.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/videos/{video_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the video is being attached to.
    </div>
    <div class="param">
     video_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Video` the video is being operated on.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductVideoResponse">
     ProductVideoResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "length" : "aeiou",
    "description" : "aeiou",
    "id" : 123,
    "title" : "aeiou",
    "sort_order" : 123
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of product videos and meta data
   <a href="#ProductVideoResponse">
    ProductVideoResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getProductVideos">
   </a>
   <h2 class_="jumptarget" id="getProductVideos">
    Gets all videos on a product.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/videos
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the video is being attached to.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductVideoCollectionResponse">
     ProductVideoCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "product_id" : 123,
    "length" : "aeiou",
    "description" : "aeiou",
    "id" : 123,
    "title" : "aeiou",
    "sort_order" : 123
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   List of product videos and meta
   <a href="#ProductVideoCollectionResponse">
    ProductVideoCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getProducts">
   </a>
   <h2 class_="jumptarget" id="getProducts">
    Returns a paginated collection of `Products` objects from the BigCommerce Catalog.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by id.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by name.
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by sku.
    </div>
    <div class="param">
     upc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by upc.
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by price.
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by weight.
    </div>
    <div class="param">
     condition (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by condition.
    </div>
    <div class="param">
     brand_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by brand_id.
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_modified.
 format: data-time
    </div>
    <div class="param">
     date_last_imported (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_last_imported.
 format: data-time
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_visible.
    </div>
    <div class="param">
     is_featured (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_featured.
    </div>
    <div class="param">
     is_free_shipping (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by is_free_shipping.
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by inventory_level.
    </div>
    <div class="param">
     inventory_low (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by inventory_low, values: 1, 0.
    </div>
    <div class="param">
     out_of_stock (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by out_of_stock, to enable the filter, pass out_of_stock=1.
    </div>
    <div class="param">
     total_sold (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by total_sold.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by type: `physical` or `digital`
    </div>
    <div class="param">
     categories (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by categories.
    </div>
    <div class="param">
     keyword (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by keywords found in the name, description, sku, keywords, brand name.
    </div>
    <div class="param">
     keyword_context (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Set context for a product search.
    </div>
    <div class="param">
     include (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Include sub-resources on a product with a comma separated list. Valid expansions currently include `variants`, `images`, `custom_fields`, and `bulk_pricing_rules`.
    </div>
    <div class="param">
     availability (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by availability, values: available, disabled, preorder.
    </div>
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
    <div class="param">
     direction (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Sort direction. Values: asc, desc.
    </div>
    <div class="param">
     sort (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Field name to sort by.
Values: id, name, sku, price, date_modified, date_last_imported, inventory_level, is_visible.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductCollectionResponse">
     ProductCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "calculated_price" : 1.3579000000000001069366817318950779736042022705078125,
    "gift_wrapping_options_list" : [ 123 ],
    "page_title" : "aeiou",
    "videos" : [ {
      "product_id" : 123,
      "length" : "aeiou",
      "description" : "aeiou",
      "id" : 123,
      "title" : "aeiou",
      "sort_order" : 123
    } ],
    "is_condition_shown" : true,
    "variants" : [ {
      "image_url" : "aeiou",
      "option_values" : [ {
        "option_display_name" : "aeiou",
        "option_id" : 123,
        "id" : 123,
        "label" : "aeiou"
      } ],
      "weight" : 1.3579000000000001069366817318950779736042022705078125,
      "upc" : "aeiou",
      "bin_picking_number" : "aeiou",
      "sku_id" : 123,
      "purchasing_disabled_message" : "aeiou",
      "inventory_level" : 123,
      "price" : 1.3579000000000001069366817318950779736042022705078125,
      "inventory_warning_level" : 123,
      "product_id" : 123,
      "id" : 123,
      "purchasing_disabled" : true,
      "sku" : "aeiou",
      "cost_price" : 1.3579000000000001069366817318950779736042022705078125
    } ],
    "type" : "aeiou",
    "retail_price" : 1.3579000000000001069366817318950779736042022705078125,
    "layout_file" : "aeiou",
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "warranty" : "aeiou",
    "is_free_shipping" : true,
    "id" : 123,
    "sku" : "aeiou",
    "height" : 1.3579000000000001069366817318950779736042022705078125,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    },
    "images" : [ {
      "url_thumbnail" : "aeiou",
      "product_id" : 123,
      "description" : "aeiou",
      "image_file" : "aeiou",
      "id" : 123,
      "url_standard" : "aeiou",
      "url_zoom" : "aeiou",
      "url_tiny" : "aeiou",
      "sort_order" : 123,
      "is_thumbnail" : true
    } ],
    "custom_fields" : [ {
      "product_id" : 123,
      "name" : "aeiou",
      "id" : 123,
      "value" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "brand_id" : 123,
    "meta_description" : "aeiou",
    "condition" : "aeiou",
    "inventory_level" : 123,
    "name" : "aeiou",
    "inventory_tracking" : "aeiou",
    "preorder_release_date" : "aeiou",
    "description" : "aeiou",
    "bin_picking_number" : "aeiou",
    "availability" : "aeiou",
    "search_keywords" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "is_price_hidden" : true,
    "order_quantity_minimum" : 123,
    "availability_description" : "aeiou",
    "fixed_cost_shipping_price" : 123,
    "categories" : [ 123 ],
    "sort_order" : 123,
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125,
    "order_quantity_maximum" : 123,
    "is_visible" : true,
    "is_preorder_only" : true,
    "date_created" : "aeiou",
    "preorder_message" : "aeiou",
    "tax_class_id" : 123,
    "bulk_pricing_rules" : [ {
      "amount" : 1.3579000000000001069366817318950779736042022705078125,
      "quantity_min" : 123,
      "quantity_max" : 123,
      "id" : 123,
      "type" : "aeiou"
    } ],
    "sale_price" : 1.3579000000000001069366817318950779736042022705078125,
    "product_tax_code" : "aeiou",
    "depth" : 1.3579000000000001069366817318950779736042022705078125,
    "date_modified" : "aeiou",
    "gift_wrapping_options_type" : "aeiou",
    "width" : 1.3579000000000001069366817318950779736042022705078125,
    "price_hidden_label" : "aeiou",
    "is_featured" : true,
    "view_count" : 123
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of products and meta data
   <a href="#ProductCollectionResponse">
    ProductCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="getVariantById">
   </a>
   <h2 class_="jumptarget" id="getVariantById">
    Get a `Variant` object.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/variants/{variant_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#VariantResponse">
     VariantResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou",
    "option_values" : [ {
      "option_display_name" : "aeiou",
      "option_id" : 123,
      "id" : 123,
      "label" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "bin_picking_number" : "aeiou",
    "sku_id" : 123,
    "purchasing_disabled_message" : "aeiou",
    "inventory_level" : 123,
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "product_id" : 123,
    "id" : 123,
    "purchasing_disabled" : true,
    "sku" : "aeiou",
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A variant and meta data
   <a href="#VariantResponse">
    VariantResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getVariantMetafieldByProductIdAndVariantId">
   </a>
   <h2 class_="jumptarget" id="getVariantMetafieldByProductIdAndVariantId">
    Get a `Metafield` by product_id and variant_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/variants/{variant_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#Metafield">
     Metafield
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "updated_at" : "2000-01-23T04:56:07.000+00:00",
  "namespace" : "aeiou",
  "resource_type" : "aeiou",
  "description" : "aeiou",
  "resource_id" : 123,
  "created_at" : "2000-01-23T04:56:07.000+00:00",
  "id" : 123,
  "value" : "aeiou",
  "key" : "aeiou",
  "permission_set" : "aeiou"
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield object
   <a href="#Metafield">
    Metafield
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getVariantMetafieldsByProductIdAndVariantId">
   </a>
   <h2 class_="jumptarget" id="getVariantMetafieldsByProductIdAndVariantId">
    Get a `Metafield` object list by product_id and variant_id
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/variants/{variant_id}/metafields
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter based on a metafield's key
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetaFieldCollectionResponse">
     MetaFieldCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of meta fields and meta data
   <a href="#MetaFieldCollectionResponse">
    MetaFieldCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getVariants">
   </a>
   <h2 class_="jumptarget" id="getVariants">
    Returns a `Variant` object list from the BigCommerce Catalog.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/variants
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by id.
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by sku.
    </div>
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#VariantCollectionResponse">
     VariantCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "image_url" : "aeiou",
    "option_values" : [ {
      "option_display_name" : "aeiou",
      "option_id" : 123,
      "id" : 123,
      "label" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "bin_picking_number" : "aeiou",
    "sku_id" : 123,
    "purchasing_disabled_message" : "aeiou",
    "inventory_level" : 123,
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "product_id" : 123,
    "id" : 123,
    "purchasing_disabled" : true,
    "sku" : "aeiou",
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of variants and meta data
   <a href="#VariantCollectionResponse">
    VariantCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getVariantsByProductId">
   </a>
   <h2 class_="jumptarget" id="getVariantsByProductId">
    Returns a `Variant` object list from the BigCommerce Catalog.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /catalog/products/{product_id}/variants
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#VariantCollectionResponse">
     VariantCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "image_url" : "aeiou",
    "option_values" : [ {
      "option_display_name" : "aeiou",
      "option_id" : 123,
      "id" : 123,
      "label" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "bin_picking_number" : "aeiou",
    "sku_id" : 123,
    "purchasing_disabled_message" : "aeiou",
    "inventory_level" : 123,
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "product_id" : 123,
    "id" : 123,
    "purchasing_disabled" : true,
    "sku" : "aeiou",
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of variants and meta data
   <a href="#VariantCollectionResponse">
    VariantCollectionResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateBrand">
   </a>
   <h2 class_="jumptarget" id="updateBrand">
    Update a `Brand` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/brands/{brand_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` requested
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     brand
     <a href="#Brand">
      Brand
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — Returns a `Brand` from the BigCommerce Catalog
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#BrandResponse">
     BrandResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "meta_description" : "aeiou",
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "name" : "aeiou",
    "id" : 123,
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A brand object
   <a href="#BrandResponse">
    BrandResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Brand` was in conflict with another product. This is the result of duplicate unique value such as name
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Brand` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="updateBrandMetafield">
   </a>
   <h2 class_="jumptarget" id="updateBrandMetafield">
    Update a `Metafield` object.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/brands/{brand_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     brand_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Brand` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield and meta data
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateCategory">
   </a>
   <h2 class_="jumptarget" id="updateCategory">
    Update a `Category` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/categories/{category_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     category
     <a href="#Category">
      Category
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `Category` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#CategoryResponse">
     CategoryResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "is_visible" : true,
    "page_title" : "aeiou",
    "image_url" : "aeiou",
    "description" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "search_keywords" : "aeiou",
    "default_product_sort" : "aeiou",
    "meta_description" : "aeiou",
    "layout_file" : "aeiou",
    "parent_id" : 123,
    "name" : "aeiou",
    "id" : 123,
    "sort_order" : 123,
    "views" : 123,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    }
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A category object
   <a href="#CategoryResponse">
    CategoryResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Category` was in conflict with another category. This is the result of duplicate unique values such as name or custom_url.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Category` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="updateCategoryMetafield">
   </a>
   <h2 class_="jumptarget" id="updateCategoryMetafield">
    Update a `Metafield` object.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/categories/{category_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     category_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Category` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield and meta data
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateComplexRule">
   </a>
   <h2 class_="jumptarget" id="updateComplexRule">
    Update an Product's `ComplexRule` based on the product_id and complex_rule_id.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/complex-rules/{complex_rule_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `ComplexRule` belongs to.
 format: int
    </div>
    <div class="param">
     complex_rule_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `ComplexRule`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ComplexRuleResponse">
     ComplexRuleResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "purchasing_hidden" : true,
    "stop" : true,
    "price_adjuster" : {
      "adjuster" : "aeiou",
      "adjuster_value" : 1.3579000000000001069366817318950779736042022705078125
    },
    "image_url" : "aeiou",
    "product_id" : 123,
    "weight_adjuster" : "",
    "id" : 123,
    "purchasing_disabled" : true,
    "purchasing_disabled_message" : "aeiou",
    "conditions" : [ {
      "rule_id" : 123,
      "variant_id" : 123,
      "combination_id" : 123,
      "modifier_id" : 123,
      "modifier_value_id" : 123,
      "id" : 123
    } ],
    "sort_order" : 123,
    "enabled" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A `ComplexRule` object
   <a href="#ComplexRuleResponse">
    ComplexRuleResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `ComplexRule` was in conflict with another `ComplexRule`. This is the result of duplicate conditions.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `ComplexRule` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="updateModifier">
   </a>
   <h2 class_="jumptarget" id="updateModifier">
    Update an Product's `Modifier` based on the product_id and modifier_id.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/modifiers/{modifier_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Modifier` belongs to.
 format: int
    </div>
    <div class="param">
     modifier_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Modifier`
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     modifier
     <a href="#Modifier">
      Modifier
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `Modifier` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ModifierResponse">
     ModifierResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "option_values" : [ "" ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    },
    "required" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A modifier object
   <a href="#ModifierResponse">
    ModifierResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Modifier` was in conflict with another modifier or option. This is the result of duplicate unique fields such as name.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Modifier` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="updateOption">
   </a>
   <h2 class_="jumptarget" id="updateOption">
    Update a Product's `Option` based on the product_id and option_id.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/options/{option_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the `Option` belongs to.
 format: int
    </div>
    <div class="param">
     option_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Option`.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     option
     <a href="#Option">
      Option
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `Option` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#OptionResponse">
     OptionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "option_values" : [ {
      "id" : 123,
      "label" : "aeiou",
      "value_data" : "{}",
      "is_default" : true,
      "sort_order" : 123
    } ],
    "name" : "aeiou",
    "id" : 123,
    "display_name" : "aeiou",
    "type" : "aeiou",
    "config" : {
      "text_max_length" : 123,
      "file_types_other" : [ "aeiou" ],
      "file_max_size" : 123,
      "file_types_supported" : [ "aeiou" ],
      "text_characters_limited" : true,
      "product_list_adjusts_inventory" : true,
      "number_limited" : true,
      "checked_by_default" : true,
      "date_latest_value" : "2000-01-23",
      "product_list_adjusts_pricing" : true,
      "default_value" : "aeiou",
      "date_limited" : true,
      "text_max_lines" : 123,
      "checkbox_label" : "aeiou",
      "text_min_length" : 123,
      "file_types_mode" : "aeiou",
      "text_lines_limited" : true,
      "number_highest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "date_earliest_value" : "2000-01-23",
      "date_limit_mode" : "aeiou",
      "number_lowest_value" : 1.3579000000000001069366817318950779736042022705078125,
      "number_integers_only" : true,
      "product_list_shipping_calc" : "aeiou",
      "number_limit_mode" : "aeiou"
    }
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An option object
   <a href="#OptionResponse">
    OptionResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Option` was in conflict with another option. This is the result of duplicate unique fields such as name.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Option` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="updateProduct">
   </a>
   <h2 class_="jumptarget" id="updateProduct">
    Updates a `Product` in the BigCommerce Catalog
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     product
     <a href="#ProductPut">
      ProductPut
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `Product` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductResponse">
     ProductResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "calculated_price" : 1.3579000000000001069366817318950779736042022705078125,
    "gift_wrapping_options_list" : [ 123 ],
    "page_title" : "aeiou",
    "videos" : [ {
      "product_id" : 123,
      "length" : "aeiou",
      "description" : "aeiou",
      "id" : 123,
      "title" : "aeiou",
      "sort_order" : 123
    } ],
    "is_condition_shown" : true,
    "variants" : [ {
      "image_url" : "aeiou",
      "option_values" : [ {
        "option_display_name" : "aeiou",
        "option_id" : 123,
        "id" : 123,
        "label" : "aeiou"
      } ],
      "weight" : 1.3579000000000001069366817318950779736042022705078125,
      "upc" : "aeiou",
      "bin_picking_number" : "aeiou",
      "sku_id" : 123,
      "purchasing_disabled_message" : "aeiou",
      "inventory_level" : 123,
      "price" : 1.3579000000000001069366817318950779736042022705078125,
      "inventory_warning_level" : 123,
      "product_id" : 123,
      "id" : 123,
      "purchasing_disabled" : true,
      "sku" : "aeiou",
      "cost_price" : 1.3579000000000001069366817318950779736042022705078125
    } ],
    "type" : "aeiou",
    "retail_price" : 1.3579000000000001069366817318950779736042022705078125,
    "layout_file" : "aeiou",
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "warranty" : "aeiou",
    "is_free_shipping" : true,
    "id" : 123,
    "sku" : "aeiou",
    "height" : 1.3579000000000001069366817318950779736042022705078125,
    "custom_url" : {
      "is_customized" : true,
      "url" : "aeiou"
    },
    "images" : [ {
      "url_thumbnail" : "aeiou",
      "product_id" : 123,
      "description" : "aeiou",
      "image_file" : "aeiou",
      "id" : 123,
      "url_standard" : "aeiou",
      "url_zoom" : "aeiou",
      "url_tiny" : "aeiou",
      "sort_order" : 123,
      "is_thumbnail" : true
    } ],
    "custom_fields" : [ {
      "product_id" : 123,
      "name" : "aeiou",
      "id" : 123,
      "value" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "brand_id" : 123,
    "meta_description" : "aeiou",
    "condition" : "aeiou",
    "inventory_level" : 123,
    "name" : "aeiou",
    "inventory_tracking" : "aeiou",
    "preorder_release_date" : "aeiou",
    "description" : "aeiou",
    "bin_picking_number" : "aeiou",
    "availability" : "aeiou",
    "search_keywords" : "aeiou",
    "meta_keywords" : [ "aeiou" ],
    "is_price_hidden" : true,
    "order_quantity_minimum" : 123,
    "availability_description" : "aeiou",
    "fixed_cost_shipping_price" : 123,
    "categories" : [ 123 ],
    "sort_order" : 123,
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125,
    "order_quantity_maximum" : 123,
    "is_visible" : true,
    "is_preorder_only" : true,
    "date_created" : "aeiou",
    "preorder_message" : "aeiou",
    "tax_class_id" : 123,
    "bulk_pricing_rules" : [ {
      "amount" : 1.3579000000000001069366817318950779736042022705078125,
      "quantity_min" : 123,
      "quantity_max" : 123,
      "id" : 123,
      "type" : "aeiou"
    } ],
    "sale_price" : 1.3579000000000001069366817318950779736042022705078125,
    "product_tax_code" : "aeiou",
    "depth" : 1.3579000000000001069366817318950779736042022705078125,
    "date_modified" : "aeiou",
    "gift_wrapping_options_type" : "aeiou",
    "width" : 1.3579000000000001069366817318950779736042022705078125,
    "price_hidden_label" : "aeiou",
    "is_featured" : true,
    "view_count" : 123
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product
   <a href="#ProductResponse">
    ProductResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    409
   </h4>
   `Product` was in conflict with another product. This is the result of duplicate unique values such as name or SKU, a missing category, brand, or tax_class that the product is being associate to, or a conflicting bulk pricing rule.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   `Product` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="updateProductImage">
   </a>
   <h2 class_="jumptarget" id="updateProductImage">
    Updates an image on a product. Publically accessible URLs and files (form post) are valid parameters.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/images/{image_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the image is being attached to.
    </div>
    <div class="param">
     image_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Image` that is being operated on.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     productImage
     <a href="#ProductImage">
      ProductImage
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `ProductImage` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductImageResponse">
     ProductImageResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "url_thumbnail" : "aeiou",
    "product_id" : 123,
    "description" : "aeiou",
    "image_file" : "aeiou",
    "id" : 123,
    "url_standard" : "aeiou",
    "url_zoom" : "aeiou",
    "url_tiny" : "aeiou",
    "sort_order" : 123,
    "is_thumbnail" : true
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product image
   <a href="#ProductImageResponse">
    ProductImageResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateProductMetafield">
   </a>
   <h2 class_="jumptarget" id="updateProductMetafield">
    Update a `Metafield` object.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield and meta data
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateProductVideo">
   </a>
   <h2 class_="jumptarget" id="updateProductVideo">
    Updates an video on a product.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/videos/{video_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the video is being attached to.
    </div>
    <div class="param">
     video_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Video` the video is being operated on.
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     productVideo
     <a href="#ProductVideo">
      ProductVideo
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — A BigCommerce `ProductVideo` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#ProductVideoResponse">
     ProductVideoResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "product_id" : 123,
    "length" : "aeiou",
    "description" : "aeiou",
    "id" : 123,
    "title" : "aeiou",
    "sort_order" : 123
  },
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A product video
   <a href="#ProductVideoResponse">
    ProductVideoResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateVariant">
   </a>
   <h2 class_="jumptarget" id="updateVariant">
    Update a `Variant` object.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/variants/{variant_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Variant
     <a href="#Variant">
      Variant
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Variant` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#VariantResponse">
     VariantResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "image_url" : "aeiou",
    "option_values" : [ {
      "option_display_name" : "aeiou",
      "option_id" : 123,
      "id" : 123,
      "label" : "aeiou"
    } ],
    "weight" : 1.3579000000000001069366817318950779736042022705078125,
    "upc" : "aeiou",
    "bin_picking_number" : "aeiou",
    "sku_id" : 123,
    "purchasing_disabled_message" : "aeiou",
    "inventory_level" : 123,
    "price" : 1.3579000000000001069366817318950779736042022705078125,
    "inventory_warning_level" : 123,
    "product_id" : 123,
    "id" : 123,
    "purchasing_disabled" : true,
    "sku" : "aeiou",
    "cost_price" : 1.3579000000000001069366817318950779736042022705078125
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A variant and meta data
   <a href="#VariantResponse">
    VariantResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="updateVariantMetafield">
   </a>
   <h2 class_="jumptarget" id="updateVariantMetafield">
    Update a `Metafield` object.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /catalog/products/{product_id}/variants/{variant_id}/metafields/{metafield_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     metafield_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Metafield`.
 format: int
    </div>
    <div class="param">
     product_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Product` the resource belongs to.
 format: int
    </div>
    <div class="param">
     variant_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Variant` the resource belongs to.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     Metafield
     <a href="#Metafield">
      Metafield
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Metafield` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#MetafieldResponse">
     MetafieldResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "updated_at" : "2000-01-23T04:56:07.000+00:00",
    "namespace" : "aeiou",
    "resource_type" : "aeiou",
    "description" : "aeiou",
    "resource_id" : 123,
    "created_at" : "2000-01-23T04:56:07.000+00:00",
    "id" : 123,
    "value" : "aeiou",
    "key" : "aeiou",
    "permission_set" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A metafield and meta data
   <a href="#MetafieldResponse">
    MetafieldResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <hr/>
  <h1>
   <a name="Customers">
    Customers
   </a>
  </h1>
  <div class="method">
   <a name="createSubscriber">
   </a>
   <h2 class_="jumptarget" id="createSubscriber">
    Creates a `Subscriber` object.
   </h2>
   <div class_="method-path">
    <span class_="post">
     <span class_="http-method">
      POST
     </span>
     /customers/subscribers
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     subscriber
     <a href="#Subscriber">
      Subscriber
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — `Subscriber` object
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#SubscriberResponse">
     SubscriberResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "date_modified" : "aeiou",
    "date_created" : "aeiou",
    "last_name" : "aeiou",
    "id" : 123,
    "source" : "aeiou",
    "first_name" : "aeiou",
    "order_id" : 123,
    "email" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A Subscriber object
   <a href="#SubscriberResponse">
    SubscriberResponse
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Subscriber` was in conflict with another subscriber. This is the result of duplicate unique values such as email
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Subscriber` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <div class="method">
   <a name="deleteSubscriberById">
   </a>
   <h2 class_="jumptarget" id="deleteSubscriberById">
    Delete a `Subscriber` object.
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /customers/subscribers/{subscriber_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     subscriber_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Subscriber` requested.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="deleteSubscribers">
   </a>
   <h2 class_="jumptarget" id="deleteSubscribers">
    Delete a subscriber or subscribers from BigCommerce Customers.
   </h2>
   <div class_="method-path">
    <span class_="delete">
     <span class_="http-method">
      DELETE
     </span>
     /customers/subscribers
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     email (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by email.
    </div>
    <div class="param">
     first_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by first_name.
    </div>
    <div class="param">
     last_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by last_name.
    </div>
    <div class="param">
     source (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by source.
    </div>
    <div class="param">
     order_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by order_id.
    </div>
    <div class="param">
     date_created (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_created.
 format: data-time
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_modified.
 format: data-time
    </div>
   </div>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    204
   </h4>
   An empty response
   <a href="#">
   </a>
  </div>
  <div class="method">
   <a name="getSubscriberById">
   </a>
   <h2 class_="jumptarget" id="getSubscriberById">
    Gets `Subscriber` object.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /customers/subscribers/{subscriber_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     subscriber_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Subscriber` requested.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#SubscriberResponse">
     SubscriberResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "date_modified" : "aeiou",
    "date_created" : "aeiou",
    "last_name" : "aeiou",
    "id" : 123,
    "source" : "aeiou",
    "first_name" : "aeiou",
    "order_id" : 123,
    "email" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A Subscriber object
   <a href="#SubscriberResponse">
    SubscriberResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
  </div>
  <div class="method">
   <a name="getSubscribers">
   </a>
   <h2 class_="jumptarget" id="getSubscribers">
    Returns a paginated Subscribers collection.
   </h2>
   <div class_="method-path">
    <span class_="get">
     <span class_="http-method">
      GET
     </span>
     /customers/subscribers
    </span>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Query parameters
   </h3>
   <div class="field-items">
    <div class="param">
     email (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by email.
    </div>
    <div class="param">
     first_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by first_name.
    </div>
    <div class="param">
     last_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by last_name.
    </div>
    <div class="param">
     source (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by source.
    </div>
    <div class="param">
     order_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by order_id.
    </div>
    <div class="param">
     date_created (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_created.
 format: data-time
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Filter items by date_modified.
 format: data-time
    </div>
    <div class="param">
     page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the page in a limited list of products.
    </div>
    <div class="param">
     limit (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Query Parameter
     </span>
     — Control the items per page.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#SubscriberCollectionResponse">
     SubscriberCollectionResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : [ {
    "date_modified" : "aeiou",
    "date_created" : "aeiou",
    "last_name" : "aeiou",
    "id" : 123,
    "source" : "aeiou",
    "first_name" : "aeiou",
    "order_id" : 123,
    "email" : "aeiou"
  } ],
  "meta" : {
    "per_page" : 123,
    "total" : 123,
    "count" : 123,
    "links" : {
      "next" : "aeiou",
      "current" : "aeiou",
      "previous" : "aeiou"
    },
    "total_pages" : 123,
    "current_page" : 123
  }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   An array of subscriber objects and meta data
   <a href="#SubscriberCollectionResponse">
    SubscriberCollectionResponse
   </a>
  </div>
  <div class="method">
   <a name="updateSubscriber">
   </a>
   <h2 class_="jumptarget" id="updateSubscriber">
    Update a `Subscriber` object.
   </h2>
   <div class_="method-path">
    <span class_="put">
     <span class_="http-method">
      PUT
     </span>
     /customers/subscribers/{subscriber_id}
    </span>
   </div>
   <h3 class="field-label">
    Path parameters
   </h3>
   <div class="field-items">
    <div class="param">
     subscriber_id (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Path Parameter
     </span>
     — The id of the `Subscriber` requested.
 format: int
    </div>
   </div>
   <h3 class="field-label">
    Consumes
   </h3>
   This API call consumes the following media types via the
   <span class="heaader">
    Content-Type
   </span>
   request header:
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Request body
   </h3>
   <div class="field-items">
    <div class="param">
     subscriber
     <a href="#Subscriber">
      Subscriber
     </a>
     (required)
    </div>
    <div class="param-desc">
     <span class="param-type">
      Body Parameter
     </span>
     — Returns a `Subscriber` object.
    </div>
   </div>
   <h3 class="field-label">
    Return type
   </h3>
   <div class="return-type">
    <a href="#SubscriberResponse">
     SubscriberResponse
    </a>
   </div>
   <h3 class="field-label">
    Example data
   </h3>
   <div class="example-data-content-type">
    Content-Type: application/json
   </div>
   <pre class="example"><code>{
  "data" : {
    "date_modified" : "aeiou",
    "date_created" : "aeiou",
    "last_name" : "aeiou",
    "id" : 123,
    "source" : "aeiou",
    "first_name" : "aeiou",
    "order_id" : 123,
    "email" : "aeiou"
  },
  "meta" : { }
}</code></pre>
   <h3 class="field-label">
    Produces
   </h3>
   This API call produces the following media types according to the
   <span class="header">
    Accept
   </span>
   request header;
    the media type will be conveyed by the
   <span class="heaader">
    Content-Type
   </span>
   response header.
   <ul>
    <li>
     <code>
      application/json
     </code>
    </li>
   </ul>
   <h3 class="field-label">
    Responses
   </h3>
   <h4 class="field-label">
    200
   </h4>
   A Subscriber object
   <a href="#SubscriberResponse">
    SubscriberResponse
   </a>
   <h4 class="field-label">
    404
   </h4>
   The resource was not found
   <a href="#NotFound">
    NotFound
   </a>
   <h4 class="field-label">
    409
   </h4>
   The `Subscriber` was in conflict with another subscriber. This is the result of duplicate unique value such as email
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
   <h4 class="field-label">
    422
   </h4>
   The `Subscriber` was not valid. This is the result of missing required fields or invalid data. See the response for more details.
   <a href="#ErrorResponse">
    ErrorResponse
   </a>
  </div>
  <hr/>
  <h2 id="__Models" class="jumptarget"> Models – Contents </h2>

[ Jump to <a href="#__Methods">Methods</a> ]
  <ol>
   <li>
    <a href="#Adjuster">
     <code>
      Adjuster
     </code>
    </a>
   </li>
   <li>
    <a href="#BaseError">
     <code>
      BaseError
     </code>
    </a>
   </li>
   <li>
    <a href="#Brand">
     <code>
      Brand
     </code>
    </a>
   </li>
   <li>
    <a href="#BrandCollectionResponse">
     <code>
      BrandCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#BrandResponse">
     <code>
      BrandResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#BulkPricingRule">
     <code>
      BulkPricingRule
     </code>
    </a>
   </li>
   <li>
    <a href="#CatalogSummary">
     <code>
      CatalogSummary
     </code>
    </a>
   </li>
   <li>
    <a href="#CatalogSummaryResponse">
     <code>
      CatalogSummaryResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#Category">
     <code>
      Category
     </code>
    </a>
   </li>
   <li>
    <a href="#CategoryCollectionResponse">
     <code>
      CategoryCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#CategoryNode">
     <code>
      CategoryNode
     </code>
    </a>
   </li>
   <li>
    <a href="#CategoryResponse">
     <code>
      CategoryResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#CategoryTreeCollectionResponse">
     <code>
      CategoryTreeCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#CollectionMeta">
     <code>
      CollectionMeta
     </code>
    </a>
   </li>
   <li>
    <a href="#CollectionMeta_links">
     <code>
      CollectionMeta_links
     </code>
    </a>
   </li>
   <li>
    <a href="#ComplexRule">
     <code>
      ComplexRule
     </code>
    </a>
   </li>
   <li>
    <a href="#ComplexRuleCollectionResponse">
     <code>
      ComplexRuleCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ComplexRuleCondition">
     <code>
      ComplexRuleCondition
     </code>
    </a>
   </li>
   <li>
    <a href="#ComplexRuleResponse">
     <code>
      ComplexRuleResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#CustomField">
     <code>
      CustomField
     </code>
    </a>
   </li>
   <li>
    <a href="#CustomUrl">
     <code>
      CustomUrl
     </code>
    </a>
   </li>
   <li>
    <a href="#DetailedErrors">
     <code>
      DetailedErrors
     </code>
    </a>
   </li>
   <li>
    <a href="#ErrorResponse">
     <code>
      ErrorResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ImageResponse">
     <code>
      ImageResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#Meta">
     <code>
      Meta
     </code>
    </a>
   </li>
   <li>
    <a href="#MetaFieldCollectionResponse">
     <code>
      MetaFieldCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#Metafield">
     <code>
      Metafield
     </code>
    </a>
   </li>
   <li>
    <a href="#MetafieldResponse">
     <code>
      MetafieldResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#Modifier">
     <code>
      Modifier
     </code>
    </a>
   </li>
   <li>
    <a href="#ModifierCollectionResponse">
     <code>
      ModifierCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ModifierResponse">
     <code>
      ModifierResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ModifierValue">
     <code>
      ModifierValue
     </code>
    </a>
   </li>
   <li>
    <a href="#ModifierValue_adjusters">
     <code>
      ModifierValue_adjusters
     </code>
    </a>
   </li>
   <li>
    <a href="#ModifierValue_adjusters_purchasing_disabled">
     <code>
      ModifierValue_adjusters_purchasing_disabled
     </code>
    </a>
   </li>
   <li>
    <a href="#NotFound">
     <code>
      NotFound
     </code>
    </a>
   </li>
   <li>
    <a href="#Option">
     <code>
      Option
     </code>
    </a>
   </li>
   <li>
    <a href="#OptionCollectionResponse">
     <code>
      OptionCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#OptionConfig">
     <code>
      OptionConfig
     </code>
    </a>
   </li>
   <li>
    <a href="#OptionResponse">
     <code>
      OptionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#OptionValue">
     <code>
      OptionValue
     </code>
    </a>
   </li>
   <li>
    <a href="#OptionValueShort">
     <code>
      OptionValueShort
     </code>
    </a>
   </li>
   <li>
    <a href="#OptionValueShortPost">
     <code>
      OptionValueShortPost
     </code>
    </a>
   </li>
   <li>
    <a href="#Product">
     <code>
      Product
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductCollectionResponse">
     <code>
      ProductCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductImage">
     <code>
      ProductImage
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductImageCollectionResponse">
     <code>
      ProductImageCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductImageResponse">
     <code>
      ProductImageResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductPost">
     <code>
      ProductPost
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductPut">
     <code>
      ProductPut
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductResponse">
     <code>
      ProductResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductVideo">
     <code>
      ProductVideo
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductVideoCollectionResponse">
     <code>
      ProductVideoCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ProductVideoResponse">
     <code>
      ProductVideoResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#ResourceImage">
     <code>
      ResourceImage
     </code>
    </a>
   </li>
   <li>
    <a href="#Subscriber">
     <code>
      Subscriber
     </code>
    </a>
   </li>
   <li>
    <a href="#SubscriberCollectionResponse">
     <code>
      SubscriberCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#SubscriberResponse">
     <code>
      SubscriberResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#Variant">
     <code>
      Variant
     </code>
    </a>
   </li>
   <li>
    <a href="#VariantCollectionResponse">
     <code>
      VariantCollectionResponse
     </code>
    </a>
   </li>
   <li>
    <a href="#VariantPost">
     <code>
      VariantPost
     </code>
    </a>
   </li>
   <li>
    <a href="#VariantResponse">
     <code>
      VariantResponse
     </code>
    </a>
   </li>
  </ol>
  <div class="model">
   <h3 class="field-label">
    <a name="Adjuster">
     Adjuster -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     adjuster (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of adjuster as either `relative` or `percentage` for either the price or the weight of the variant when the modifier value is selected on the storefront.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     relative
    </div>
    <div class="param-enum">
     percentage
    </div>
    <div class="param">
     adjuster_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#number">
       BigDecimal
      </a>
     </span>
     The numeric amount the adjuster will change either the price or the weight of the variant when the modifier value is selected on the storefront.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="BaseError">
     BaseError -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Error payload for the BigCommerce API
   </div>
   <div class="field-items">
    <div class="param">
     status (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The HTTP status code
    </div>
    <div class="param">
     title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The error title describing the particular
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
    <div class="param">
     instance (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Brand">
     Brand -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the brand, increments sequentially.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the brand. Must be unique
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The title shown in the browser while viewing the brand
    </div>
    <div class="param">
     meta_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     Comma separated list of meta keywords to include in the HTML
    </div>
    <div class="param">
     meta_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A meta description to include
    </div>
    <div class="param">
     search_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A comma separated list of keywords that can be used to locate this brand
    </div>
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     URL of the image url for this category used on the storefront. Images can be uploaded via form file post to /brannds/{brandId}/image or by providing publicly accessible URL to this field.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="BrandCollectionResponse">
     BrandCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Brand">
       array[Brand]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="BrandResponse">
     BrandResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Brand">
       Brand
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="BulkPricingRule">
     BulkPricingRule -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Rules that offer price discounts based on quantity breaks.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The ID of the bulk pricing rule.
    </div>
    <div class="param">
     quantity_min (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The maximum inclusive quantity of a product to satisfy this rule. Must be greater than the min value, unless this field has a value of 0 (zero), in which case there will be no maximum bound for this rule.
    </div>
    <div class="param">
     quantity_max (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The minimum inclusive quantity of a product to satisfy this rule. Must be greater than or equal to zero.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of adjument that is made, 'price' - The adjument amount per product, 'percent' - The adjustment as a percent of the original price, 'fixed' - the adjusted absolute price of the product.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     price
    </div>
    <div class="param-enum">
     percent
    </div>
    <div class="param-enum">
     fixed
    </div>
    <div class="param">
     amount (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The value of the adjusted by the bulk pricing rule.
 format: double
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CatalogSummary">
     CatalogSummary -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    A BigCommerce Catalog Summary object describes a lightweight summary of the catalog.
   </div>
   <div class="field-items">
    <div class="param">
     inventory_count (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     A count of all inventory items in the catalog.
    </div>
    <div class="param">
     inventory_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Total value of store's inventory.
 format: double
    </div>
    <div class="param">
     primary_category_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Id of the category containing the most of products.
    </div>
    <div class="param">
     primary_category_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Name of the category containing the most of products.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CatalogSummaryResponse">
     CatalogSummaryResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CatalogSummary">
       CatalogSummary
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Category">
     Category -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    A BigCommerce category object.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the category, increments sequentially.
    </div>
    <div class="param">
     parent_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the category's parent. This field controls where the category sits in the tree of categories that organize the catalog.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name displayed for the category. Name is unique to the category's siblings.
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product description which can include HTML formatting.
    </div>
    <div class="param">
     views (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Number of views the category has on the storefront
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Priority this category will be given when included in the menu and category pages. The lower the number, the closer to the top of the results the category will be.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom title for the category page, if not defined the category name will be used as the meta title.
    </div>
    <div class="param">
     meta_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     Custom meta keywords for the category page, if not defined the store default keywords will be used. Must post as an array like: ["awesome","sauce"]
    </div>
    <div class="param">
     meta_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom meta description for the category page, if not defined the store default meta description will be used.
    </div>
    <div class="param">
     layout_file (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The layout template file used to render this category.
    </div>
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     URL of the image url for this category used on the storefront. Images can be uploaded via form file post to /categories/{categoryId}/image or by providing publicly accessible URL to this field.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be displayed to customers browsing the store or not. If true the category will be displayed, false the category will be hidden from view.
    </div>
    <div class="param">
     search_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A comma separated list of keywords that can be used to locate the category when searching the store.
    </div>
    <div class="param">
     default_product_sort (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Determines how the products are sorted on category page load.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     use_store_settings
    </div>
    <div class="param-enum">
     featured
    </div>
    <div class="param-enum">
     newest
    </div>
    <div class="param-enum">
     best_selling
    </div>
    <div class="param-enum">
     alpha_asc
    </div>
    <div class="param-enum">
     alpha_desc
    </div>
    <div class="param-enum">
     avg_customer_review
    </div>
    <div class="param-enum">
     price_asc
    </div>
    <div class="param-enum">
     price_desc
    </div>
    <div class="param">
     custom_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomUrl">
       CustomUrl
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CategoryCollectionResponse">
     CategoryCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Category">
       array[Category]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CategoryNode">
     CategoryNode -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    A BigCommerce category node object. Used to reflect parent &lt;&gt; child category relationships.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the category, increments sequentially.
    </div>
    <div class="param">
     parent_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the category's parent. This field controls where the category sits in the tree of categories that organize the catalog.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name displayed for the category. Name is unique to the category's siblings.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be displayed to customers browsing the store or not. If true the category will be displayed, false the category will be hidden from view.
    </div>
    <div class="param">
     url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The custom url for the category on the store front.
    </div>
    <div class="param">
     children (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CategoryNode">
       array[CategoryNode]
      </a>
     </span>
     The list of children of the category.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CategoryResponse">
     CategoryResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Category">
       Category
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CategoryTreeCollectionResponse">
     CategoryTreeCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CategoryNode">
       array[CategoryNode]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CollectionMeta">
     CollectionMeta -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Data about the response including pagination and collection totals
   </div>
   <div class="field-items">
    <div class="param">
     total (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Total number of items return in the result set
    </div>
    <div class="param">
     count (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Total number of items in the collection
    </div>
    <div class="param">
     per_page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The amount of items returned in the collection per page, controlled by the limit parameter
    </div>
    <div class="param">
     current_page (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The page you are currently on within the collection
    </div>
    <div class="param">
     total_pages (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The total number of pages in the collection
    </div>
    <div class="param">
     links (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta_links">
       CollectionMeta_links
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CollectionMeta_links">
     CollectionMeta_links -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Pagination links for the previous and next parts of the whole collection
   </div>
   <div class="field-items">
    <div class="param">
     previous (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Link to the previous page returned in the response
    </div>
    <div class="param">
     current (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Link to the current page returned in the response
    </div>
    <div class="param">
     next (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Link to the next page returned in the response
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ComplexRule">
     ComplexRule -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Apply price, weight. image, or availabilty adjustments to product based on a set of conditions. A complex rule's condistion must contain more than one modifier value or a modifier value and a variant id.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the rule, increments sequentially.
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the product the rule is associated with, increments sequentially.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Priority this rule will be given when make adjustments to the product properties.
    </div>
    <div class="param">
     enabled (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag for determining if the rule is to be used when adjusting a product's price, weight. image, or availabilty.
    </div>
    <div class="param">
     stop (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag for determining if other rules should not be applied after this rule has been applied.
    </div>
    <div class="param">
     price_adjuster (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Adjuster">
       Adjuster
      </a>
     </span>
    </div>
    <div class="param">
     weight_adjuster (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Adjuster">
       Adjuster
      </a>
     </span>
    </div>
    <div class="param">
     purchasing_disabled (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag for determining if the rule should disable purchasing of a product when the conditions are applied.
    </div>
    <div class="param">
     purchasing_disabled_message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Message presented in the storefront when a rule disables the purchasing of a product.
    </div>
    <div class="param">
     purchasing_hidden (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag for determining if the rule should hide purchasing of a product when the conditions are applied.
    </div>
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The url for an image displayed on the storefront when the conditions are applied.
    </div>
    <div class="param">
     conditions (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ComplexRuleCondition">
       array[ComplexRuleCondition]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ComplexRuleCollectionResponse">
     ComplexRuleCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ComplexRule">
       array[ComplexRule]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ComplexRuleCondition">
     ComplexRuleCondition -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Complex rule conditions associated a rule with a particular combination of modifier values or variants and modifier values. Complex rules may return with conditions that apply to one or more variants or a single modifier value of the rules were created using the V2 API or the Control Panel. Complex rules created or updated in V3 must have conditions referencing multiple `modifier_value_id`(s) or a `modifier_value_id` and a `variant_id`.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the rule condition, increments sequentially.
    </div>
    <div class="param">
     rule_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the rule the condition is associated with.
    </div>
    <div class="param">
     modifier_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the modifier the rule condition is associated with.
    </div>
    <div class="param">
     modifier_value_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the modifier value the rule condition is associated with.
    </div>
    <div class="param">
     variant_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the variant the rule condition is associated with.
    </div>
    <div class="param">
     combination_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     (READ ONLY) The unique numerical ID of the SKU (V2 API) or Combination the rule condition is associated with. This is to maintain cross compatibility between V2 and V3.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ComplexRuleResponse">
     ComplexRuleResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ComplexRule">
       ComplexRule
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CustomField">
     CustomField -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Gets custom fields associated with a product, which allow you to specify additional information that will appear on the product's page, such as a book's ISBN or a DVD's release date.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the custom field, increments sequentially
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the field shown on the store front, orders, etc..
    </div>
    <div class="param">
     value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The values or text of the field shown on the store front, orders, etc..
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical identifier for the product that the field is associated with.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="CustomUrl">
     CustomUrl -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    The custom url for the product on the store front.
   </div>
   <div class="field-items">
    <div class="param">
     url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Product url on the store front.
    </div>
    <div class="param">
     is_customized (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Returns true if the url has been changed from it's default state (the auto-assigned url BigCommerce provides)
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="DetailedErrors">
     DetailedErrors -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ErrorResponse">
     ErrorResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     status (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The HTTP status code
    </div>
    <div class="param">
     title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The error title describing the particular
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
    <div class="param">
     instance (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
    <div class="param">
     errors (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#DetailedErrors">
       DetailedErrors
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ImageResponse">
     ImageResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ResourceImage">
       ResourceImage
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Meta">
     Meta -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Empty meta object, may be used later
   </div>
   <div class="field-items">
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="MetaFieldCollectionResponse">
     MetaFieldCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Metafield">
       array[Metafield]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Metafield">
     Metafield -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Allows for app partners to write custom data to various resources in the API.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique identifier for the meta fields.
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Description for the meta fields.
    </div>
    <div class="param">
     permission_set (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Determines if the field is completely private to the app that owns the field (app_only), visible to other API consumers (read), or completely open for reading and writing to other apps (write).
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     app_only
    </div>
    <div class="param-enum">
     read
    </div>
    <div class="param-enum">
     write
    </div>
    <div class="param">
     namespace (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Namespace for the meta field for organizational purposes.
    </div>
    <div class="param">
     resource_type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of resource that the meta field is associated with.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     category
    </div>
    <div class="param-enum">
     brand
    </div>
    <div class="param-enum">
     product
    </div>
    <div class="param-enum">
     variant
    </div>
    <div class="param">
     resource_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique identifier for the resource that the meta field is associated with.
    </div>
    <div class="param">
     key (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the field i.e. "location_id", "color"
    </div>
    <div class="param">
     value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The value of the field i.e. "1", "blue"
    </div>
    <div class="param">
     created_at (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#DateTime">
       Date
      </a>
     </span>
     Created date and time for the meta field
 format: date-time
    </div>
    <div class="param">
     updated_at (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#DateTime">
       Date
      </a>
     </span>
     Last updated date and time for the metafield
 format: date-time
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="MetafieldResponse">
     MetafieldResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Metafield">
       Metafield
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Modifier">
     Modifier -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the modifier, increments sequentially.
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the product that the option belongs to.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name unique option name auto-generated from the display name, a timestamp, and the product id.
    </div>
    <div class="param">
     display_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the option shown on the store front.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of modifier, which determines how it will display on the storefront. For reference, former v2 API values:
D = date, C = checkbox, F = file, T = text, MT = multi_line_text, N = numbers_only_text, RB = radio_buttons,
RT = rectangles, S = dropdown, P = product_list, PI = product_list_with_images, CS = swatch
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     date
    </div>
    <div class="param-enum">
     checkbox
    </div>
    <div class="param-enum">
     file
    </div>
    <div class="param-enum">
     text
    </div>
    <div class="param-enum">
     multi_line_text
    </div>
    <div class="param-enum">
     numbers_only_text
    </div>
    <div class="param-enum">
     radio_buttons
    </div>
    <div class="param-enum">
     rectangles
    </div>
    <div class="param-enum">
     dropdown
    </div>
    <div class="param-enum">
     product_list
    </div>
    <div class="param-enum">
     product_list_with_images
    </div>
    <div class="param-enum">
     swatch
    </div>
    <div class="param">
     required (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Whether this modifer is required or not at checkout
    </div>
    <div class="param">
     config (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#OptionConfig">
       OptionConfig
      </a>
     </span>
    </div>
    <div class="param">
     option_values (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ModifierValue">
       array[ModifierValue]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ModifierCollectionResponse">
     ModifierCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Modifier">
       array[Modifier]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ModifierResponse">
     ModifierResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Modifier">
       Modifier
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ModifierValue">
     ModifierValue -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the value, increments sequentially.
    </div>
    <div class="param">
     is_default (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     The flag for preselecting a value as the default on the store front. This field is not supported for swatch options/modifiers.
    </div>
    <div class="param">
     label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The text display identifying the value on the store front.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The order in which the value will be displayed on the product page.
    </div>
    <div class="param">
     value_data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#object">
       Object
      </a>
     </span>
     Extra data describing the value based on the type of option or modifier that the value is associated with swatch requires an array of colors with up to three hexidecimal color keys, product list requires a `product_id`, and checkbox requires boolean flag called `checked_value` to determine which value is considered to be the checked state.
    </div>
    <div class="param">
     adjusters (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ModifierValue_adjusters">
       ModifierValue_adjusters
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ModifierValue_adjusters">
     ModifierValue_adjusters -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Adjuster">
       Adjuster
      </a>
     </span>
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Adjuster">
       Adjuster
      </a>
     </span>
    </div>
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The url for an image displayed on the storefront when the modifier value is selected.
    </div>
    <div class="param">
     purchasing_disabled (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ModifierValue_adjusters_purchasing_disabled">
       ModifierValue_adjusters_purchasing_disabled
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ModifierValue_adjusters_purchasing_disabled">
     ModifierValue_adjusters_purchasing_disabled -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     status (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag for whether the modifier value disables purchasing when selected on the storefront. This can be used for temporarily disabling a particular modifier value.
    </div>
    <div class="param">
     message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The message displayed on the storefront when the purchasing disabled status is `true`.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="NotFound">
     NotFound -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Error payload for the BigCommerce API
   </div>
   <div class="field-items">
    <div class="param">
     status (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     404 HTTP status code
    </div>
    <div class="param">
     title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The error title describing the particular
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
    <div class="param">
     instance (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Option">
     Option -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the option, increments sequentially.
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the product that the option belongs to.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name unique option name auto-generated from the display name, a timestamp, and the product id.
    </div>
    <div class="param">
     display_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the option shown on the store front.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of option, which determines how it will display on the storefront. For reference, former v2 API values:
RB = radio_buttons, RT = rectangles, S = dropdown, P = product_list, PI = product_list_with_images, CS = swatch
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     radio_buttons
    </div>
    <div class="param-enum">
     rectangles
    </div>
    <div class="param-enum">
     dropdown
    </div>
    <div class="param-enum">
     product_list
    </div>
    <div class="param-enum">
     product_list_with_images
    </div>
    <div class="param-enum">
     swatch
    </div>
    <div class="param">
     config (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#OptionConfig">
       OptionConfig
      </a>
     </span>
    </div>
    <div class="param">
     option_values (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#OptionValue">
       array[OptionValue]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="OptionCollectionResponse">
     OptionCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Option">
       array[Option]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="OptionConfig">
     OptionConfig -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     default_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     (date, text, multi_line_text, numbers_only_text) The default value shown on a date option as an ISO-8601 formatted string or text option as a string.
    </div>
    <div class="param">
     checked_by_default (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (checkbox) Flag for setting the check box to be checked by default.
    </div>
    <div class="param">
     checkbox_label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     (checkbox) Label displayed for the checkbox option.
    </div>
    <div class="param">
     date_limited (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (date) Flag to limit the date allowed to be entered on a date option.
    </div>
    <div class="param">
     date_limit_mode (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     (date) The type of limit that is allowed to be entered on a date option (`earliest`, `range`, `latest`).
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     earliest
    </div>
    <div class="param-enum">
     range
    </div>
    <div class="param-enum">
     latest
    </div>
    <div class="param">
     date_earliest_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#date">
       date
      </a>
     </span>
     (date) The earliest date allowed to be entered on the date option as an ISO-8601 formatted string.
 format: date
    </div>
    <div class="param">
     date_latest_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#date">
       date
      </a>
     </span>
     (date) The latest date allowed to be entered on the date option as an ISO-8601 formatted string.
 format: date
    </div>
    <div class="param">
     file_types_mode (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     (file) The kind of restriction on the type of files that can be uploaded to a file upload option.
  `specific` - restricts upload to particular file types.
  `all` - allows all files types.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     specific
    </div>
    <div class="param-enum">
     all
    </div>
    <div class="param">
     file_types_supported (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     (file) The kind of files allowed to be uploaded if the `file_type_option` is set to `specific`.
  `images` - Allows upload of image MIME types (`bmp`,`gif`,`jpg`,`jpeg`,`jpe`,`jif`,`jfif`,`jfi`,`png`,`wbmp`,`xbm`,`tiff`).
  `documents` - Allows upload of document MIME types (`txt`,`pdf`,`rtf`,`doc`,`docx`,`xls`,`xlsx`,`accdb`,`mdb`,`one`,`pps`,`ppsx`,`ppt`,`pptx`,`pub`,`odt`,`ods`,`odp`,`odg`,`odf`).
  `other` - Allows other file type defined in the `file_types_other` array.
    </div>
    <div class="param">
     file_types_other (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     (file) A list of other files types allowed with the file upload option.
    </div>
    <div class="param">
     file_max_size (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     (file) The maximum size of the file that can be used in the file upload option.
    </div>
    <div class="param">
     text_characters_limited (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (text, multi_line_text) Flag to validate the length of the text of a text or multi-line text input.
    </div>
    <div class="param">
     text_min_length (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     (text, multi_line_text) The minimum length allowed for a text or multi-line text option.
    </div>
    <div class="param">
     text_max_length (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     (text, multi_line_text) The maximum length allowed for a text or multi line text option.
    </div>
    <div class="param">
     text_lines_limited (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (multi_line_text) Flag to validate the maximum number of lines allowed on a multi-line text input.
    </div>
    <div class="param">
     text_max_lines (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     (multi_line_text) The maximum number of lines allowed on a multi-line text input.
    </div>
    <div class="param">
     number_limited (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (numbers_only_text) Flag to limit the value of a number option.
    </div>
    <div class="param">
     number_limit_mode (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     (numbers_only_text) The type of limit that is allowed to be entered on a number option (`lowest`, `highest`, `range`).
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     lowest
    </div>
    <div class="param-enum">
     highest
    </div>
    <div class="param-enum">
     range
    </div>
    <div class="param">
     number_lowest_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#number">
       BigDecimal
      </a>
     </span>
     (numbers_only_text) The lowest allowed value for a number option if `limit_input` is true.
    </div>
    <div class="param">
     number_highest_value (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#number">
       BigDecimal
      </a>
     </span>
     (numbers_only_text) The highest allowed value for a number option if `limit_input` is true.
    </div>
    <div class="param">
     number_integers_only (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (numbers_only_text) Flag to limit the imput on a number option to only accept whole numbers.
    </div>
    <div class="param">
     product_list_adjusts_inventory (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (product_list, product_list_with_images) Flag for automatically adjusting inventory on a product included in the list.
    </div>
    <div class="param">
     product_list_adjusts_pricing (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     (product_list, product_list_with_images) Flag to add the price of the optional product to the price of the main product
    </div>
    <div class="param">
     product_list_shipping_calc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     (product_list, product_list_with_images)  How to factor the optional product's weight and dimensions (package) into the shipping quote (none - don't adjust, weight - use shipping weight only, package - use package, weight and dimensions)
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     weight
    </div>
    <div class="param-enum">
     package
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="OptionResponse">
     OptionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Option">
       Option
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="OptionValue">
     OptionValue -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the value, increments sequentially.
    </div>
    <div class="param">
     is_default (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     The flag for preselecting a value as the default on the store front. This field is not supported for swatch options/modifiers.
    </div>
    <div class="param">
     label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The text display identifying the value on the store front.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The order in which the value will be displayed on the product page.
    </div>
    <div class="param">
     value_data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#object">
       Object
      </a>
     </span>
     Extra data describing the value based on the type of option or modifier that the value is associated with swatch requires an array of colors with up to three hexidecimal color keys, product list requires a `product_id`, and checkbox requires boolean flag called `checked_value` to determine which value is considered to be the checked state.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="OptionValueShort">
     OptionValueShort -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
    </div>
    <div class="param">
     option_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
    </div>
    <div class="param">
     option_display_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the option
    </div>
    <div class="param">
     label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The label of the option value
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="OptionValueShortPost">
     OptionValueShortPost -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     option_display_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The name of the option to be created on POST
    </div>
    <div class="param">
     label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The label of the option value to be created on POST
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Product">
     Product -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    A BigCommerce Product object describes a single or collection of purchasable units.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the product, increments sequentially.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product name.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product type: physical - a physical stock unit, digital - a digital download
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     physical
    </div>
    <div class="param-enum">
     digital
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     User defined product code/stock keeping unit (SKU).
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product description which can include HTML formatting.
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Weight of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     width (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Width of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     depth (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Depth of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     height (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Height of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The price of the product, the price should include or exclude tax based on the store settings.
 format: double
    </div>
    <div class="param">
     cost_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The cost price of the product, stored for reference only, it is not used or displayed anywhere on the store.
 format: double
    </div>
    <div class="param">
     retail_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The retail cost of the product, if entered the retail cost price will be shown on the product page.
 format: double
    </div>
    <div class="param">
     sale_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The sale price will be used instead of value in the price field when calculating the products cost if entered.
 format: double
    </div>
    <div class="param">
     tax_class_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The ID of the tax class applied to the product. NOTE: Value ignored if automatic tax is enabled.
    </div>
    <div class="param">
     product_tax_code (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Accepts AvaTax system codes that identify products and services that fall into special sales tax categories. Allows merchants that subscribe to Avalara Premium to achieve increased accuracy in sales tax calculations. Stores without Avalara Premium will ignore the code when calculating sales tax. Do not pass more than one code. The codes are case-sensitive. Refer to the 'AvaTax System tax codes' section of the following page for further information and the full list of codes: https://help.avalara.com/000_AvaTax_Calc/000AvaTaxCalc_User_Guide/040_Managing_Tax_Profiles/050_Tax_Codes/001_What_is_a_Tax_Code
    </div>
    <div class="param">
     calculated_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The price of the product unless a sale_price is set.
 format: double
    </div>
    <div class="param">
     categories (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       array[Integer]
      </a>
     </span>
     An array of IDs for the categories this product belongs to. When updating a product, if an array of categories is supplied all product categories will be overwritten. Does not accept more than 1,000 ID values.
    </div>
    <div class="param">
     brand_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The id associated with the product's brand.
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Current inventory level of the product. Simple inventory tracking must be enabled (See the inventory_tracking field) for this to take any effect.
    </div>
    <div class="param">
     inventory_warning_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Inventory Warning level for the product. When the products inventory level drops below the warning level the store owner will be informed. Simple inventory tracking must be enabled (See the inventory_tracking field) for this to take any effect.
    </div>
    <div class="param">
     inventory_tracking (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of inventory tracking for the product: none - inventory levels will not be tracked. product - inventory levels will be tracked using the 'inventory_level' and 'inventory_warning_level' fields. variant - inventory levels will be tracked based on  variants which maintain their own warning levels and inventory levels.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     product
    </div>
    <div class="param-enum">
     variant
    </div>
    <div class="param">
     fixed_cost_shipping_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     A fixed shipping cost for the product, if defined the value will be used during checkout instead of normal shipping cost calculation.
    </div>
    <div class="param">
     is_free_shipping (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag used to indicate if the product has free shipping or not. If true the shipping cost for the product will be zero.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be displayed to customers browsing the store or not. If true the product will be displayed, false the product will be hidden from view.
    </div>
    <div class="param">
     is_featured (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be included in 'featured products' panel when viewing the store.
    </div>
    <div class="param">
     warranty (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Warranty information displayed on the product page which can include HTML formatting.
    </div>
    <div class="param">
     bin_picking_number (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The BIN picking number for the product.
    </div>
    <div class="param">
     layout_file (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The layout template file used to render this product.
    </div>
    <div class="param">
     upc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product UPC code which is used in feeds for shopping comparison sites and external channel integrations.
    </div>
    <div class="param">
     search_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A comma separated list of keywords that can be used to locate the product when searching the store.
    </div>
    <div class="param">
     availability (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Availability of the product. availability options: available - The product can be purchased in the store front. disabled - The product is listed in the store front but can not be purchased. preorder - The product is listed for pre-orders.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     available
    </div>
    <div class="param-enum">
     disabled
    </div>
    <div class="param-enum">
     preorder
    </div>
    <div class="param">
     availability_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Availability text displayed on the checkout page under the product title telling the customer how long it will normally take to ship this product, such as 'Usually ships in 24 hours'.
    </div>
    <div class="param">
     gift_wrapping_options_type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     `any` - allow any gift wrapping options in the store, `none` - disallow gift wrapping on the product. When the type is set to `list`, a list of ids in gift_wrapping_options_list field should be provided.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     any
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     list
    </div>
    <div class="param">
     gift_wrapping_options_list (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       array[Integer]
      </a>
     </span>
     A list of gift wrapping option ids.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Priority this product will be given when included in product lists on category pages and search results. The lower the number, the closer to the top of the results the product will be.
    </div>
    <div class="param">
     condition (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product condition, will be shown on the product page if the value of the 'is_condition_shown' field is true. Possible values: New, Used, Refurbished
    </div>
    <div class="param">
     is_condition_shown (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag used to determine if the product condition is shown to the customer on the product page.
    </div>
    <div class="param">
     order_quantity_minimum (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The minimum quantity an order has to contain to be able to purchase this product.
    </div>
    <div class="param">
     order_quantity_maximum (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The maximum quantity an order can contain when purchasing the product.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom title for the products page, if not defined the product name will be used as the meta title.
    </div>
    <div class="param">
     meta_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     Custom meta keywords for the product page, if not defined the store default keywords will be used.
    </div>
    <div class="param">
     meta_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom meta description for the product page, if not defined the store default meta description will be used.
    </div>
    <div class="param">
     date_created (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the product was created.
 format: data-time
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the product was created.
 format: data-time
    </div>
    <div class="param">
     view_count (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The number of times the product has been viewed.
    </div>
    <div class="param">
     preorder_release_date (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Pre-order release date. See availability field for details on setting a products availability to accept pre-orders.
 format: data-time
    </div>
    <div class="param">
     preorder_message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom expected date message to display on the product page, if undefined the message defaults to the store wide setting. Can contain the %%DATE%% place holder which will be substituted for the release date
    </div>
    <div class="param">
     is_preorder_only (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     If set to false, the product will not change its availability from preorder to available on the release date. Otherwise on the release date the products availability/status will change to available.
    </div>
    <div class="param">
     is_price_hidden (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     False by default, which indicates that the price of this product should be shown on the product page. If set to 'true', the price is hidden. NOTE: To successfully set 'is_price_hidden' to 'true', the 'availability' value must be 'disabled'.
    </div>
    <div class="param">
     price_hidden_label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     By default, an empty string. If 'is_price_hidden' is 'true', the value of 'price_hidden_label' is displayed instead of the price. NOTE: To successfully set a non-empty string value for 'is_price_hidden' to 'true', the 'availability' value must be 'disabled'.
    </div>
    <div class="param">
     images (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductImage">
       array[ProductImage]
      </a>
     </span>
    </div>
    <div class="param">
     videos (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductVideo">
       array[ProductVideo]
      </a>
     </span>
    </div>
    <div class="param">
     custom_fields (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomField">
       array[CustomField]
      </a>
     </span>
    </div>
    <div class="param">
     custom_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomUrl">
       CustomUrl
      </a>
     </span>
    </div>
    <div class="param">
     bulk_pricing_rules (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#BulkPricingRule">
       array[BulkPricingRule]
      </a>
     </span>
    </div>
    <div class="param">
     variants (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Variant">
       array[Variant]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductCollectionResponse">
     ProductCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Product">
       array[Product]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductImage">
     ProductImage -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    An product image model.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the image, increments sequentially
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical identifier for the product that the image is associated with.
    </div>
    <div class="param">
     is_thumbnail (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag for identifying if the image is used as the product's thumbnail.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The order in which the image will be displayed on the product page. When updating if the image is given a lower priority, all image with a sort_order the same or greater than the images new sort_order value will have their sort_order reordered
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The description for the image.
    </div>
    <div class="param">
     image_file (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The local path to the original image file uploaded to BigCommerce. Must be POSTed into as a multipart/form-data field.
    </div>
    <div class="param">
     url_zoom (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The zoom url for this image.
    </div>
    <div class="param">
     url_standard (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Url The standard url for this image.
    </div>
    <div class="param">
     url_thumbnail (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Url fThe thumbnail url for this image.
    </div>
    <div class="param">
     url_tiny (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The tiny url for this image.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductImageCollectionResponse">
     ProductImageCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductImage">
       array[ProductImage]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductImageResponse">
     ProductImageResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductImage">
       ProductImage
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductPost">
     ProductPost -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the product, increments sequentially.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product name.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product type: physical - a physical stock unit, digital - a digital download
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     physical
    </div>
    <div class="param-enum">
     digital
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     User defined product code/stock keeping unit (SKU).
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product description which can include HTML formatting.
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Weight of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     width (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Width of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     depth (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Depth of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     height (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Height of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The price of the product, the price should include or exclude tax based on the store settings.
 format: double
    </div>
    <div class="param">
     cost_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The cost price of the product, stored for reference only, it is not used or displayed anywhere on the store.
 format: double
    </div>
    <div class="param">
     retail_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The retail cost of the product, if entered the retail cost price will be shown on the product page.
 format: double
    </div>
    <div class="param">
     sale_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The sale price will be used instead of value in the price field when calculating the products cost if entered.
 format: double
    </div>
    <div class="param">
     tax_class_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The ID of the tax class applied to the product. NOTE: Value ignored if automatic tax is enabled.
    </div>
    <div class="param">
     product_tax_code (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Accepts AvaTax system codes that identify products and services that fall into special sales tax categories. Allows merchants that subscribe to Avalara Premium to achieve increased accuracy in sales tax calculations. Stores without Avalara Premium will ignore the code when calculating sales tax. Do not pass more than one code. The codes are case-sensitive. Refer to the 'AvaTax System tax codes' section of the following page for further information and the full list of codes: https://help.avalara.com/000_AvaTax_Calc/000AvaTaxCalc_User_Guide/040_Managing_Tax_Profiles/050_Tax_Codes/001_What_is_a_Tax_Code
    </div>
    <div class="param">
     calculated_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The price of the product unless a sale_price is set.
 format: double
    </div>
    <div class="param">
     categories (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       array[Integer]
      </a>
     </span>
     An array of IDs for the categories this product belongs to. When updating a product, if an array of categories is supplied all product categories will be overwritten. Does not accept more than 1,000 ID values.
    </div>
    <div class="param">
     brand_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The id associated with the product's brand.
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Current inventory level of the product. Simple inventory tracking must be enabled (See the inventory_tracking field) for this to take any effect.
    </div>
    <div class="param">
     inventory_warning_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Inventory Warning level for the product. When the products inventory level drops below the warning level the store owner will be informed. Simple inventory tracking must be enabled (See the inventory_tracking field) for this to take any effect.
    </div>
    <div class="param">
     inventory_tracking (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of inventory tracking for the product: none - inventory levels will not be tracked. product - inventory levels will be tracked using the 'inventory_level' and 'inventory_warning_level' fields. variant - inventory levels will be tracked based on  variants which maintain their own warning levels and inventory levels.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     product
    </div>
    <div class="param-enum">
     variant
    </div>
    <div class="param">
     fixed_cost_shipping_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     A fixed shipping cost for the product, if defined the value will be used during checkout instead of normal shipping cost calculation.
    </div>
    <div class="param">
     is_free_shipping (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag used to indicate if the product has free shipping or not. If true the shipping cost for the product will be zero.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be displayed to customers browsing the store or not. If true the product will be displayed, false the product will be hidden from view.
    </div>
    <div class="param">
     is_featured (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be included in 'featured products' panel when viewing the store.
    </div>
    <div class="param">
     warranty (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Warranty information displayed on the product page which can include HTML formatting.
    </div>
    <div class="param">
     bin_picking_number (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The BIN picking number for the product.
    </div>
    <div class="param">
     layout_file (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The layout template file used to render this product.
    </div>
    <div class="param">
     upc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product UPC code which is used in feeds for shopping comparison sites and external channel integrations.
    </div>
    <div class="param">
     search_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A comma separated list of keywords that can be used to locate the product when searching the store.
    </div>
    <div class="param">
     availability (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Availability of the product. availability options: available - The product can be purchased in the store front. disabled - The product is listed in the store front but can not be purchased. preorder - The product is listed for pre-orders.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     available
    </div>
    <div class="param-enum">
     disabled
    </div>
    <div class="param-enum">
     preorder
    </div>
    <div class="param">
     availability_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Availability text displayed on the checkout page under the product title telling the customer how long it will normally take to ship this product, such as 'Usually ships in 24 hours'.
    </div>
    <div class="param">
     gift_wrapping_options_type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     `any` - allow any gift wrapping options in the store, `none` - disallow gift wrapping on the product. When the type is set to `list`, a list of ids in gift_wrapping_options_list field should be provided.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     any
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     list
    </div>
    <div class="param">
     gift_wrapping_options_list (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       array[Integer]
      </a>
     </span>
     A list of gift wrapping option ids.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Priority this product will be given when included in product lists on category pages and search results. The lower the number, the closer to the top of the results the product will be.
    </div>
    <div class="param">
     condition (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product condition, will be shown on the product page if the value of the 'is_condition_shown' field is true. Possible values: New, Used, Refurbished
    </div>
    <div class="param">
     is_condition_shown (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag used to determine if the product condition is shown to the customer on the product page.
    </div>
    <div class="param">
     order_quantity_minimum (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The minimum quantity an order has to contain to be able to purchase this product.
    </div>
    <div class="param">
     order_quantity_maximum (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The maximum quantity an order can contain when purchasing the product.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom title for the products page, if not defined the product name will be used as the meta title.
    </div>
    <div class="param">
     meta_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     Custom meta keywords for the product page, if not defined the store default keywords will be used.
    </div>
    <div class="param">
     meta_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom meta description for the product page, if not defined the store default meta description will be used.
    </div>
    <div class="param">
     date_created (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the product was created.
 format: data-time
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the product was created.
 format: data-time
    </div>
    <div class="param">
     view_count (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The number of times the product has been viewed.
    </div>
    <div class="param">
     preorder_release_date (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Pre-order release date. See availability field for details on setting a products availability to accept pre-orders.
 format: data-time
    </div>
    <div class="param">
     preorder_message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom expected date message to display on the product page, if undefined the message defaults to the store wide setting. Can contain the %%DATE%% place holder which will be substituted for the release date
    </div>
    <div class="param">
     is_preorder_only (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     If set to false, the product will not change its availability from preorder to available on the release date. Otherwise on the release date the products availability/status will change to available.
    </div>
    <div class="param">
     is_price_hidden (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     False by default, which indicates that the price of this product should be shown on the product page. If set to 'true', the price is hidden. NOTE: To successfully set 'is_price_hidden' to 'true', the 'availability' value must be 'disabled'.
    </div>
    <div class="param">
     price_hidden_label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     By default, an empty string. If 'is_price_hidden' is 'true', the value of 'price_hidden_label' is displayed instead of the price. NOTE: To successfully set a non-empty string value for 'is_price_hidden' to 'true', the 'availability' value must be 'disabled'.
    </div>
    <div class="param">
     images (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductImage">
       array[ProductImage]
      </a>
     </span>
    </div>
    <div class="param">
     videos (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductVideo">
       array[ProductVideo]
      </a>
     </span>
    </div>
    <div class="param">
     custom_fields (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomField">
       array[CustomField]
      </a>
     </span>
    </div>
    <div class="param">
     custom_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomUrl">
       CustomUrl
      </a>
     </span>
    </div>
    <div class="param">
     bulk_pricing_rules (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#BulkPricingRule">
       array[BulkPricingRule]
      </a>
     </span>
    </div>
    <div class="param">
     variants (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#VariantPost">
       array[VariantPost]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductPut">
     ProductPut -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the product, increments sequentially.
    </div>
    <div class="param">
     name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product name.
    </div>
    <div class="param">
     type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product type: physical - a physical stock unit, digital - a digital download
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     physical
    </div>
    <div class="param-enum">
     digital
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     User defined product code/stock keeping unit (SKU).
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product description which can include HTML formatting.
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Weight of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     width (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Width of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     depth (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Depth of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     height (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     Height of the product used which can be used when calculating shipping costs.
 format: double
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The price of the product, the price should include or exclude tax based on the store settings.
 format: double
    </div>
    <div class="param">
     cost_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The cost price of the product, stored for reference only, it is not used or displayed anywhere on the store.
 format: double
    </div>
    <div class="param">
     retail_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The retail cost of the product, if entered the retail cost price will be shown on the product page.
 format: double
    </div>
    <div class="param">
     sale_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The sale price will be used instead of value in the price field when calculating the products cost if entered.
 format: double
    </div>
    <div class="param">
     tax_class_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The ID of the tax class applied to the product. NOTE: Value ignored if automatic tax is enabled.
    </div>
    <div class="param">
     product_tax_code (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Accepts AvaTax system codes that identify products and services that fall into special sales tax categories. Allows merchants that subscribe to Avalara Premium to achieve increased accuracy in sales tax calculations. Stores without Avalara Premium will ignore the code when calculating sales tax. Do not pass more than one code. The codes are case-sensitive. Refer to the 'AvaTax System tax codes' section of the following page for further information and the full list of codes: https://help.avalara.com/000_AvaTax_Calc/000AvaTaxCalc_User_Guide/040_Managing_Tax_Profiles/050_Tax_Codes/001_What_is_a_Tax_Code
    </div>
    <div class="param">
     calculated_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The price of the product unless a sale_price is set.
 format: double
    </div>
    <div class="param">
     categories (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       array[Integer]
      </a>
     </span>
     An array of IDs for the categories this product belongs to. When updating a product, if an array of categories is supplied all product categories will be overwritten. Does not accept more than 1,000 ID values.
    </div>
    <div class="param">
     brand_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The id associated with the product's brand.
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Current inventory level of the product. Simple inventory tracking must be enabled (See the inventory_tracking field) for this to take any effect.
    </div>
    <div class="param">
     inventory_warning_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Inventory Warning level for the product. When the products inventory level drops below the warning level the store owner will be informed. Simple inventory tracking must be enabled (See the inventory_tracking field) for this to take any effect.
    </div>
    <div class="param">
     inventory_tracking (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The type of inventory tracking for the product: none - inventory levels will not be tracked. product - inventory levels will be tracked using the 'inventory_level' and 'inventory_warning_level' fields. variant - inventory levels will be tracked based on  variants which maintain their own warning levels and inventory levels.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     product
    </div>
    <div class="param-enum">
     variant
    </div>
    <div class="param">
     fixed_cost_shipping_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     A fixed shipping cost for the product, if defined the value will be used during checkout instead of normal shipping cost calculation.
    </div>
    <div class="param">
     is_free_shipping (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag used to indicate if the product has free shipping or not. If true the shipping cost for the product will be zero.
    </div>
    <div class="param">
     is_visible (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be displayed to customers browsing the store or not. If true the product will be displayed, false the product will be hidden from view.
    </div>
    <div class="param">
     is_featured (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag to determine if the product should be included in 'featured products' panel when viewing the store.
    </div>
    <div class="param">
     warranty (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Warranty information displayed on the product page which can include HTML formatting.
    </div>
    <div class="param">
     bin_picking_number (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The BIN picking number for the product.
    </div>
    <div class="param">
     layout_file (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The layout template file used to render this product.
    </div>
    <div class="param">
     upc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product UPC code which is used in feeds for shopping comparison sites and external channel integrations.
    </div>
    <div class="param">
     search_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A comma separated list of keywords that can be used to locate the product when searching the store.
    </div>
    <div class="param">
     availability (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Availability of the product. availability options: available - The product can be purchased in the store front. disabled - The product is listed in the store front but can not be purchased. preorder - The product is listed for pre-orders.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     available
    </div>
    <div class="param-enum">
     disabled
    </div>
    <div class="param-enum">
     preorder
    </div>
    <div class="param">
     availability_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Availability text displayed on the checkout page under the product title telling the customer how long it will normally take to ship this product, such as 'Usually ships in 24 hours'.
    </div>
    <div class="param">
     gift_wrapping_options_type (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     `any` - allow any gift wrapping options in the store, `none` - disallow gift wrapping on the product. When the type is set to `list`, a list of ids in gift_wrapping_options_list field should be provided.
    </div>
    <div class="param-enum-header">
     Enum:
    </div>
    <div class="param-enum">
     any
    </div>
    <div class="param-enum">
     none
    </div>
    <div class="param-enum">
     list
    </div>
    <div class="param">
     gift_wrapping_options_list (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       array[Integer]
      </a>
     </span>
     A list of gift wrapping option ids.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Priority this product will be given when included in product lists on category pages and search results. The lower the number, the closer to the top of the results the product will be.
    </div>
    <div class="param">
     condition (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The product condition, will be shown on the product page if the value of the 'is_condition_shown' field is true. Possible values: New, Used, Refurbished
    </div>
    <div class="param">
     is_condition_shown (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     Flag used to determine if the product condition is shown to the customer on the product page.
    </div>
    <div class="param">
     order_quantity_minimum (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The minimum quantity an order has to contain to be able to purchase this product.
    </div>
    <div class="param">
     order_quantity_maximum (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The maximum quantity an order can contain when purchasing the product.
    </div>
    <div class="param">
     page_title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom title for the products page, if not defined the product name will be used as the meta title.
    </div>
    <div class="param">
     meta_keywords (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       array[String]
      </a>
     </span>
     Custom meta keywords for the product page, if not defined the store default keywords will be used.
    </div>
    <div class="param">
     meta_description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom meta description for the product page, if not defined the store default meta description will be used.
    </div>
    <div class="param">
     date_created (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the product was created.
 format: data-time
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the product was created.
 format: data-time
    </div>
    <div class="param">
     view_count (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The number of times the product has been viewed.
    </div>
    <div class="param">
     preorder_release_date (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Pre-order release date. See availability field for details on setting a products availability to accept pre-orders.
 format: data-time
    </div>
    <div class="param">
     preorder_message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Custom expected date message to display on the product page, if undefined the message defaults to the store wide setting. Can contain the %%DATE%% place holder which will be substituted for the release date
    </div>
    <div class="param">
     is_preorder_only (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     If set to false, the product will not change its availability from preorder to available on the release date. Otherwise on the release date the products availability/status will change to available.
    </div>
    <div class="param">
     is_price_hidden (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     False by default, which indicates that the price of this product should be shown on the product page. If set to 'true', the price is hidden. NOTE: To successfully set 'is_price_hidden' to 'true', the 'availability' value must be 'disabled'.
    </div>
    <div class="param">
     price_hidden_label (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     By default, an empty string. If 'is_price_hidden' is 'true', the value of 'price_hidden_label' is displayed instead of the price. NOTE: To successfully set a non-empty string value for 'is_price_hidden' to 'true', the 'availability' value must be 'disabled'.
    </div>
    <div class="param">
     images (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductImage">
       array[ProductImage]
      </a>
     </span>
    </div>
    <div class="param">
     videos (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductVideo">
       array[ProductVideo]
      </a>
     </span>
    </div>
    <div class="param">
     custom_fields (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomField">
       array[CustomField]
      </a>
     </span>
    </div>
    <div class="param">
     custom_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CustomUrl">
       CustomUrl
      </a>
     </span>
    </div>
    <div class="param">
     bulk_pricing_rules (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#BulkPricingRule">
       array[BulkPricingRule]
      </a>
     </span>
    </div>
    <div class="param">
     variants (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Variant">
       array[Variant]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductResponse">
     ProductResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Product">
       Product
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductVideo">
     ProductVideo -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    An product video model.
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The ID of a Youtube video.
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical identifier for the product that the image is associated with.
    </div>
    <div class="param">
     sort_order (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The order in which the video will be displayed on the product page. When updating if the video is given a lower priority, all video with a sort_order the same or greater than the videos new sort_order value will have their sort_order reordered
    </div>
    <div class="param">
     description (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The description for the video. If left blank, this will be filled in according to data on Youtube.
    </div>
    <div class="param">
     title (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The title for the video. If left blank, this will be filled in according to data on Youtube.
    </div>
    <div class="param">
     length (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     length of video. This will be filled in according to data on Youtube.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductVideoCollectionResponse">
     ProductVideoCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductVideo">
       array[ProductVideo]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ProductVideoResponse">
     ProductVideoResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#ProductVideo">
       ProductVideo
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="ResourceImage">
     ResourceImage -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    An object containing a publically accessible image URL or a form post that contains an image file.
   </div>
   <div class="field-items">
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     A public URL for a GIF, JPEG, or PNG image.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Subscriber">
     Subscriber -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The unique numerical ID of the subscriber, increments sequentially.
    </div>
    <div class="param">
     email (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The email of the subscriber. Must be unique
    </div>
    <div class="param">
     first_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The first name of the subscriber.
    </div>
    <div class="param">
     last_name (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The last name of the subscriber.
    </div>
    <div class="param">
     source (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The source of the subscriber, storefront, order, or custom.
    </div>
    <div class="param">
     order_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     The id of the source order, if source was an order.
    </div>
    <div class="param">
     date_modified (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the subscriber was modified.
 format: data-time
    </div>
    <div class="param">
     date_created (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The date of which the subscriber was created.
 format: data-time
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="SubscriberCollectionResponse">
     SubscriberCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Subscriber">
       array[Subscriber]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="SubscriberResponse">
     SubscriberResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Subscriber">
       Subscriber
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="Variant">
     Variant -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
    <div class="param">
     sku_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     read-only reference to V2 sku id, null if it's a base variant
    </div>
    <div class="param">
     cost_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     The cost price of the variant. format: double
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     This variant's base price on the storefront. If this value is null, the product's default price (set in the Product resource's price field) will be used as the base price. format: double
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#double">
       Double
      </a>
     </span>
     This variant's base weight on the storefront. If this value is null, the product's default weight (set in the Product resource's weight field) will be used as the base weight. format: double
    </div>
    <div class="param">
     purchasing_disabled (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     If true, this variant will not be purchasable on the storefront
    </div>
    <div class="param">
     purchasing_disabled_message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     If purchasing_disabled is true, this message should show on the storefront when the variant is selected
    </div>
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The image that will be displayed when this variant is selected on the storefront. When updating a SKU image, send the publicly accessible URL. Supported image formats are JPEG, PNG, and GIF. Generic product images not specific to the variant should be stored on the product.
    </div>
    <div class="param">
     upc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The UPC code which is used in feeds for shopping comparison sites and external channel integrations.
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Inventory level for the variant, which is used when the product's inventory_tracking is set to variant
    </div>
    <div class="param">
     inventory_warning_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     When the variant hits this inventory level it is considered low stock
    </div>
    <div class="param">
     bin_picking_number (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Identifies where in a warehouse the variant is located.
    </div>
    <div class="param">
     option_values (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#OptionValueShort">
       array[OptionValueShort]
      </a>
     </span>
     Array of option and option values ids that make up this variant. Will be empty if the variant is the product's base variant.
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="VariantCollectionResponse">
     VariantCollectionResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Response payload for the Bigcommerce API
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Variant">
       array[Variant]
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#CollectionMeta">
       CollectionMeta
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="VariantPost">
     VariantPost -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
   </div>
   <div class="field-items">
    <div class="param">
     id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
    </div>
    <div class="param">
     product_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
    </div>
    <div class="param">
     sku (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
    </div>
    <div class="param">
     sku_id (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     read-only reference to V2 sku id, null if it's a base variant
    </div>
    <div class="param">
     price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     This variant's base price on the storefront. If this value is null, the product's default price (set in the Product resource's price field) will be used as the base price.
    </div>
    <div class="param">
     weight (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     This variant's base weight on the storefront. If this value is null, the product's default weight (set in the Product resource's weight field) will be used as the base weight.
    </div>
    <div class="param">
     purchasing_disabled (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#boolean">
       Boolean
      </a>
     </span>
     If true, this variant will not be purchasable on the storefront
    </div>
    <div class="param">
     purchasing_disabled_message (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     If purchasing_disabled is true, this message should show on the storefront when the variant is selected
    </div>
    <div class="param">
     image_url (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The image that will be displayed when this variant is selected on the storefront. When updating a SKU image, send the publicly accessible URL. Supported image formats are JPEG, PNG, and GIF. Generic product images not specific to the variant should be stored on the product.
    </div>
    <div class="param">
     cost_price (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The variant's cost price
    </div>
    <div class="param">
     upc (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     The UPC code which is used in feeds for shopping comparison sites and external channel integrations
    </div>
    <div class="param">
     inventory_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     Inventory level for the variant, which is used when the product's inventory_tracking is set to variant
    </div>
    <div class="param">
     inventory_warning_level (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#integer">
       Integer
      </a>
     </span>
     When the variant hits this inventory level it is considered low stock
    </div>
    <div class="param">
     bin_picking_number (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#string">
       String
      </a>
     </span>
     Identifies where in a warehouse the variant is located.
    </div>
    <div class="param">
     option_values (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#OptionValueShortPost">
       array[OptionValueShortPost]
      </a>
     </span>
    </div>
   </div>
  </div>
  <div class="model">
   <h3 class="field-label">
    <a name="VariantResponse">
     VariantResponse -
    </a>
    <a class="up" href="#__Models">
     Up
    </a>
   </h3>
   <div class="model-description">
    Successful response
   </div>
   <div class="field-items">
    <div class="param">
     data (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Variant">
       Variant
      </a>
     </span>
    </div>
    <div class="param">
     meta (optional)
    </div>
    <div class="param-desc">
     <span class="param-type">
      <a href="#Meta">
       Meta
      </a>
     </span>
    </div>
   </div>
  </div>
 </body>
</html>
