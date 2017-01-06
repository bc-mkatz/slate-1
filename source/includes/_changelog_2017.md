# <span class="jumptarget"> 2017 </span>



## <span class="jumptarget"> January </span>

### <span class="jumptarget"> Order Shipments > shipping_provider Usage Clarified </span>

We have updated our documentation on the Order Shipment <a href="/api/v2/#blog-posts-object-properties" target="_blank">object</a>, and <a href="/api/v2/#create-a-shipment" target="_blank">Create a Shipment endpoint</a>, to clarify that the `shipping_provider` property is effectively required in `POST` requests. (You should include the property, even as an empty string, to prevent the unexpected default behavior described in the documentation.)

### <span class="jumptarget"> Blog Posts > published_date Usage Clarified </span>

We have updated our documentation on the Blog Posts <a href="/api/v2/#blog-posts-object-properties" target="_blank">object</a>, <a href="/api/v2/#create-a-blog-post" target="_blank">POST endpoint</a>, and <a href="/api/v2/#update-a-blog-post" target="_blank">PUT endpoint</a>, to clarify the `published_date` property's usage. Although `published_date` is returned as an object in responses, your `POST` and `PUT` requests should supply it as a flat date string in <a href="http://tools.ietf.org/html/rfc2822#section-3.3" target="_blank">RFC 2822</a> or <a href="https://en.wikipedia.org/wiki/ISO_8601" target="_blank">ISO 8601</a> format.