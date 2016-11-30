Basic-Auth (or "Private") apps require the manual creation of an API token for each store. They are most useful for custom integrations for a single BigCommerce store. They generally use HTTP Basic Authentication (with the exception of [Draft apps](#private-apps-with-oauth)), and communicate directly with the store's API endpoints.

<aside class="warning">
<span class="aside-warning-hd">Limited Support for Basic Auth </span><br><br>
BigCommerce is gradually deprecating Basic Authentication. Apps must use <a href="#building-oauth-apps">OAuth</a> to access our v3 API.   
Even within the v2 API, apps relying on Basic Authentication cannot access some features. For example, the Webhooks resource requires OAuth.
</aside>

## <span class="jumptarget"> Private Apps with OAuth? </span>

A few private apps use OAuth. These exceptions must meet the following restrictions:

* To create a private app that uses OAuth, you must create it as a Draft app, on a per-user basis. This Draft app will be accessible only to stores belonging to the user who created the app in the Developer Portal.

* OAuth Draft apps are currently not shareable, unless they are approved and published in the App Store.

The remainder of this "Building Basic-Auth/Private Apps" section applies only to Basic Authentication apps.

## <span class="jumptarget"> Making Requests </span>

To allow an app to connect to a store using Basic Authentication, the store owner must manually generate an API key and provide this to the app developer along with a base path and user name.

To connect to a store using Basic Authentication, an app must:

*   Include the user name and API key in the `Authorization` field of each HTTP request header, using the following syntax: <NOBR>`Basic <username:API_key>`,</nobr> where `<username:API_key>` is base64-encoded. Here is a specific example:
    <NOBR>`Authorization: Basic YWRtaW46ZTBhMDJiMDM5NzczNWI4NzNlZGQ5NWE1ZmQ1Y2I5YmI=`</nobr>

*   Use the base path provided by the store owner.

*   Use TLS encryption.

If the user name and/or API token are invalid or missing, the app will get a `401 Unauthorized` response.

## <span class="jumptarget" id="pvt_token"> Obtaining an API Token </span>

To get an API token, complete the following steps.

1.  Log into the store.
2.  Click **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Click **Create a Legacy API Account**.
5.  Type the name of the user in the **Username** box.
6.  Copy the contents of the **API Path** box and paste this value into a text editor.
7.  Copy the contents of the **API Token** box and paste this value into a text editor.
8.  Click the **Save** button.
9.  Provide the user name, API base path, and API token to the app developer using a secure channel.

## <span class="jumptarget"> Revoking App Access </span>

To revoke app access to a store, complete the following steps.

1.  Log into the store.
2.  Click **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Click the gears icon in the **Action** column and select **Edit**.
5.  Click the **Generate New Token** button.
6.  Select the **Save** button.
7.  Select the check box next to the user.
8.  Click the trash can button.
9.  Click **OK** in the confirmation prompt.

## <span class="jumptarget"> Regenerating an API Token </span>

To change the API token that an app is using to access a store, complete the following steps.

1.  Log into the store.
2.  Click **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Click the gears icon in the **Action** column and select **Edit**.
5.  Click the **Generate New Token** button.
6.  Select the **Save** button.
