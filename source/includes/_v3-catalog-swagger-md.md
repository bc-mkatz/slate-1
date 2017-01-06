BigCommerce Catalog API (partial swagger-md conversion)
=======================
A Swagger Document for the BigCommmerce API V3.

**Version:** 3.0.0b

**Terms of service:**  
http://www.bigcommerce.com/terms

### /catalog/products
---
##### ***GET***
**Description:** Returns a paginated collection of `Products` objects from the BigCommerce Catalog.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
| sort | query | Field name to sort by. Values: id, name, sku, price, date_modified, date_last_imported, inventory_level, is_visible.  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of products and meta data  |

##### ***POST***
**Description:** Creates a `Product` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product | body | A BigCommerce `Product` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product  |
| 409 | `Product` was in conflict with another product. This is the result of duplicate unique values such as name or SKU; a missing or invalid category id, brand id, or tax_class id; or a conflicting `bulk_pricing_rule`.  |
| 422 | `Product` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Deletes one or more `Product` objects from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}
---
##### ***GET***
**Description:** Returns a `Product` from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Updates a `Product` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| product | body | A BigCommerce `Product` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product  |
| 404 | The resource was not found  |
| 409 | `Product` was in conflict with another product. This is the result of duplicate unique values such as name or SKU, a missing category, brand, or tax_class that the product is being associate to, or a conflicting bulk pricing rule.  |
| 422 | `Product` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Deletes a `Product` object from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}/images
---
##### ***GET***
**Description:** Gets all images on a product. 


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the image is being attached to.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | List of product images and meta  |

##### ***POST***
**Description:** Creates an image on a product. Publically accessible URLs and files (form post) are valid parameters.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the image is being attached to.  | Yes | integer |
| productImage | body | A BigCommerce `ProductImage` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product image  |
| 404 | The resource was not found  |

### /catalog/products/{product_id}/images/{image_id}
---
##### ***GET***
**Description:** Gets image on a product. 


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the image is being attached to.  | Yes | integer |
| image_id | path | The id of the `Image` the image is being operated on.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of product images and meta data  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Updates an image on a product. Publically accessible URLs and files (form post) are valid parameters.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the image is being attached to.  | Yes | integer |
| image_id | path | The id of the `Image` the image is being operated on.  | Yes | integer |
| productImage | body | A BigCommerce `ProductImage` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product image  |
| 404 | The resource was not found  |

##### ***DELETE***
**Description:** Delete a `ProductImage` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the image is being attached to.  | Yes | integer |
| image_id | path | The id of the `Image` the image is being operated on.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}/videos
---
##### ***GET***
**Description:** Gets all videos on a product.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the video is being attached to.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | List of product videos and meta  |

##### ***POST***
**Description:** Creates an video on a product using a video ID from Youtube


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the video is being attached to.  | Yes | integer |
| productVideo | body | A BigCommerce `ProductVideo` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product video  |
| 404 | The resource was not found  |

### /catalog/products/{product_id}/videos/{video_id}
---
##### ***GET***
**Description:** Gets video on a product.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the video is being attached to.  | Yes | integer |
| video_id | path | The id of the `Video` the video is being operated on.  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of product videos and meta data  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Updates an video on a product.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the video is being attached to.  | Yes | integer |
| video_id | path | The id of the `Video` the video is being operated on.  | Yes | string |
| productVideo | body | A BigCommerce `ProductVideo` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A product video  |
| 404 | The resource was not found  |

##### ***DELETE***
**Description:** Delete a `ProductVideo` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the video is being attached to.  | Yes | integer |
| video_id | path | The id of the `Video` the video is being operated on.  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}/variants
---
##### ***GET***
**Description:** Returns a `Variant` object list from the BigCommerce Catalog.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of variants and meta data  |
| 404 | The resource was not found  |

##### ***POST***
**Description:** Create a `Variant` object.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| Variant | body | `Variant` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A variant and meta data  |
| 404 | The resource was not found  |

### /catalog/products/{product_id}/variants/{variant_id}
---
##### ***GET***
**Description:** Get a `Variant` object.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| variant_id | path | The id of the `Variant`.  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A variant and meta data  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Update a `Variant` object.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| variant_id | path | The id of the `Variant`.  | Yes | number (int) |
| Variant | body | `Variant` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A variant and meta data  |
| 404 | The resource was not found  |

##### ***DELETE***
**Description:** Delete a `Variant`


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| variant_id | path | The id of the `Variant`.  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}/variants/{variant_id}/image
---
##### ***POST***
**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| variant_id | path | The id of the `Variant`.  | Yes | number (int) |
| image_file | formData | An image file. Support MIME types include GIF, JPEG, and PNG.  | Yes | file |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A ResourceImage and meta data  |
| 404 | The resource was not found  |
| 422 | Image was not valid. This is the result of missing image_file field or incorrect file type. See the response for more details.  |

### /catalog/products/{product_id}/options
---
##### ***GET***
**Description:** Get an array of `Option` objects.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of options and meta data  |
| 404 | The resource was not found  |

##### ***POST***
**Description:** Create an `Option`.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
| Option | body | `Option` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An option object  |
| 409 | Option was in conflict with another option. This is the result of duplicate unique fields such as name.  |
| 422 | Option was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

### /catalog/products/{product_id}/options/{option_id}
---
##### ***GET***
**Description:** Gets `Option` object by product id and option id.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Option` belongs to.  | Yes | number (int) |
| option_id | path | The id of the `Option`.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A Option object  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Update a Product's `Option` based on the product_id and option_id.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Option` belongs to.  | Yes | number (int) |
| option_id | path | The id of the `Option`.  | Yes | integer |
| option | body | A BigCommerce `Option` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An option object  |
| 409 | The `Option` was in conflict with another option. This is the result of duplicate unique fields such as name.  |
| 422 | The `Option` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a Product's `Option` based on the product_id and option_id.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Option` belongs to.  | Yes | number (int) |
| option_id | path | The id of the `Option`.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}/modifiers
---
##### ***GET***
**Description:** Get an array of `Modifier` objects.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of modifiers and meta data  |

##### ***POST***
**Description:** Create a `Modifier`.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |
| Modifier | body | `Modifier` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A modifier object  |
| 409 | The `Modifier` was in conflict with another option. This is the result of duplicate unique fields such as name.  |
| 422 | The `Modifier` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

### /catalog/products/{product_id}/modifiers/{modifier_id}
---
##### ***GET***
**Description:** Get a `Modifier` by product_id and modifier_id


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |
| modifier_id | path | The id of the `Modifier`  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A modifier object  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Update an Product's `Modifier` based on the product_id and modifier_id.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |
| modifier_id | path | The id of the `Modifier`  | Yes | integer |
| modifier | body | A BigCommerce `Modifier` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A modifier object  |
| 409 | The `Modifier` was in conflict with another modifier or option. This is the result of duplicate unique fields such as name.  |
| 422 | The `Modifier` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a Product's `Modifier` based on the product_id and modifier_id.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |
| modifier_id | path | The id of the `Modifier`  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/products/{product_id}/modifiers/{modifier_id}/values/{value_id}/image
---
##### ***POST***
**Description:** Add an image to a modifier value that will show on the storefront when it’s selected

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |
| modifier_id | path | The id of the `Modifier`  | Yes | integer |
| value_id | path | The id of the `Modifier`  | Yes | integer |
| image_file | formData | An image file. Support MIME types include GIF, JPEG, and PNG.  | Yes | file |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A ResourceImage and meta data  |
| 404 | The resource was not found  |
| 422 | Modifier image was not valid. This is the result of missing image_file fields or non-url for image_file field. See the response for more details.  |

##### ***DELETE***
**Description:** Delete the image applied to show when the modifier value is selected

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| product_id | path | The id of the `Product` the `Modifier` belongs to.  | Yes | number (int) |
| modifier_id | path | The id of the `Modifier`  | Yes | integer |
| value_id | path | The id of the `Modifier`  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | Image cleared for the modifier value |

### /catalog/categories
---
##### ***GET***
**Description:** Returns a paginated categories collection from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array category objects and meta data  |

##### ***POST***
**Description:** Creates a `Category` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| category | body | A BigCommerce `Category` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A category object  |
| 409 | The `Category` was in conflict with another category. This is the result of duplicate unique values such as name or custom_url.  |
| 422 | The `Category` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a product or products from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/categories/{category_id}
---
##### ***GET***
**Description:** Returns a `Category` from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| category_id | path | The id of the `Category` requested  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A category object  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Update a `Category` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| category_id | path | The id of the `Category` requested  | Yes | integer |
| category | body | A BigCommerce `Category` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A category object  |
| 404 | The resource was not found  |
| 409 | The `Category` was in conflict with another category. This is the result of duplicate unique values such as name or custom_url.  |
| 422 | The `Category` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete one or more `Category` objects from the BigCommerce catalog.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| category_id | path | The id of the `Category` requested  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/categories/{category_id}/image
---
##### ***POST***
**Description:** Creates an image on a category. Publically accessible URLs and files (form post) are valid parameters.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| category_id | path | The id of the `Category` the image is being attached to.  | Yes | integer |
| image_file | formData | An image file. Support MIME types include GIF, JPEG, and PNG.  | Yes | file |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A ResourceImage and meta data  |
| 404 | The resource was not found  |
| 422 | Image was not valid. This is the result of missing image_file field or incorrect file type. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a `Category` image the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| category_id | path | The id of the `Category` the image is being attached to.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/categories/tree
---
##### ***GET***
**Description:** Returns the categories tree, a nested lineage of the categories with parent->child relationship. The `Category` objects returned are a simplified version of the category objects returned in the rest of this API.


**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A array of nested category tree objects and meta data  |

### /catalog/brands
---
##### ***GET***
**Description:** Gets `Brand` objects.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of brand objects and meta  |

##### ***POST***
**Description:** Create a `Brand` object.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Brand | body | `Brand` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A brand object  |
| 409 | Brand was in conflict with another brand. This is the result of duplicate unique fields such as name.  |
| 422 | Brand was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete one or more `Brand` objects from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/brands/{brand_id}
---
##### ***GET***
**Description:** Gets `Brand` object.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| brand_id | path | The id of the `Brand` requested  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A brand object  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Update a `Brand` in the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| brand_id | path | The id of the `Brand` requested  | Yes | number (int) |
| brand | body | Returns a `Brand` from the BigCommerce Catalog  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A brand object  |
| 404 | The resource was not found  |
| 409 | The `Brand` was in conflict with another product. This is the result of duplicate unique value such as name  |
| 422 | The `Brand` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a `Brand` from the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| brand_id | path | The id of the `Brand` requested  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /catalog/brands/{brand_id}/image
---
##### ***POST***
**Description:** Creates an image on a `Brand`. Publically accessible URLs and files (form post) are valid parameters.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| brand_id | path | The id of the `Brand` the image is being attached to.  | Yes | integer |
| image_file | formData | An image file. Support MIME types include GIF, JPEG, and PNG.  | Yes | file |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A ResourceImage and meta data  |
| 404 | The resource was not found  |
| 422 | Image was not valid. This is the result of missing image_file field or incorrect file type. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a `Brand` image the BigCommerce Catalog


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| brand_id | path | The id of the `Brand` the image is being attached to.  | Yes | integer |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | Image cleared for the brand |

### /catalog/products/variants
---
##### ***GET***
**Description:** Returns a `Variant` object list from the BigCommerce Catalog.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of variants and meta data  |
| 404 | The resource was not found  |

### /catalog/summary
---
##### ***GET***
**Description:** Returns a lightweight inventory summary from the BigCommerce Catalog.


**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of catalog summary and meta data  |

### /customers/subscribers
---
##### ***GET***
**Description:** Returns a paginated Subscribers collection.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | An array of subscriber objects and meta data  |

##### ***POST***
**Description:** Creates a `Subscriber` object.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| subscriber | body | `Subscriber` object  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A Subscriber object  |
| 409 | The `Subscriber` was in conflict with another subscriber. This is the result of duplicate unique values such as email  |
| 422 | The `Subscriber` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a subscriber or subscribers from BigCommerce Customers.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |
|  |  |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |

### /customers/subscribers/{subscriber_id}
---
##### ***GET***
**Description:** Gets `Subscriber` object.

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| subscriber_id | path | The id of the `Subscriber` requested.  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A Subscriber object  |
| 404 | The resource was not found  |

##### ***PUT***
**Description:** Update a `Subscriber` object.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| subscriber_id | path | The id of the `Subscriber` requested.  | Yes | number (int) |
| subscriber | body | Returns a `Subscriber` object.  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | A Subscriber object  |
| 404 | The resource was not found  |
| 409 | The `Subscriber` was in conflict with another subscriber. This is the result of duplicate unique value such as email  |
| 422 | The `Subscriber` was not valid. This is the result of missing required fields or invalid data. See the response for more details.  |

##### ***DELETE***
**Description:** Delete a `Subscriber` object.


**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| subscriber_id | path | The id of the `Subscriber` requested.  | Yes | number (int) |

**Responses**

| Code | Description |
| ---- | ----------- |
| 204 | An empty response  |
