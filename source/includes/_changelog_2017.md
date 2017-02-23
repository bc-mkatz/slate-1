# <span class="jumptarget"> 2017 </span>


## <span class="jumptarget"> February </span>


### <span class="jumptarget"> Stencil Cornerstone 1.5.2 Theme Released </span>

Version 1.5.2 of Stencil's default Cornerstone theme is now available. (Release notes updated [here](https://stencil.bigcommerce.com/docs/release-notes-cornerstone-15-theme#152).) This release adds a Theme Editor check box to toggle the display of a GeoTrust SSL Seal in the footer. It also corrects carousel display/cropping on wide viewports, clarifies the usage of Theme Editor's `Social Media Icons` controls, and corrects a bug that displayed `Sign Up` links even when store-account creation had been disabled in the control panel.


### <span class="jumptarget"> Postman Guide for BigCommerce APIs </span>

For developers who want to exercise BigCommerce APIs without (or prior to) building an app, we have added a [guide](/api/guides/#postman-oauth-quickstart-guide) to using Postman with our APIs.


### <span class="jumptarget"> Stencil Repo Adds Onboard Changelog </span>

<b>2017-02-07:</b> The Stencil public repository now maintains its own changelog, at:     
[https://github.com/bigcommerce/stencil/blob/master/CHANGELOG.md](https://github.com/bigcommerce/stencil/blob/master/CHANGELOG.md). (Stencil-3000; PR # 919)


### <span class="jumptarget"> Stencil Cornerstone 1.5.1 Theme Released </span>

Version 1.5.1 of Stencil's default Cornerstone theme is now available. (Release notes updated [here](https://stencil.bigcommerce.com/docs/release-notes-cornerstone-15-theme#151).) This maintenance release corrects a duplicate Quick Search close box in mobile viewports, corrects a redundant Theme&#160;Editor horizontal scroll bar in smaller viewports, corrects carousel display/cropping on mobile viewports, and corrects a bug that displayed Gift Certificates options even when gift certificates had been disabled in the control panel. 


### <span class="jumptarget"> Stencil Cornerstone 1.5.0 Theme Released </span>

Version [1.5.0](https://stencil.bigcommerce.com/docs/release-notes-cornerstone-15-theme) of Stencil's default Cornerstone theme is now available. This release adds several new options for store owners to customize their store's appearance via Theme Editor. These options include displaying sale badges, displaying "as low as $x" pricing, and requiring customer logins for pricing and cart access. It also corrects the behavior of hashbang links (`#!`), and corrects the display of product options in Quick View modals. For the PR #'s/commit #'s to cherry-pick the hashbang fix, please see the <a href="https://stencil.bigcommerce.com/docs/release-notes" target="_blank">Stencil framework release notes</a>.


## <span class="jumptarget"> January </span>


### <span class="jumptarget"> OAuth Tokens via Control Panel </span>

The BigCommerce control panel's new **Advanced Settings** > **API Accounts** option allows you to directly generate and revoke OAuth tokens and their associated user accounts. For details on using these new options with your apps, please see our new documentation on <a href="/api/#cp_oauth_get" target="_blank">Obtaining OAuth Tokens</a>. 


### <span class="jumptarget"> Stencil: New template Property Replaces Deprecated template_file </span>

BigCommerce has deprecated the Stencil themes platform's global `template_file` property. Its replacement is a new `template` property, which returns correct page types for custom template files. To pick up this correction, you must update your Stencil CLI installation. For details and links, please see the <a href="https://stencil.bigcommerce.com/docs/release-notes" target="_blank">Stencil framework release notes</a>.

### <span class="jumptarget"> Stencil Cornerstone 1.4.2 Theme Released </span>

Version [1.4.2](https://stencil.bigcommerce.com/docs/cornerstone-14x-theme-release-notes#142) of Stencil's default Cornerstone theme is now available. To deter spam submissions through the storefront Contact form, this update replaces the Contact template's CAPTCHA challenge with a Google reCAPTCHA v1 challenge. For the PR #/commit # to apply this fix, please see the <a href="https://stencil.bigcommerce.com/docs/release-notes" target="_blank">Stencil framework release notes</a>.

### <span class="jumptarget"> Order Shipments > shipping_provider Usage Clarified </span>

We have updated our documentation on the Order Shipment <a href="/api/v2/#blog-posts-object-properties" target="_blank">object</a>, and <a href="/api/v2/#create-a-shipment" target="_blank">Create a Shipment endpoint</a>, to clarify that the `shipping_provider` property is effectively required in `POST` requests. (You should include the property, even as an empty string, to prevent the unexpected default behavior described in the documentation.)

### <span class="jumptarget"> Blog Posts > published_date Usage Clarified </span>

We have updated our documentation on the Blog Posts <a href="/api/v2/#blog-posts-object-properties" target="_blank">object</a>, and its <a href="/api/v2/#create-a-blog-post" target="_blank">POST</a> and <a href="/api/v2/#update-a-blog-post" target="_blank">PUT</a> endpoints, to clarify the usage of this API's `published_date` property. Although `published_date` is returned as an object in responses, your `POST` and `PUT` requests should supply it as a flat date string in <a href="http://tools.ietf.org/html/rfc2822#section-3.3" target="_blank">RFC 2822</a> or <a href="https://en.wikipedia.org/wiki/ISO_8601" target="_blank">ISO 8601</a> format.
