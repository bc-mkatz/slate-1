Basic-Auth (or "Private") apps require the manual creation of an API token for each store. They are most useful for custom integrations for a single BigCommerce store. They generally use HTTP Basic Authentication (with the exception of [Draft apps](#private-apps-with-oauth)), and communicate directly with the store's API endpoints.

<aside class="warning">
<span class="aside-warning-hd">Limited Support for Basic Auth </span><br><br>
BigCommerce is gradually deprecating Basic Authentication. Apps must use <a href="#building-oauth-apps">OAuth</a> to access our v3 API.   
Even within the v2 API, apps relying on Basic Authentication cannot access some features. (For example, the Webhooks resource requires OAuth.) Also, apps intended for sale on the BigCommerce App Marketplace must use OAuth.
</aside>

## <span class="jumptarget" id=""> Obtaining Basic-Auth API Tokens </span>

To obtain tokens to connect your app to a BigCommerce store using Basic Auth, please see [Creating Basic Auth Credentials](#basiccred).

## <span class="jumptarget"> Making Basic-Auth Requests </span>

To allow an app to connect to a store using Basic Authentication, the store owner must manually generate an API key and provide this to the app developer along with a base path and user name.

To connect to a store using Basic Authentication, an app must:

*   Include the user name and API key in the `Authorization` field of each HTTP request header, using the following syntax: <NOBR>`Basic <username:API_key>`,</nobr> where `<username:API_key>` is base64-encoded. Here is a specific example:
    <NOBR>`Authorization: Basic YWRtaW46ZTBhMDJiMDM5NzczNWI4NzNlZGQ5NWE1ZmQ1Y2I5YmI=`</nobr>

*   Use the base path provided by the store owner.

*   Use TLS encryption.

If the user name and/or API token are invalid or missing, the app will get a `401 Unauthorized` response.


