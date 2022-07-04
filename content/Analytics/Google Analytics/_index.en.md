---
title: "Google Analytics"
date: 2018-12-29T11:02:05+06:00
lastmod: 2022-01-05T10:42:26+06:00
weight: 1
draft: false
# search related keywords
keywords: [""]
---

**Overview**

We leverage Google’s analytics capabilities so you can monitor how customers access and interact with your site. This can provide valuable insights about where you are doing well as well as improvements that you could make to improve your sales.

Google Analytics is an industry leading analytics system that provides information about where site visitors are coming from, how long they spend on your site, what they are doing on there, as well as many other customisable metrics. Find out more [here](https://marketingplatform.google.com/about/analytics/).

We use Google Tag Manager to collect data and pass information for Analytics to processing and display. Tag Manager collects this data by listening for events that your Voucherstore store emits, such as a product being added to a basket, or an order being completed. You can also add in your own custom events to track if there are other specific actions that you want to monitor. Find out more [here](https://marketingplatform.google.com/about/tag-manager/).


**Setting up Analytics (If you haven’t already)**

The first step is to set up your Google Tag Manager to listen for the events emitted by your Voucherstore store.

1. Visit https://tagmanager.google.com and sign in to your Google account.
2. In Tag Manager, click Accounts and then Create account.
3. Enter an account name and optionally indicate whether you’d like to share data anonymously with Google and others.
4. Enter a descriptive container name and select Web as the type of content.
5. After clicking Create, dismiss the pop-up that appears titled “Install Google Tag Manager”.


You now have a Google Tag Manager container set up. We now need to tell the container which events it should listen out for. Voucherstore provides a template container that includes all of the e-commerce tracking that we provide. Download the file from the link below by right clicking and pressing ‘save link as’. [Download Here](https://www.help.voucherstore.io/template-container.txt)

1. On Google Tag Manager, choose the Admin option on the navigation bar.
2. Click on the Import Container option.
3. Select Choose container file, and upload the Voucherstore GTM Template Container.
4. If you have just started with Google Tag Manager, you can select Existing under Choose workspace, and Overwrite your current Default Workspace. If you are already using Google Tag Manager prior to implementing it for your Voucherstore store, you can add it as a new container, or be sure to overwrite the one you have just created if following along with this guide.


Your Google Tag Manager container is now set up to listen out for the events it needs to. However, it does not yet know where to send this information. We need to set up a Google Analytics account.

1. Visit https://google.com/analytics and sign in to your Google account.
2. Follow the prompts to create a new account and property, or if you already have a Google Analytics implementation, create a new property for your Voucherstore store.
3. Note the Tracking ID for your new property.
4. Click the Back arrow on the left side of this page to take you back to the Admin dashboard. You should see three columns: Account, Property, and View.
5. In the View column, click E-commerce Settings and enable E-commerce and Enhanced E-commerce. You can also set your store currency in View Settings.


We need to let Tag Manager know the tracking ID of the Analytics property to send data to.

1. In Tag Manager, select Workspace from the navigation bar.
2. Select Variables from the sidebar.
3. Under User-Defined Variables, click on Google Analytics.
4. Change the Tracking ID to the Tracking ID from your Analytics property and save your changes.
5. Note the container ID shown in the navigation bar – this should start with “GTM-”.
6. Click Submit in the top right of the page, optionally enter a version name and description, and Publish your container.


**Adding Your GTM to Voucherstore**

The only thing left is to enter your container ID in your Voucherstore store settings to let Voucherstore know where to send its events.

1. From your Voucherstore dashboard, select ANALYTICS from the left hand navigation.
2. Click on [Google Tag Manager] in the top right of the page.
3. Enter your container ID in the field, and click [Save].

Your Voucherstore analytics are now set up and ready to use. Visits to your store will be tracked and sent to Google Analytics.

Be aware that customers using ad-blockers and certain cookie settings will inhibit tracking, so you should not rely on the information displayed in Google Analytics as a source of truth for things like sales totals. Also, depending on the traffic to your site, Analytics can take up to two days to update and reflect the latest statistics.
