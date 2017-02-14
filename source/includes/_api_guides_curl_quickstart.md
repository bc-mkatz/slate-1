# <span class="jumptarget" id="curl_quickstart"> cURL Quickstart Guide </span>

This section provides some sample cURL commands, for quickstart purposes. These use Basic Authentication, so before you can issue these commands, you must generate Basic Authentication credentials by following the steps discussed [here](/api#pvt_token). Once you have your Basic Authentication credentials, you can issue cURL commands as listed below.

```
    curl --request GET \
    -H "Authorization: Basic _username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/time
```

If the request is made using the `Authorization` header, you need to encode the credentials using base64. Or, a simple way to accomplish the same task as above is:

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/orders.json
```

## <span class="jumptarget"> Orders cURL Commands </span>

Here are sample cURL commands to handle orders.

### <span class="jumptarget"> Get a List of Orders from the Store</span>

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/orders.json
```

By default, the API request returns only 50 orders. If you want to return all the orders from the store, you must use filters, as shown in the next example below.

### <span class="jumptarget"> Get All Orders from the Store</span>

Use the `limit` and `page` filter parameters to get a data beyond what the default query returns. Note that 200 orders is the maximum returned per page:

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/orders.json?limit=200&page=1
```

### <span class="jumptarget"> Update an Order</span>

Orders take many fields upon update requests. (For details, please see <a href="/api/v2/#update-an-order" target="_blank">this documentation</a>.) Here, we update an order using just the mandatory fields:

```
    curl --request PUT \
    -u "_username_:_API_key_" \
    -H "Content-Type: application/json" \
    --data-binary '{"status_id":1}' \
    https://store.mybigcommerce.com/api/v2/orders/101
```


### <span class="jumptarget"> Get Orders Created since a Certain Date</span>

You can use the `If-Modified-Since` header to request orders that have been created after a given date:

```    
    curl -I --request GET \
    -u "_username_:_API_key_" \
    -H "Content-Type: application/json" \
    -H "If-Modified-Since: Tue, 4 Dec 2012 00:00:00 GMT" \
    https://store.mybigcommerce.com/api/v2/orders.json
```

### <span class="jumptarget"> Get Coupons Associated with an Order</span>

An order can contain coupons, which might be applied to the order to offer discounts to the customer. You can look at all the available coupons in an order as follows:

```
    curl --request GET \
    -u "_username_:_API_key_"\
    https://store.mybigcommerce.com/api/v2/orders/115/coupons.json
```

### <span class="jumptarget"> Create a Shipment for an Order</span>

You can create a shipment for an order via the <a href="/api/v2/#create-a-shipment" target="_blank">Orders &gt; Create a Shipment</a> endpoint. As an example, third-party shipping services can query orders from a store when the orders are created, and create shipments for those:

```
    curl --request POST \
    -u "_username_:_API_key_" \
    -H "Content-Type: application/json" \
    -d '{"order_address_id":15,"tracking_number":"123-123-123","items":[{"order_product_id":15,"quantity":1}]}' \
    https://store.mybigcommerce.com/api/v2/orders/114/shipments.json
```

## <span class="jumptarget"> Products cURL Commands </span>

Here are sample cURL commands to handle products.

#### <span class="jumptarget"> Get a List of Products from the Store </span>

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/products.json
```

By default, the API request returns only 50 products. If you want to return all the products from the store, you must use filters, as shown in the example below.

#### <span class="jumptarget"> Get All Products from the Store </span>

Use the `limit` and `page` filter parameters to get data beyond what the default query returns. Note that a maximum of 200 products are returned per page:

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/products.json?limit=200&page=1
```

#### <span class="jumptarget"> Create a Product </span>

Products have many fields. For details on the product fields allowed as part of a `POST` request, please see <a href="/api/v2/#create-a-product" target="_blank">this page</a>.

Let's assume that we want to create a product using only the fields that are for a `POST` request. Here, `price` must specified as a string, while `weight` is a decimal. The `is_visible` flag is not mandatory, but if it is not set to `true`, the product would not be visible by default:

```
    curl --request POST \
    -H "Content-Type: application/json" \
    -u "_username_:_API_key_" \
    -d '{"name":"startrek","price":19.99,"categories":[2],"type":"physical","availability":"available", "weight":0}' \
    https://store.mybigcommerce.com/api/v2/products.json
```

### <span class="jumptarget"> Update a Product </span>

To update the product created above, you could use the following:

```
    curl --request PUT \
    -H "Content-Type: application/json" \
    -u "_username_:_API_key_" \
    -d '{"name":"startrek","sku":"STREK-DVD","categories":[2,3],"inventory_tracking":"simple","inventory_level":"500", "inventory_warning":100}' \
    https://store.mybigcommerce.com/api/v2/products/id.json
```

### <span class="jumptarget"> Search a Product by SKU </span>

To search by a product SKU, we could use the following code. Remember that when a product has optionset/variations defined, and if the individual options have SKUs defined, then the product SKU is overriden by the option SKUs. Currently, there are two ways to search for SKUs: `GET /products?sku="something"` or `GET /products/skus?sku="something"`. The first call returns only product-level SKUs and not option-level SKUs.

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/products/skus.json?sku="abcd"
```

## <span class="jumptarget"> Coupons cURL Commands </span>

Here are sample cURL commands to handle coupons.

### <span class="jumptarget"> Get a List of Coupons from the Store </span>

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/coupons.json
```

Coupons can be filtered by `code`, `type`, `name`, `min_id` and `max_id`. Without these filters, the call returns all the coupons in the store. So for example, if we wanted to return a list of only those coupons of `type=percentage_discount`, we could make the following request:

```
    curl --request GET \
    -u "_username_:_API_key_" \
    https://store.mybigcommerce.com/api/v2/coupons.json?type=percentage_discount
```

For details on filter fields, please see the <a href="/api/v2#coupons" target="_blank">Coupons resource</a>.

#### <span class="jumptarget"> Create a Coupon </span>

Coupons can be created by a `POST` request on the coupons endpoint. For example, if we want to create a coupon to take 50% off an order, then our coupon will have `percentage_discount` as the type. The `applies_to` field is optional, and can be used to restrict the coupon to a set of products or categories. In the example shown below, the coupon is being restricted to a set of products:

```
    curl --request POST \
    -H "Content-Type: application/json" \
    -u "_username_:_API_key_" \
    -d '{"code":"50OFF", "type":"percentage_discount", "name":"testcoupon1", "amount":50.00, "enabled":"true", "applies_to":"{\"entity\":\"products\",\"ids\":[32]}"}' \
    https://store.mybigcommerce.com/api/v2/coupons.json
```

#### <span class="jumptarget"> Update a Coupon </span>

Updating a coupon is almost similar to the Create example above, except that we work off an ID via a `PUT` request. For example, assume that we want to change the above coupon from a 50% to a 30% discount, and that the coupon ID is `15`. We can update the coupon using the following:

```
    curl --request PUT \
    -H "Content-Type: application/json" \
    -u "_username_:_API_key_" \
    -d '{"code":"30OFF", "type":"percentage_discount"' \
    https://store.mybigcommerce.com/api/v2/coupons/15.json
```

## <span class="jumptarget"> Option Sets cURL Commands </span>

Here are sample cURL commands to handle option sets.

### <span class="jumptarget"> Connect Options to Option Sets </span>

This is currently a four-step process.

1.  Create the option.
2.  Add some values to the option.
3.  Create the option set.
4.  Create option-set options, using the options you just created.

Use the following command to create an option:

```
    curl --request POST \
    -H "Content-Type: application/json" \
    -u "_username_:_API_key_" \
    -d '{"name":"homer simpson", "type":"T"}' \
    https://store.mybigcommerce.com/api/v2/options.json
```

BigCommerce returns the following, which includes an option ID:

```
{"id":33,"name":"homer simpson","display_name":"homer simpson","type":"T","values":{"url":"https://store.mybigcommerce.com-bwvr466.mybigcommerce.com/api/v2/options/33/values.json","resource":"/options/33/values"}}
```

Next, create a new option set:

```
    curl --request POST \
    -u "admin:key" \
    -d '{"name": "Simpson family"}' \
    -H "Content-Type: application/json" \
    https://store.mybigcommerce.com/api/v2/optionsets.json
```

The API returns the following, which includes an option-set ID:

```
{"id":27,"name":"Simpson family","options":{"url":"https://store.mybigcommerce.com-bwvr466.mybigcommerce.com/api/v2/optionsets/27/options.json","resource":"/optionsets/27/options"}}
```

The final step is to connect the option with the option set:

```
    curl --request POST \
    -u "_username_:_API_key_" \
    -d '{"option_id": "33", "display_name":"Simpson family"}' \
    -H "Content-Type: application/json" \
    https://store.mybigcommerce.com/api/v2/optionsets/27/options.json
```

Which yields the following:

```
{"id":44,"option_id":33,"option_set_id":27,"display_name":"Simpson family","sort_order":0,"is_required":false,"option":{"url":"https://store.mybigcommerce.com-bwvr466.mybigcommerce.com/api/v2/options/33.json","resource":"/options/33"}}
```
