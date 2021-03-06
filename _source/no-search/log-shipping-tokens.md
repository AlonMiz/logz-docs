---
layout: article
title: Log shipping tokens
permalink: /user-guide/tokens/log-shipping-tokens/
flags:
  alpha: true
  admin: true
tags:
  - tokens
  - account-tokens
contributors:
  - shalper
---

Log shipping tokens are used in shipper configurations to direct data to the relevant Logz.io account.
<br>
Every account has its own set of tokens.

You need to be an account admin to access your tokens and to view or manage them.

To manage your log shipping tokens, select an account, and then select [**<i class="li li-gear"></i> > Settings > Manage accounts**](https://app.logz.io/#/dashboard/settings/manage-tokens/log-shipping) in the top menu.

#### Managing log shipping tokens

You can have up to 5 tokens enabled simultaneously.

* To create a token, click **+Add log shipping token**, type in a **name**, then click **Add**. The new token will be enabled by default.

* To rename a token, hover over the token, click **edit** <i class="li li-pencil"></i> and type in a new name. Then click **Save**.

* To delete a token, hover over it, and click **delete** <i class="li li-trash"></i> to delete it. A confirmation module will ask you to confirm the action.

* To enable or disable a token, toggle the control. <br> Every account is required to have at least one enabled token at any given time, so you will be blocked from disabling the last token.


#### Using log shipping tokens

Log shipping tokens are used in the shipping configuration to direct data to the relevant Logz.io account.

To view your tokens, go to [**<i class="li li-gear"></i> > Settings > Manage accounts**](https://app.logz.io/#/dashboard/settings/manage-tokens/log-shipping). Click any **Token** to copy it.

When configuring your log shippers, replace the `<<SHIPPING-TOKEN>>` placeholder with one of your enabled log shipping tokens. See more in the [log shipping guide]({{site.baseurl}}/shipping/).

If you are using the shipping instructions in the [Logz.io app](https://app.logz.io/#/dashboard/data-sources/Filebeat), keep in mind that the configurations include the default token for the account from which you are viewing the page. You can replace the token with any other active token, as needed.

#### Security advantages

Having multiple log shipping tokens gives you greater control to manage your tokens and to decide when and how to reset them for regulatory compliance reasons or for security best-practices.

For example, you'll be able to cycle your tokens following changes to your team, after members join or leave, or when collaborating with contractors outside of your organization. If you're working on an integration with a partner organization, you'll be able to give them a temporary log shipping token and delete it once the project is complete.
