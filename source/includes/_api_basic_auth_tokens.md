## <span class="jumptarget" id="basiccred"> Creating Basic Auth Credentials </span>

The following sections outline how to create and manage Basic Auth tokens in the BigCommerce control panel.

<aside class="warning">
<span class="aside-warning-hd">Limited Support for Basic Auth </span><br><br>
BigCommerce is gradually deprecating Basic Authentication. Apps must use <a href="#building-oauth-apps">OAuth</a> to access our v3 API.   
Even within the v2 API, apps relying on Basic Authentication cannot access some features. (For example, the Webhooks resource requires OAuth.) Also, apps intended for sale on the BigCommerce App Marketplace must use OAuth.
</aside>

### <span class="jumptarget" id="pvt_token"> Obtaining an API Token </span>

To get an API token, use the following steps:

1.  Log into your store's control panel.
2.  Select **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Select **Create a Legacy API Account**.
5.  Enter a **Username**. Reusing the app's name is a good way to keep track of which account corresponds to which app. After saving, you can use the API credentials listed on this page.
6.  Copy the **API Path** field's value and paste it into a text editor. You will need this value to authenticate your app.
7.  Copy the **API Token** field's value and paste it into a text editor. You will need this value to authenticate your app.
8.  Select **Save** if you're creating or changing the API account.

### <span class="jumptarget"> Revoking App Access </span>

To revoke app access to a store, use the following steps:

1.  Log into your store's control panel.
2.  Select **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Select the gears icon in the **Action** column, then select **Edit**.
5.  Select the **Generate New Token** button.
6.  Select the **Save** button.
7.  Select the check box next to the user.
8.  Select the trash-can button.
9.  Select **OK** in the confirmation prompt.

### <span class="jumptarget"> Regenerating an API Token </span>

To change the API token that an app is using to access a store, use the following steps:

1.  Log into your store's control panel.
2.  Select **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Select the gears icon in the **Action** column, then select **Edit**.
5.  Select the **Generate New Token** button.
6.  Select the **Save** button.

## <span class="jumptarget" id="request_basic"> Making an API Request with Basic Auth </span>

Many tools are available to interact with APIs. For example, to see how to quickly make initial requests using <a href="https://en.wikipedia.org/wiki/CURL" target="_blank">cURL</a> commands, please see our [cURL Quickstart Guide](#curl-quickstart-guide).