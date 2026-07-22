# Configuring subscription settings

!!! info

    **Last updated:** January 24, 2022 for OJS 3.3.0.8

This page tells you how to configure the 2 parts of OJS required to properly use the subscription module:

1.  [The Payments tab under Distribution Settings](#distribution-payments-page), and
2.  [The Payments page in the left-hand menu](#payments-page).

You must enable payments via Distribution > Payments in order for the Payments _page_ to appear.

You must complete both of these tasks for the Subscriptions page to appear on the front-end of the OJS site. By default, Subscriptions will appear in the About menu. If a link to the Subscriptions page does not appear under the About menu, you should ensure that both of these tasks are complete. You should also ensure that Subscriptions appears in the Assigned Menu Items list of your [navigation menu](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#navigation).

## Distribution > Payments page

1.  In the back end, click **Distribution** in the left-hand menu
2.  Click on the **Payments** tab
3.  Click the checkbox under **Enable.** Additional content will now appear on the page
4.  Using the **Payment Plugins** dropdown, select either **Paypal Fee Payment** or **Manual Fee Payment**
5.  Complete the fields for Paypal Fee Payment or Manual Fee Payment, as appropriate
6.  Click **Save.**

Once you complete step 6, a new link called **Payments** will appear in the left-hand navigation menu under Submissions, Issues and, if it is active, Announcements (see Figure 1).

![The Payments link appears after the links for Submissions, Issues, and Announcements.](/images/left-menu-link-to-Payments-page.jpg)

Figure 1: The Payments link appears after the links for Submissions, Issues, and, Announcements (if  active).

## Payments Page

If you do not see the link for Payments in the left-hand menu, you must complete the steps listed under [Distribution > Payments](#distribution-payments-page), above.

To complete setting up the subscriptions module:

1.  In the back end, click **Payments** in the left-hand menu
2.  Create one or more subscription types:
    1.  Click the **Subscription Types** tab
    2.  Click **Create New Subscription Type** and complete the required fields to create as many subscription types as required.
3.  Add your subscription policies:
    1.  Click the **Subscription Policies** tab
    2.  Complete all fields and click **Save**.
4.  Optionally, add per-article and per-issue reader fees:
    1.  Click **Payment Types**
    2.  Add a price to **Purchase Issue** and/or **Purchase Article**
    3.  Click **Save**.