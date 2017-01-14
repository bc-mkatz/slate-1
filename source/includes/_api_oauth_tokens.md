# <span class="jumptarget" id=""> OAuth Tokens via CP – Draft </span>

<aside class="warning">
<span class="aside-warning-hd">Draft New CP > OAuth Instructions</span><br><br>
This will replace <em>subsections</em> of: <a href="https://developer.bigcommerce.com/api/#making-requests" target="_blank">https://developer.bigcommerce.com/api/#making-requests</a>.
</aside>

## <span class="jumptarget" id="cp_oauth_get"> Obtaining an OAuth Token </span>

You can create and manage OAuth tokens in the BigCommerce control panel by creating an API account, as described below. (Only the <a href="https://support.bigcommerce.com/articles/Public/Store-Owner" target="_blank">store owner</a> can create API accounts, which are limited to 50 accounts per store.) 

<img src="../assets/CreateAccount.png" alt="Creating an API account" height=80% width=80%>

To create your API account and its corresponding token, use the following steps:

1.  Log into the store, using the store owner's username/password.
2.  Select **Advanced Settings**.
3.  Select **API Accounts**. This will display the **Store API Accounts** page.
4.  Select **Create API Account**. This will display the **Create API Account** page shown above.
5.  In the **Name** field, summarize the purpose for which you will use these credentials. (This name is for internal use only, so assign any name that you will recognize.)
6.  In the **OAuth Scopes** section, select at least the minimal scopes your app will require (as explained <a href="#request_scopes" target="_blank">here</a>). 
8.  Select **Save** at the page's lower right-hand corner.

Successfully saving the account will display the pop-up shown below, containing the API credentials that your app will need for OAuth access: your **Client ID**, **Client Secret**, and **Access&#160;Token**. A .txt file containing the same credentials will also download to your computer.

<img src="../assets/SaveCreds.png" alt="Viewing and saving OAuth credentials" height=67% width=67%>

<aside class="warning">
<span class="aside-warning-hd">Keep Your Credentials</span><br><br>
There is no way to re-display this pop-up, after you select <b>Done</b> to dismiss it. So make sure you store your credentials &ndash; either by locating the downloaded .txt file, or by copying/pasting the contents of each field out of the pop-up. Otherwise, you will need to repeat all the above steps to generate new credentials.
</aside>


<aside class="notice">
<span class="aside-notice-hd">More Drafts Pending</span><br><br>
The 2 struck-out sections below are copied verbatim from existing content within <a href="https://developer.bigcommerce.com/api/#building-basic-auth-apps">https://developer.bigcommerce.com/api/#building-basic-auth-apps</a>. Awaiting <b>store owner</b> access to some integration store (or the correct experiment enabled on my own store) to test/rewrite corresponding steps under the new OAuth flow.  
</aside>

<strike>
## <span class="jumptarget" id="cp_oauth_revoke"> Revoking App Access </span>

To revoke app access to a store, use the following steps:

1.  Log into the store.
2.  Click **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Click the gears icon in the **Action** column and select **Edit**.
5.  Click the **Generate New Token** button.
6.  Select the **Save** button.
7.  Select the check box next to the user.
8.  Click the trash can button.
9.  Click **OK** in the confirmation prompt.

## <span class="jumptarget" id="cp_oauth_regen"> Regenerating an API Token </span>

To change the API token that an app is using to access a store, use the following steps:

1.  Log into the store.
2.  Click **Advanced Settings**.
3.  Select **Legacy API Accounts**.
4.  Click the gears icon in the **Action** column and select **Edit**.
5.  Click the **Generate New Token** button.
6.  Select the **Save** button.
</strike>
