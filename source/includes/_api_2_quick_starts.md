# <span class="jumptarget" id="apiquickstart"> API/Apps First Steps </span>

The following sections offer initial steps for two different development scenarios:

* Developing private apps for a particular BigCommerce store: You can follow the [Apps Quick Start](#apicred) procedure, which has no administrative requirements.

* Developing <a href="https://www.bigcommerce.com/single-click-apps/" target="_blank">Single-Click Apps</a> for sale to/installation on any BigCommerce store: Jump to the [App Marketplace Workflow](#joinappmkt) procedure, which requires applying to become a BigCommerce partner.

These two scenarios are not mutually exclusive –  some developers will work under both scenarios. But some of their setup instructions are redundant. Therefore, we suggest that you start with the section that best matches your immediate scenario.

# <span class="jumptarget" id="api2paths"> Apps Quick Start </span>

<aside class="notice">
<span class="aside-notice-hd"> Private or Saleable Apps? </span><br><br>
This section is intended for developers who want to immediately start developing and testing private apps for a particular store. <br> If your ultimate goal is to distribute apps on the BigCommerce Apps Marketplace, you can avoid repeated steps (like creating trial/sandbox stores for app testing) by jumping directly to the instructions under <a href="#joinappmkt">Joining the BigCommerce App Marketplace</a>.
</aside>

To obtain Basic or OAuth credentials to use this API, you will first need to create a trial store. (If you already have a store, skip ahead to [Logging&#160;In](#login).)

## <span class="jumptarget" id="createstore"> Creating a Trial Store</span>

1. Go to the <a href="https://www.bigcommerce.com" target ="_blank">BigCommerce home page</a>.

2. Select either **GET STARTED** or **START YOUR FREE TRIAL**.

3. Enter an email address where prompted, and select **START YOUR TRIAL**.

4. In the trial store form, enter a store name, password, and other details. Then select **CREATE YOUR STORE**.

5. Wait for the store-creation animation to stop, then select either **FINISH** or **Ask Me Later**.

## <span class="jumptarget" id="login"> Logging In</span>

If you have just created your trial store, you will already be logged into the store's control panel. Skip ahead to [Creating Basic Auth Credentials](#basiccred).

Otherwise, you might need to log into your store:

1. Return to the <a href="https://www.bigcommerce.com" target ="_blank">BigCommerce home page</a>.

2. Select **LOG IN** at the upper right. 

3. If prompted to **Log in to your store**, enter the email address and password you set when you created  your trial, then select **LOG IN**.

    This will reopen your store's control panel.

