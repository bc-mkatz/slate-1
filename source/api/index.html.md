---
title: BigCommerce API Documentation
layout: "apitwocolumn"

language_tabs:
  - json--request
  - json--response

toc_footers:
  - <a href="/">Home</a>
  - <a href="/api/">API - Basics</a>
  - <a href="/themes/">Themes</a>
  - <a href="https://stencil.bigcommerce.com/docs/" target="_blank"> &nbsp;  Stencil Themes</a>
  - <a href="/themes/blueprint/"> &nbsp; Blueprint Themes</a>
  - <a href="http://goo.gl/forms/380FmYFlaJ05CL3q2" target="_blank">Sign Up for the Developer Newsletter</a>
  - <a href="http://github.com/tripit/slate" target="_blank">Site Built with Slate</a>

includes:
  - api_2_quick_starts
  - api_oauth_tokens
  - api_basic_auth_tokens
  - api_partners
  - api_req_headers
  - api_response_headers
  - api_media_types
  - api_clients
  - api_webhooks_getting_started
  - api_root_oauth
  - api_registration
  - api_callback
  - api_load
  - api_multi-user
  - api_ui_constraints
  - api_scopes
  - api_rate-limits_oauth
  - api_approval-requirements
  - api_completing_reg
  - api_app_gallery
  - api_sample_contract
  - api_root_basic_auth
  - api_legacy_basic_auth
  - api_rate_limits_basic
  - api_guides_oauth_transition
  - api_storefront_apps_root
  - api_customer_login
  - api_current_customer
  - add-to-cart-urls
  - api_browsers.md
  - api_status_codes
  - api_data_types
  - api_faqs

search: true
---

# <span class="jumptarget"> API Documentation </span>

The Bigcommerce Stores API features a RESTful architecture, allowing you to code in the language of your choice. This API supports the [JSON&#160;media type](#media-types), and uses UTF-8 character encoding. 

With clever use of this API, you can automate various commerce, business, and publishing tasks, and can integrate all kinds of apps with our platform. 

All connections require authentication, and are secured by TLS encryption. As of June 30, 2016, all requests must support Server Name Indication (SNI). We currently support two generations of our API:

<span class="fake-h3"> [API v3 Documentation](//github.com/bigcommerce/api) </span>

  New Catalog/Customers/Orders API, with more-efficient variant/modifier model. OAuth-only, but fully backward-compatible with v2.

<span class="type-large">
<a class="button button--action" href="//github.com/bigcommerce/api"  style="margin-left: 0rem">
  View V3 Docs</a><br></span></p>

<span class="fake-h3"> [API v2 Documentation](/api/v2) </span>

  Core API. Supports all currently exposed resources via OAuth; supports compatible resources via Basic Auth.

<span class="type-large">
<a class="button button--action" href="/api/v2"  style="margin-left: 0rem">
  View V2 Docs</a><br></span></p>