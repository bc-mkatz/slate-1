<!-- Gnarly links are reset; reset the easy ones. Link from "Create an Order" endpoint. Stuff this into docs tree below Orders endpoints – between "Delete All Orders" and "Order Coupons". -->

## <span class="jumptarget"> Order Products Array </span>

|||
|---|---|
| Managed by | [Orders Resource](#orders)

Nested inside the <a href="/api/objects/v2/#orders">`order`</a> object, the `products` object/array allows you to achieve several goals:

* When retrieving order(s) using a `GET`, the `products` array provides JSON and XML summaries of the product(s) in the order. For an example of the syntax, see the sample code in [List Orders](#list-orders).

* When sending order(s) using a `POST` or `PUT`, the `products` array allows you to add either a product that already exists in the store, or a product that does not exist in the store. For an example of the syntax, see the sample code in [Create an Order](#create-an-order).

<aside class="warning">
<span class="aside-warning-hd">Updates Are Additive</span><br><br>
Values passed for the <code>products</code> array to a <code>PUT</code> are appended to any existing values. You cannot use a <code>PUT</code> to overwrite existing <code>products</code> values.
</aside>

### <span class="jumptarget"> Retrieving Product Information using GET </span>

<table>
<thead>
  <tr>
    <th>Name</th>
    <th>Type</th>
    <th>Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>url</td>
    <td>string</td>
    <td>The URI of a JSON object containing the product details.</td>
  </tr>
  <tr>
    <td>resource</td>
    <td>string</td>
    <td>A context path that provides an alternate means of retrieving the data (for example, if you prefer XML).</td>
  </tr>
 </tbody>
</table>


### <span class="jumptarget"> Adding an Existing Product (that Already Exists in the Store) to the Order </span>

<table>
<thead>
  <tr>
    <th>Name</th>
    <th>Type</th>
    <th>Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>product_id</td>
    <td>int</td>
    <td>The ID of the product that you want to add to the order (required).</td>
  </tr>
  <tr>
    <td>quantity</td>
    <td>int</td>
    <td>How many products of this type to add to the order (required).</td>
  </tr>
  <tr>
    <td>product_options</td>
    <td>array</td>
    <td>These values might be required, depending on how the product's options are set up. If the options are required, pass in the <a href="#options-object-properties"><code>id</code></a> of the product option (not the option itself) and the <a href="#option-value-object-properties"><code>value</code></a>  of the option (not the product).</td>
  </tr>
  <tr>
    <td>price_inc_tax</td>
    <td>int</td>
    <td>If you include a value here, it will overwrite the price (including tax) already specified for the product. This property is optional, but if you do include a value for <code>price_inc_tax</code>, you must also include a value for <code>price_ex_tax</code>.</td>
  </tr>
  <tr>
    <td>price_ex_tax</td>
    <td>int</td>
    <td>If you include a value here, it will overwrite the price (excluding tax) already specified for the product. This property is optional, but if you do include a value for <code>price_ex_tax</code>, you must also include a value for <code>price_inc_tax</code>.</td>
  </tr>
 </tbody>
</table>


### <span class="jumptarget" id="custom-product"> Adding a New Product (that Does Not Already Exist in the Store) to the Order </span>
<table>
  <thead>
   <tr>
     <th style="width: 100px;">Name</th>
     <th style="width: 50px;">Type</th>
     <th>Description</th>
   </tr>
  </thead>
  <tbody>
    <tr class="mandatory">
        <td>name</td>
        <td>int</td>
        <td>The name of the custom product tax. (Required.)</td>
    </tr>
    <tr class="mandatory">
        <td>quantity</td>
        <td>int</td>
        <td>The quantity of the purchase for this custom product tax. (Required. Can be positive or negative. Cannot be zero.)</td>
    </tr>
    <tr class="mandatory">
        <td>price_inc_tax</td>
        <td>decimal</td>
        <td>The price of the custom product, including tax. (Required.)</td>
    </tr>
    <tr class="mandatory">
        <td>price_ex_tax</td>
        <td>decimal</td>
        <td>The price of the custom product, excluding tax. (Required.)</td>
    </tr>
    <tr>
        <td>sku</td>
        <td>text</td>
        <td>The SKU of the custom product. (Optional.)</td>
    </tr>
  </tbody>
</table>