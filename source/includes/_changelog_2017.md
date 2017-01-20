# <span class="jumptarget"> 2017 </span>



## <span class="jumptarget"> January </span>



### <span class="jumptarget"> Stencil: New template Property Replaces Deprecated template_file </span>

BigCommerce has deprecated the Stencil themes platform's global `template_file` property. Its replacement is a new `template` property, which returns correct page types for custom template files. To pick up this correction, you must update your Stencil CLI installation. For details and links, please see the <a href="https://stencil.bigcommerce.com/docs/release-notes" target="_blank">Stencil framework release notes</a>.

### <span class="jumptarget"> Stencil Cornerstone 1.4.2 Theme Released </span>

Version [1.4.2](https://stencil.bigcommerce.com/docs/cornerstone-14x-theme-release-notes#142) of Stencil's default Cornerstone theme is now available. To deter spam submissions through the storefront Contact form, this update replaces the Contact template's CAPTCHA challenge with a Google reCAPTCHA v1 challenge. For the PR #/commit # to apply this fix, please see the <a href="https://stencil.bigcommerce.com/docs/release-notes" target="_blank">Stencil framework release notes</a>.

### <span class="jumptarget"> Order Shipments > shipping_provider Usage Clarified </span>

We have updated our documentation on the Order Shipment <a href="/api/v2/#blog-posts-object-properties" target="_blank">object</a>, and <a href="/api/v2/#create-a-shipment" target="_blank">Create a Shipment endpoint</a>, to clarify that the `shipping_provider` property is effectively required in `POST` requests. (You should include the property, even as an empty string, to prevent the unexpected default behavior described in the documentation.)

### <span class="jumptarget"> Blog Posts > published_date Usage Clarified </span>

We have updated our documentation on the Blog Posts <a href="/api/v2/#blog-posts-object-properties" target="_blank">object</a>, and its <a href="/api/v2/#create-a-blog-post" target="_blank">POST</a> and <a href="/api/v2/#update-a-blog-post" target="_blank">PUT</a> endpoints, to clarify the usage of this API's `published_date` property. Although `published_date` is returned as an object in responses, your `POST` and `PUT` requests should supply it as a flat date string in <a href="http://tools.ietf.org/html/rfc2822#section-3.3" target="_blank">RFC 2822</a> or <a href="https://en.wikipedia.org/wiki/ISO_8601" target="_blank">ISO 8601</a> format.