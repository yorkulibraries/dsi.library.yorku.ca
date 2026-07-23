# The OJS site

!!! info

    **Last updated:** October 4, 2021

This sections deals with parts of the OJS site that don’t relate directly to issues or submissions. This includes page content and user roles. See also [PKP Docs](https://docs.pkp.sfu.ca/) for the developer’s documentation on how to work with OJS.

## Understanding the OJS homepage layout (Default Theme)

!!! info

    **Last updated:** August 9, 2022 for OJS 3.3.0.11

This chapter provides an overview of all possible elements that appear on the homepage of a journal using the OJS Default Theme. This chapter only discusses the layout of the homepage as viewed on a large screen, such as a computer or large tablet.

### OJS homepage layout (Default Theme)

The page elements labeled in this screenshot are described in the next section.

![Annotated screenshot of the OJS homepage showing the relative location of site elements](/images/hompage-logo-ANNOTATED.png)

#### 1\. Header OR header background image

By default, OJS displays a coloured header at the top of the page that spans the entire window. The colour can be configured via **Website Settings > Appearance > Theme**, using the **Colour** field.

You can replace the entire header with an image if you follow two steps:

1.  Add a homepage image in **Website Settings > Appearance > Setup** in the **Homepage Image** field
2.  Click the checkbox under **Header Background Image** in **Website Settings > Appearance > Theme.**

If you use this option, you cannot have a regular homepage image (#6 below).

The screenshot on this page shows a journal homepage with the homepage image in the default location. You can also see an [example of the same journal with the homepage image used as a header background](/images/homepage-logo-background.png).

The header or header background image persist across all pages on the OJS site.

#### 2\. User navigation menu

The user navigation menu appears at the top right of the screen, against the backdrop of the header. When the visitor is logged out, this menu displays **Register** and **Login** buttons. When logged in, it displays the username as a dropdown menu with the links **Dashboard**, **View Profile**, and **Logout**.

The user navigation menu can be configured via **Website Settings > Setup > Navigation**, using the **Navigation** and Navigation Menu Items fields.

The user navigation menu persists across all pages on the OJS site.

#### 3\. Title OR logo

By default, OJS displays the title of the journal as an H1-level heading at the top left of the page, against the backdrop of the header. The title is configured via **Journal Settings > Masthead**, using the **Journal title** field.

You can display a logo image instead of the title of the journal. The logo is configured via **Website Settings > Appearance > Setup**, using the **Logo** field.

The screenshot on this page shows a journal homepage with a logo instead of the journal title. You can also see an [example of the same journal with the journal title instead of a logo.](/images/homepage-nologo.png)

The title or logo persist across all pages on the OJS site.

#### 4\. Primary navigation menu

The primary navigation menu appears under the journal title or logo, against the backdrop of the header and aligned to the left margin.

The primary navigation menu can be configured via **Website Settings > Setup > Navigation**, using the **Navigation** and Navigation Menu Items fields.

The primary navigation menu persists across all pages on the OJS site.

#### 5\. Search

The search tool appears under the journal title or logo, against the backdrop of the header and aligned to the right margin. The search tool cannot be configured.

The search tool persists across all pages on the OJS site.

#### 6\. Homepage image

The homepage image is an optional element. It will only appear if an image has been uploaded to **Homepage Image** in **Website Settings > Appearance > Setup**. The homepage image will appear in the central pane of the page, below the header.

The homepage image will only be displayed on the homepage.

The homepage image can also be used to replace the coloured header (#1 above) if you upload an image and click the checkbox under **Header Background Image** in **Website Settings > Appearance > Theme**. If you use this option, you cannot have a regular homepage image.

#### 7\. Blocks

Blocks appear in the right sidebar, below the header. Multiple blocks display in sequence vertically. Blocks are configured via **Website Settings > Appearance > Setup** using the **Sidebar** field. Some [plugins](#managing-plugins) may add blocks to your sidebar. You can also [create custom blocks](#adding-custom-blocks-to-the-right-sidebar) for your site.

Blocks persist across all pages of the OJS site.

#### 8\. Journal Summary

The journal summary is an optional element. If activated, the journal summary will appear in the central pane of the page, below the header. If a Homepage image is present (#6), it will appear below that image.

OJS automatically adds the heading "About the Journal" when the journal summary appears.

You can activate the journal summary if you follow two steps:

1.  Add the summary text in **Journal Settings > Masthead** using the **Journal Summary** field
2.  Click the checkbox under **Journal Summary** in **Website Settings > Appearance > Theme.**

The journal summary will only be displayed on the homepage.

#### 9\. Announcements

Announcements are an optional element. If activated, announcements will appear in the central pane of the page, below the header. If a homepage image (#7) or journal summary (#8) are present, it will appear below these elements.

You can activate announcements if you click the checkbox under **Announcements** in **Website Settings > Setup > Announcements** and click **Save.** You can then add announcements via **Announcements** in the left sidebar menu.

Even if announcements are activated, the announcement elements will _not_ appear on the homepage if:

*  The number in the *Display on Homepage* field at **Website Settings > Setup > Announcements** is set to 0, or
*  No announcements have been published, or
*  All published announcements have expired.

The announcements element will only be displayed on the homepage. However, activating the announcements feature will create a new page called Announcements and automatically added to it the primary navigation menu.

#### 10\. Current Issue

By default, OJS displays the journal’s Current Issue on the homepage. The current issue announcements appears in the central pane of the page, below the header. If a homepage image (#6), a journal summary (#8), or announcements (#9) are present, it will appear below these elements.

The current issue element displays the full issue metadata and table of contents, including:

*   Issue cover, if present
*   Issue volume, number, year, and title as applicable
*   Issue description, if present
*   Issue publication date
*   Section titles for all sections included in the issue
*   Submission covers for all submissions, if present
*   Submission titles for all submissions and subtitles, if present
*   Submission contributors for all submissions
*   Submission page numbers for all submissions, if present
*   Submission galley links for all submissions

OJS automatically adds the heading "Current Issue" to the top of this element and adds a link to the Archive labeled "View All Issues" to the bottom.

By default, your Current Issue is your most recently published issue; however, you can also [change your Current Issue](issues#setting-your-current-issue).

The current issue element will only be displayed on the homepage.

#### 11\. Additional Content

Additional content is an optional element. It will only appear if content has been added to **Additional Content** in **Website Settings > Appearance > Advanced**. The additional content will appear in the central pane of the page, below the current issue.

Additional content will only be displayed on the homepage.

#### 12\. Page Footer

By default, OJS displays a light grey footer at the bottom of the page that spans the entire window. The colour cannot be configured.

You can add content to the page footer via **Website Settings > Appearance > Setup**, using the **Page Footer** field.

The page footer persists across all pages on the OJS site.

#### 13\. PKP logo

By default, OJS displays the logo of the software developer, PKP, in the bottom left corner of the page against the backdrop of the footer. This logo cannot be configured.

The PKP logo persists across all pages on the OJS site.


## Managing your site's appearance


!!! info

    **Last updated:** October 21, 2025 for OJS 3.3.0.19

This chapter covers the different elements of OJS that affect the appearance and layout of your site. This chapter complements the information presented in the PKP guide [Designing Your Journal](https://docs.pkp.sfu.ca/designing-your-journal/en/) and in the [Website Settings section](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website) of [Learning OJS 3.3](https://docs.pkp.sfu.ca/learning-ojs/en/); this chapter links to the relevant sections from those guides throughout.

OJS uses [responsive web design](https://en.wikipedia.org/wiki/Responsive_web_design), which means that site elements will automatically rescale and rearrange to fit larger or smaller browser windows. You can see how this works on a computer by manually resizing your browser window. There is no mobile version of the OJS website: the site automatically optimizes for viewing according to the browser size. This chapter uses "large browser window" to refer to the experience a user would have on a computer with a maximized browser window or a large tablet; it uses "small browser window" to refer to the experience a user would have on a phone, a small tablet, or a computer with a small browser window.

There are five ways you can affect the overall look and feel of your OJS site:

* [General settings](#general-settings)  
* [Theme and theme settings](#theme-and-theme-settings)  
* [Navigation menus](#navigation-menus)  
* [Sidebar blocks](#sidebar-blocks)  
* [Stylesheets](#stylesheets)  

### General settings

Some elements that appear on the site are common to all journals, regardless of theme. These are controlled via **Website Settings > Appearance > Setup** and **Website Settings > Appearance > Advanced.**

The elements controled via **Website Settings > Appearance > Setup** are:

*   **Logo**: an image that will appear in the header of any page on your site.. If you do not use a logo, the title of your journal will appear here as text.
*   **Journal thumbnail**: this setting is not used for YDJ journals and is not necessary for your journal.
*   **Homepage Image**: an image that will appear on the homepage of your site, unless the Homepage Background Image toggle (described below) is used.
*   **Page Footer**: text or other content that will appear on the footer of any page on your site.
*   **Sidebar**: sidebar blocks will be discussed in a separate section on this page.

The elements controled via **Website Settings > Appearance > Advanced** are:

*   **Journal style sheet**: this setting will be discussed in a separate section on this page.
*   **Favicon**: upload a [favicon](https://en.wikipedia.org/wiki/Favicon) for your journal.
*   **Additional Content**: text or other content that will appear at the bottom of the content page of your homepage only.

You can read more about [Appearance Setup](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#setup) and [Advanced Appearance](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#advanced) settings in Learning OJS 3.3.

### Theme and theme settings

Many elements of the OJS website are controlled by theme and the theme settings. These are configured through **Website Settings > Appearance > Theme.** When using the Default Theme, these settings are:

*   **Typography**: font combinations used on the site.
*   **Colour**: the colour of the site header.
*   **Journal Summary**: toggle whether the Journal Summary appears on the homepage.
*   **Header Background Image**: toggle whether the homepage image (if applicable) appears as the background of the header or in the main content pane.

YDJ prefers that participating journals use the Default Theme for two reasons:

1.  The Default Theme has been audited for accessibility and simplifies journals’ requirement to comply with the _Accessibility for Ontarians with Disabilities Act_ (AODA), whereas other themes may present accessibility issues, and
2.  Themes other than Default are not always updated with the core OJS software and may not render or function properly when YDJ upgrades your journal to a new version of the software.

If you wish to use or try out different themes for your journal, please [contact YDJ](ydj-contact.md). Themes are implemented as [plugins](#managing-plugins) and you will not be able to implement them without assistance. YDJ cannot customize themes or fix any problems with non-Default themes that may arise.

You can read more about [Theme settings](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#theme) in Learning OJS 3.3 and about [Theme Features and Design Elements](https://docs.pkp.sfu.ca/designing-your-journal/en/theme-features-design-elements) in Designing Your Journal. If you have access to development expertise, you can read about creating or modifying themes in the [PKP Theming Guide](https://docs.pkp.sfu.ca/pkp-theming-guide/en/).

### Navigation menus

There are two navigation menus in the OJS Default Theme: the User Navigation Menu and the Primary Navigation Menu. Both menus are configured via **Website Settings > Setup > Navigation**. These menus may be rearranged; items may also be added or removed.

The **User Navigation Menu** contains a login link when site visitors are logged out or, when logged in, links related to their OJS user account. It appears at the top right of all OJS site pages when viewed in a large browser window; in a small browser window, these links are accessible via the hamburger menu at the top of the page.

The **Primary Navigation Menu** contains links to the public-facing site content, including About the Journal, Submissions, and Archives. It appears at the bottom of the site header on all OJS site pages when viewed in a large browser window; in a small browser window, these links are accessible via the hamburger menu at the top of the page alongsite the User Navigation Menu links.

You can edit each menu by rearranging, adding, and removing menu items. Be careful when removing menu items, lest you make important parts of the website inaccessible to readers. Adding a new **Navigation Menu Item** creates a new page on the OJS site that can be added to a menu.

You can read more about [Navigation settings](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#navigation) in Learning OJS 3.3.

!!! warning

    Creating a page with the same URL as an existing page in OJS may cause a site-breaking URL conflict. Before creating a new page, test your intended URL by inputting it into your browser to see if a page with that URL already exists on your site.

### Sidebar blocks

**Blocks** are flexible content containers that can appear to the right of the main content pane on any OJS page (on a large browser window) or below it (on a small browser windows). Blocks are managed via the **Sidebar** settings at **Website Settings > Appearance > Setup**, where you can reorder, activate, or deactivate blocks.

Several blocks are activated by default in OJS. Several [plugins](#managing-plugins) will also create blocks that can be managed via the Sidebar settings. One of these plugins is the Custom Block Manager, which allows you create custom block content. Learn more about [Adding custom blocks to the right sidebar](#adding-custom-blocks-to-the-right-sidebar) elsewhere in this guide.

### Stylesheets

You can customize the deisgn of your OJS site by adding a .css file to **Journal style sheet**, which is accessed via **Website Settings > Appearance > Advanced**. You can read more about stylesheets in the [Create a Stylesheet](https://docs.pkp.sfu.ca/designing-your-journal/en/creating-stylesheet) section of Designing Your Journal.

YDJ cannot customize stylesheets or fix any problems with custom stylesheets that may arise. If your custom stylesheet causes accessibility problems, we will require you to edit your stylesheet; if the accessibility problems are serious enough, we may have to remove the stylesheet unilaterally in order to comply with AODA requirements.

## Adding custom blocks to the right sidebar

!!! info

    **Last updated:** November 22, 2021 for OJS 3.3.0.8

You can create custom blocks to appear in the right sidebar by following these steps:

1.  In the back end, go to **Website > Plugins**.
2.  On the Installed Plugins screen, you should see plugin called **Custom Block Manager** in the Generic Plugins section.
    1.  If you do not see the Custom Block Manager in that list, [contact YDJ](ydj-contact.md) to have it installed before proceeding.
3.  Activate the Custom Block Manager by clicking the checkbox beside the plugin description.
4.  Once activated, click the blue triangle next to the plugin name to see the plugin options.
5.  Click **Manage Custom Blocks**.
6.  In the Custom Block Manager window, click **Add Block**.
7.  Add the **Block Name**, **Content**, and check **Show Name** if desire.
8.  Click **Save**.
9.  Go to **Website > Appearance** > **Setup.**
10.  Activate your custom block by checking the box next to the block name in the Sidebar section.
11.  Drag the blocks into your preferred order.
12.  Click **Save.**

## Managing plugins

!!! info

    **Last updated:** October 7, 2021 for OJS 3.3.0.8

Plugins provide extra functions in OJS. Some plugins are developed by the PKP community and are available through the OJS administrative interface; others are developed by third parties and must be uploaded manually.

### Managing plugins

You can access your journal’s plugins through the **Plugins** tab on the **Website Settings** page. There, you will find two facets: Installed Plugins and Plugin Gallery.

**Installed Plugins** lists the plugins that are installed on your system but not necessarily activated. To activate them, you must click the checkbox to the left of the plugin’s name.

Most of the built-in plugins for OJS are updated when the core OJS software package is updated.

### Installing and updating plugins

The **Plugin Gallery** lists optional plugins that you can install on your system and will also display whether updates are available. Only the OJS administrator can install and update plugins – you will not be able to do this for your own journal, even if you have the Journal Manager user role. If you wish to install or upgrade a plugin, please [contact YDJ](ydj-contact.md).

YDJ has not yet been able to automate the plugin update process for our journals, although we are currently working on this. Therefore, you may sometimes discover that certain plugins (such as [QuickSubmit](submissions#using-the-quicksubmit-plugin) are not available due to an update being required. If this happens, please [contact YDJ](ydj-contact.md).

### Third-party plugins

If you discover third-party plugins you wish to use, [contact YDJ](ydj-contact.md) to discuss installing them. If YDJ has no immediately concerns about security or computing resources, we should be able to install them for you.

YDJ cannot support the use or maintenance of third-party plugins. In other words: if the plugin doesn’t work with the current version of OJS, or if the plugin doesn’t work as expected, or if you can’t figure out to use the plugin, we will be unable to support you. Additionally, if YDJ discovers that there is a major security concern with the plugin, we may have to unilaterally uninstall it.

## Web and readership statistics

!!! info

    **Last updated:** July 8, 2026 for OJS 3.5

This chapter covers two types of statistics:

* [Article and editorial statistics](#article-and-editorial-stats), which are collected and accessed through OJS itself, and
* [Web analytics](#web-analytics), which are collected by third-party applications.

### Article and editorial stats

OJS offers robust statistical reporting tools for article views and downloads and for editorial activity as of version 3.2.

You can [learn about OJS’ built-in statistics reports](https://docs.pkp.sfu.ca/learning-ojs/en/statistics) in the _Learning OJS 3_ guide.

### Web analytics

You should know that analytics packages only provide statistics as of the date of their implementation.

#### Matomo

YUL has implemented a locally-hosted instance of [Matomo](https://matomo.org/) for all journals as an alternative to Google Analytics. As of late 2023, Matomo has been configured for all YDJ publications. YDJ does not currently have standardized reporting procedures: if you would like to request stats from Matomo, please [contact YDJ](ydj-contact.md).

#### Google Analytics

Some YDJ journals created in OJS prior to 2019 used [Google Analytics Universal Analytics](https://analytics.google.com), which was shut down in 2024. YDJ no longer maintains Google Analytics accounts for journals and has replaced the service with Matomo.

## Changing user roles

!!! info

   **Last updated:** April 19, 2022 for OJS 3.3.0.10

To change the roles assigned to any user account, including your own:

1.  In the left navigation menu, click **Users & Roles** (under Settings)
2.  Search or browse to locate the account you wish to edit
3.  Click the blue triangle to the left of the user name and then click **Edit User**
4.  In the Edit User window, scroll down to User Roles and check/uncheck the roles as required
5.  Click **OK** to save your changes.

You must have the Journal Manager or Journal Editor role in order change user roles. However, you will not be able to change the YDJ admin account or certain special accounts created by and for YDJ staff.

## Reviewing user roles

!!! info

    **Last updated:** April 19, 2022 for OJS 3.3.0.10

Certain [user roles](https://docs.pkp.sfu.ca/learning-ojs/en/users-and-roles) in OJS grant permissions to make major changes to the OJS site or to publish and unpublish content. **Journal Manager**, **Journal Editor**, and **Production Editor** are the roles with the most permissions to make changes to the site and content. **Section Editor** and **Guest Editor** may also affect site content to a less degree.

For security’s sake, it is important to make sure that users do not retain these roles if they no longer occupy editorial positions for your journal. You should ensure that only current editorial staff for your journal have these roles in OJS. YDJ recommends that you periodically review which users have these editorial roles, and update those users’ accounts as required.

You must have the Journal Manager or Journal Editor role to view user accounts.

To review all user accounts that have a particular role:

1.  In the left-hand navigation menu, click **Users & Roles** under _Settings_
2.  Click the **Search** button
3.  Use the drop-down menu to select the role you wish to review (the default is _All Roles_)
4.  Leave the text box blank and click **Search.**

You will now see a list of all user accounts that have this this role assigned. You can now [update user roles](#changing-user-roles) as required.

**Note:** YDJ maintains an admin account for all journals, which is required for hosting. Periodically, YDJ will create additional accounts for troubleshooting or for special projects – we will generally inform you if this is required and will usually use descriptive usernames to identify these accounts.. We also have a policy of periodically reviewing and, if necessary, removing YDJ staff accounts. If you see any accounts that should not have editorial privileges for your journal, you should update them accordingly.

## Adding sections

!!! info

    **Last updated:** August 18, 2022 for OJS 3.3.0.11

To add a new section to your journal:

1.  Go to **Journal Settings > Sections**
2.  Click **Create Section**
3.  Add the **Section Title** and **Abbreviation**
4.  You may add a **Section Policy** if you wish.
    1.  Note: this content will appear on the Submissions page on the front end, alongside the Submission Guidelines
5.  Check the **Section Options**, as appropriate
    1.  Note: important options with downstream implications include **Will not be peer-reviewed**, **Do not require abstracts**, and **Items can only be submitted by Editors and Section Editors**.
6.  Click **Save**.

The new section will now be available during the appropriate submission workflows.

## Enabling and disabling notifications

!!! info

    **Last updated**: November 9, 2022 for OJS 3.3.0.13

OJS makes several automatic notifications available to users. These notifications may be email and will also appear in the notifications section of the journal dashboard for logged-in users. Some user accounts are automatically enrolled for specific notifications based on their role – for example, journal editors are automatically enrolled for email notifications about editorial statistics.

To turn notifications on or off:

1.  Log into your OJS account for the journal
2.  In the back end, click the profile avatar icon in the top, far-right corner of the window
3.  Click **Edit Profile**
4.  On the Profile page, open the **Notifications** tab
5.  Enable or disable notifications and email alert for specific events and announcements as required
6.  Click **Save**.

At present, it does not appear to be possible for journal managers or editors to enable or disable notifications on behalf of users.
