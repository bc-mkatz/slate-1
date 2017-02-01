# <span class="jumptarget" id="postman_qs"> Postman/OAuth Quickstart Guide </span>

This section shows you how to quickly get started exercising BigCommerce APIs, using the <a href="https://www.getpostman.com/" target="_blank">Postman app</a>.

To get started, you'll need OAuth credentials to supply to Postman. BigCommerce uses OAuth 2.0. 

## <span class="jumptarget"> Creating OAuth2.0 Credentials </span>

Create your OAuth 2.0 credentials as described above under [Obtaining OAuth Tokens](/api#cp_oauth_get). (Depending on what scopes you set, you will be limited in what objects you can request. You can view scope information [here](/api#oauth-scopes).)

## <span class="jumptarget"> Postman Setup </span>

You'll do the next steps in the Postman app.

### <span class="jumptarget"> Select No Auth </span>

In Postman, set the **Type** drop-down list to **No Auth** (so as to create only the OAuth headers that you need). This will display the form shown below:

![](../assets/postman-noauth.png)

### <span class="jumptarget"> Populate Auth Headers </span>

Select the **Headers** tab to display the form shown below: 

![](../assets/postman-headers.png)

Next, add these two key/value pairs, using the OAuth credentials you obtained in the BigCommerce control panel:

| Key | Value |
|---|---|
| `X-Auth-Client` | The **Client ID** you obtained when you [created your OAuth token](/api#cp_oauth_get). |
| `X-Auth-Token` | The **Access Token** string you obtained when you [created your OAuth token](/api#cp_oauth_get). |


## <span class="jumptarget" id="post_setup"> Sending a Request </span>

We have created a collection of Postman requests for our v3 API, which you can import by clicking the button below:

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/0911a7fefbc14ed2e4cb)

To use this collection, you'll need to enter your OAuth credentials, as explained above under [Postman Setup](#post_setup).
 
You'll also need to enter your store's API Path, as displayed in the [control panel](/api#cp_oauth_get). You can do so in either of these days:

* Within each endpoint, replace the variable `{{store_hash}}`; or 

* Add a new environment, in which you create a  `store_hash` key, then set its value to the alpahnumeric string from your API Path. (For&#160;details on setting up a Postman environment, see [this Postman documentation](https://www.getpostman.com/docs/environments).)

Now you can send and receive information through an OAuth API connection with BigCommerce. If you'd like to register webhooks through Postman, please see [Creating Webhooks: Sending the POST Request](/api#creating-webhooks-sending-the-post-request). 


