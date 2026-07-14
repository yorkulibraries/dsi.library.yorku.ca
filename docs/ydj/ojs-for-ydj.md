# OJS for YDJ

## Introduction

!!! info

    **Last updated:** July 8, 2026
    This document has been ported from its [original site](https://pressbooks.library.yorku.ca/ojsforydj/) using YUL's instance of Pressbooks with minimal changes beyond formatting for the new platform. Most information here covers OJS 3.3 and 3.4, and is gradually being updated to reflect changes in OJS 3.5.

This documentation has two purposes: 

1. As a supplement the official documentation developed by PKP, to respond to frequently asked questions from YDJ editors, and
2. To describe YDJ-specific requirements, workflows, and standards.

You should see [PKP’s guide to OJS](https://docs.pkp.sfu.ca/) to learn more about what the fields and options mean on particular screens.

Unless otherwise noted, this guide refers to OJS 3. Where possible, this document notes the version of OJS on which each section is based. It is gradually being updated for OJS 3.5 as YDJ journals upgrade.

This guide has been created by Digital Publishing Librarian Tomasz Mrozewski at York University Libraries. Any errors are the author’s own. 

## The OJS site

!!! info

    **Last updated:** October 4, 2021

This sections deals with parts of the OJS site that don’t relate directly to issues or submissions. This includes page content and user roles. See also [PKP Docs](https://docs.pkp.sfu.ca/) for the developer’s documentation on how to work with OJS.

### Understanding the OJS homepage layout (Default Theme)

!!! info

    **Last updated:** August 9, 2022 for OJS 3.3.0.11

This chapter provides an overview of all possible elements that appear on the homepage of a journal using the OJS Default Theme. This chapter only discusses the layout of the homepage as viewed on a large screen, such as a computer or large tablet.

#### OJS homepage layout (Default Theme)

The page elements labeled in this screenshot are described in the next section.

![Annotated screenshot of the OJS homepage showing the relative location of site elements](/images/hompage-logo-ANNOTATED.png)

##### 1\. Header OR header background image

By default, OJS displays a coloured header at the top of the page that spans the entire window. The colour can be configured via **Website Settings > Appearance > Theme**, using the **Colour** field.

You can replace the entire header with an image if you follow two steps:

1.  Add a homepage image in **Website Settings > Appearance > Setup** in the **Homepage Image** field
2.  Click the checkbox under **Header Background Image** in **Website Settings > Appearance > Theme.**

If you use this option, you cannot have a regular homepage image (#6 below).

The screenshot on this page shows a journal homepage with the homepage image in the default location. You can also see an [example of the same journal with the homepage image used as a header background](/images/homepage-logo-background.png).

The header or header background image persist across all pages on the OJS site.

##### 2\. User navigation menu

The user navigation menu appears at the top right of the screen, against the backdrop of the header. When the visitor is logged out, this menu displays **Register** and **Login** buttons. When logged in, it displays the username as a dropdown menu with the links **Dashboard**, **View Profile**, and **Logout**.

The user navigation menu can be configured via **Website Settings > Setup > Navigation**, using the **Navigation** and Navigation Menu Items fields.

The user navigation menu persists across all pages on the OJS site.

##### 3\. Title OR logo

By default, OJS displays the title of the journal as an H1-level heading at the top left of the page, against the backdrop of the header. The title is configured via **Journal Settings > Masthead**, using the **Journal title** field.

You can display a logo image instead of the title of the journal. The logo is configured via **Website Settings > Appearance > Setup**, using the **Logo** field.

The screenshot on this page shows a journal homepage with a logo instead of the journal title. You can also see an [example of the same journal with the journal title instead of a logo.](/images/homepage-nologo.png)

The title or logo persist across all pages on the OJS site.

##### 4\. Primary navigation menu

The primary navigation menu appears under the journal title or logo, against the backdrop of the header and aligned to the left margin.

The primary navigation menu can be configured via **Website Settings > Setup > Navigation**, using the **Navigation** and Navigation Menu Items fields.

The primary navigation menu persists across all pages on the OJS site.

##### 5\. Search

The search tool appears under the journal title or logo, against the backdrop of the header and aligned to the right margin. The search tool cannot be configured.

The search tool persists across all pages on the OJS site.

##### 6\. Homepage image

The homepage image is an optional element. It will only appear if an image has been uploaded to **Homepage Image** in **Website Settings > Appearance > Setup**. The homepage image will appear in the central pane of the page, below the header.

The homepage image will only be displayed on the homepage.

The homepage image can also be used to replace the coloured header (#1 above) if you upload an image and click the checkbox under **Header Background Image** in **Website Settings > Appearance > Theme**. If you use this option, you cannot have a regular homepage image.

##### 7\. Blocks

Blocks appear in the right sidebar, below the header. Multiple blocks display in sequence vertically. Blocks are configured via **Website Settings > Appearance > Setup** using the **Sidebar** field. Some [plugins](#managing-plugins) may add blocks to your sidebar. You can also [create custom blocks](#adding-custom-blocks-to-the-right-sidebar) for your site.

Blocks persist across all pages of the OJS site.

##### 8\. Journal Summary

The journal summary is an optional element. If activated, the journal summary will appear in the central pane of the page, below the header. If a Homepage image is present (#6), it will appear below that image.

OJS automatically adds the heading "About the Journal" when the journal summary appears.

You can activate the journal summary if you follow two steps:

1.  Add the summary text in **Journal Settings > Masthead** using the **Journal Summary** field
2.  Click the checkbox under **Journal Summary** in **Website Settings > Appearance > Theme.**

The journal summary will only be displayed on the homepage.

##### 9\. Announcements

Announcements are an optional element. If activated, announcements will appear in the central pane of the page, below the header. If a homepage image (#7) or journal summary (#8) are present, it will appear below these elements.

You can activate announcements if you click the checkbox under **Announcements** in **Website Settings > Setup > Announcements** and click **Save.** You can then add announcements via **Announcements** in the left sidebar menu.

Even if announcements are activated, the announcement elements will _not_ appear on the homepage if:

*  The number in the *Display on Homepage* field at **Website Settings > Setup > Announcements** is set to 0, or
*  No announcements have been published, or
*  All published announcements have expired.

The announcements element will only be displayed on the homepage. However, activating the announcements feature will create a new page called Announcements and automatically added to it the primary navigation menu.

##### 10\. Current Issue

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

By default, your Current Issue is your most recently published issue; however, you can also [change your Current Issue](#setting-your-current-issue).

The current issue element will only be displayed on the homepage.

##### 11\. Additional Content

Additional content is an optional element. It will only appear if content has been added to **Additional Content** in **Website Settings > Appearance > Advanced**. The additional content will appear in the central pane of the page, below the current issue.

Additional content will only be displayed on the homepage.

##### 12\. Page Footer

By default, OJS displays a light grey footer at the bottom of the page that spans the entire window. The colour cannot be configured.

You can add content to the page footer via **Website Settings > Appearance > Setup**, using the **Page Footer** field.

The page footer persists across all pages on the OJS site.

##### 13\. PKP logo

By default, OJS displays the logo of the software developer, PKP, in the bottom left corner of the page against the backdrop of the footer. This logo cannot be configured.

The PKP logo persists across all pages on the OJS site.


### Managing your site's appearance


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

#### General settings

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

#### Theme and theme settings

Many elements of the OJS website are controlled by theme and the theme settings. These are configured through **Website Settings > Appearance > Theme.** When using the Default Theme, these settings are:

*   **Typography**: font combinations used on the site.
*   **Colour**: the colour of the site header.
*   **Journal Summary**: toggle whether the Journal Summary appears on the homepage.
*   **Header Background Image**: toggle whether the homepage image (if applicable) appears as the background of the header or in the main content pane.

YDJ prefers that participating journals use the Default Theme for two reasons:

1.  The Default Theme has been audited for accessibility and simplifies journals’ requirement to comply with the _Accessibility for Ontarians with Disabilities Act_ (AODA), whereas other themes may present accessibility issues, and
2.  Themes other than Default are not always updated with the core OJS software and may not render or function properly when YDJ upgrades your journal to a new version of the software.

If you wish to use or try out different themes for your journal, please contact the Digital Publishing Librarian. Themes are implemented as [plugins](#managing-plugins) and you will not be able to implement them without assistance. YDJ cannot customize themes or fix any problems with non-Default themes that may arise.

You can read more about [Theme settings](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#theme) in Learning OJS 3.3 and about [Theme Features and Design Elements](https://docs.pkp.sfu.ca/designing-your-journal/en/theme-features-design-elements) in Designing Your Journal. If you have access to development expertise, you can read about creating or modifying themes in the [PKP Theming Guide](https://docs.pkp.sfu.ca/pkp-theming-guide/en/).

#### Navigation menus

There are two navigation menus in the OJS Default Theme: the User Navigation Menu and the Primary Navigation Menu. Both menus are configured via **Website Settings > Setup > Navigation**. These menus may be rearranged; items may also be added or removed.

The **User Navigation Menu** contains a login link when site visitors are logged out or, when logged in, links related to their OJS user account. It appears at the top right of all OJS site pages when viewed in a large browser window; in a small browser window, these links are accessible via the hamburger menu at the top of the page.

The **Primary Navigation Menu** contains links to the public-facing site content, including About the Journal, Submissions, and Archives. It appears at the bottom of the site header on all OJS site pages when viewed in a large browser window; in a small browser window, these links are accessible via the hamburger menu at the top of the page alongsite the User Navigation Menu links.

You can edit each menu by rearranging, adding, and removing menu items. Be careful when removing menu items, lest you make important parts of the website inaccessible to readers. Adding a new **Navigation Menu Item** creates a new page on the OJS site that can be added to a menu.

You can read more about [Navigation settings](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#navigation) in Learning OJS 3.3.

!!! warning

    If you create a new page through the navigation menu, test your intended URL path first_ to ensure that you don’t create a site-breaking URL conflict.

#### Sidebar blocks

**Blocks** are flexible content containers that can appear to the right of the main content pane on any OJS page (on a large browser window) or below it (on a small browser windows). Blocks are managed via the **Sidebar** settings at **Website Settings > Appearance > Setup**, where you can reorder, activate, or deactivate blocks.

Several blocks are activated by default in OJS. Several [plugins](#managing-plugins) will also create blocks that can be managed via the Sidebar settings. One of these plugins is the Custom Block Manager, which allows you create custom block content. Learn more about [Adding custom blocks to the right sidebar](#adding-custom-blocks-to-the-right-sidebar) elsewhere in this guide.

#### Stylesheets

You can customize the deisgn of your OJS site by adding a .css file to **Journal style sheet**, which is accessed via **Website Settings > Appearance > Advanced**. You can read more about stylesheets in the [Create a Stylesheet](https://docs.pkp.sfu.ca/designing-your-journal/en/creating-stylesheet) section of Designing Your Journal.

YDJ cannot customize stylesheets or fix any problems with custom stylesheets that may arise. If your custom stylesheet causes accessibility problems, we will require you to edit your stylesheet; if the accessibility problems are serious enough, we may have to remove the stylesheet unilaterally in order to comply with AODA requirements.

### Adding custom blocks to the right sidebar

!!! info

    **Last updated:** November 22, 2021 for OJS 3.3.0.8

You can create custom blocks to appear in the right sidebar by following these steps:

1.  In the back end, go to **Website > Plugins**.
2.  On the Installed Plugins screen, you should see plugin called **Custom Block Manager** in the Generic Plugins section.
    1.  If you do not see the Custom Block Manager in that list, contact Tomasz to have it installed before proceeding.
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

### Managing plugins

!!! info

    **Last updated:** October 7, 2021 for OJS 3.3.0.8

Plugins provide extra functions in OJS. Some plugins are developed by the PKP community and are available through the OJS administrative interface; others are developed by third parties and must be uploaded manually.

#### Managing plugins

You can access your journal’s plugins through the **Plugins** tab on the **Website Settings** page. There, you will find two facets: Installed Plugins and Plugin Gallery.

**Installed Plugins** lists the plugins that are installed on your system but not necessarily activated. To activate them, you must click the checkbox to the left of the plugin’s name.

Most of the built-in plugins for OJS are updated when the core OJS software package is updated.

#### Installing and updating plugins

The **Plugin Gallery** lists optional plugins that you can install on your system and will also display whether updates are available. Only the OJS administrator can install and update plugins – you will not be able to do this for your own journal, even if you have the Journal Manager user role. If you wish to install or upgrade a plugin, please contact your Digital Publishing Librarian.

YDJ has not yet been able to automate the plugin update process for our journals, although we are currently working on this. Therefore, you may sometimes discover that certain plugins (such as [QuickSubmit](#using-the-quicksubmit-plugin) are not available due to an update being required. If this happens, please contact your Digital Publishing Librarian.

#### Third-party plugins

If you discover third-party plugins you wish to use, contact your Digital Publishing Librarian to discuss installing them. If YDJ has no immediately concerns about security or computing resources, we should be able to install them for you.

YDJ cannot support the use or maintenance of third-party plugins. In other words: if the plugin doesn’t work with the current version of OJS, or if the plugin doesn’t work as expected, or if you can’t figure out to use the plugin, we will be unable to support you. Additionally, if YDJ discovers that there is a major security concern with the plugin, we may have to unilaterally uninstall it.

### Web and readership statistics

!!! info

    **Last updated:** July 8, 2026 for OJS 3.5

This chapter covers two types of statistics:

* [Article and editorial statistics](#article-and-editorial-stats), which are collected and accessed through OJS itself, and
* [Web analytics](#web-analytics), which are collected by third-party applications.

#### Article and editorial stats

OJS offers robust statistical reporting tools for article views and downloads and for editorial activity as of version 3.2.

You can [learn about OJS’ built-in statistics reports](https://docs.pkp.sfu.ca/learning-ojs/en/statistics) in the _Learning OJS 3_ guide.

#### Web analytics

You should know that analytics packages only provide statistics as of the date of their implementation.

##### Matomo

YUL has implemented a locally-hosted instance of [Matomo](https://matomo.org/) for all journals as an alternative to Google Analytics. As of late 2023, Matomo has been configured for all YDJ publications. YDJ does not currently have standardized reporting procedures: if you would like to request stats from Matomo, please contact the Digital Publishing Librarian.

##### Google Analytics

Some YDJ journals created in OJS prior to 2019 used [Google Analytics Universal Analytics](https://analytics.google.com), which was shut down in 2024. YDJ no longer maintains Google Analytics accounts for journals and has replaced the service with Matomo.

### Changing user roles

!!! info

   **Last updated:** April 19, 2022 for OJS 3.3.0.10

To change the roles assigned to any user account, including your own:

1.  In the left navigation menu, click **Users & Roles** (under Settings)
2.  Search or browse to locate the account you wish to edit
3.  Click the blue triangle to the left of the user name and then click **Edit User**
4.  In the Edit User window, scroll down to User Roles and check/uncheck the roles as required
5.  Click **OK** to save your changes.

You must have the Journal Manager or Journal Editor role in order change user roles. However, you will not be able to change the YDJ admin account or certain special accounts created by and for YDJ staff.

### Reviewing user roles

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

### Adding sections

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

### Enabling and disabling notifications

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

## Submissions

!!! info

    **Last updated:** September 29, 2021

The submission is the other key element in OJS. As a noun, "submission" is a generic term that includes articles, book reviews, and art. A submission has its own page, one or more galleys, and metadata. It will appear in the table of contents for an issue when assigned to a published issue.

### Using the QuickSubmit Plugin

!!! info

    **Last updated:** July 28, 2025 for OJS 3.3.0.19 and OJS 3.4.0.7

QuickSubmit is a tool for uploading submissions that bypasses all stages of the workflow. Use it to upload content that does not required review (such as editorials) or if you conduct your review and editorial workflow outside of OJS.

**Important note:** do _not_ use this process to upload a single galley file of your full issue. Instead, see the instructions for [Adding a full-issue PDF galley](#adding-a-full-issue-pdf-galley).

Contents:

*   [Published or Unpublished: which option to use for your publication model](#published-or-unpublished-which-option-to-use-for-your-publication-model)
*   [Finding the QuickSubmit plugin](#finding-the-quicksubmit-plugin)
*   [Uploading submissions with the QuickSubmit plugin](#uploading-submissions-with-the-quicksubmit-plugin)
*   [Finding and editing submissions after completing QuickSubmit](#finding-and-editing-submissions-after-completing-quicksubmit)

#### Published or Unpublished: which option to use for your publication model

All publication in OJS happens at the _issue_ level, so using QuickSubmit alone does not necessarily publish the submission. There are three ways to publish the submission, depending on your publication model:

1.  In Step 7 below, select **Published** and then, in Step 8, assign the submission to a Back Issue or the Current Issue that has already been published: when you complete the process, the submission will immediately appear online as part of that issue.
2.  In Step 7 below, select **Published** and then, in Step 8, assign the submission to a Future Issue that has not yet been published: when you complete the process, the submission will appear online when you [publish the issue](#publishing-an-issue).
3.  In Step 7 below, leave the selection as **Unpublished**: you can then [find the submission at a later date](#finding-and-editing-submissions-after-completing-quicksubmit) and edit the details later to assign it to an issue.

#### Finding the QuickSubmit plugin

Once logged in, click **Tools** in the left-hand sidebar. This brings you to the Import/Expert tab of the Tools page. You should see **QuickSubmit Plugin** in the list of tools – if you do not, contact the Digital Publishing Librarian to have the plugin upgraded.

#### Uploading submissions with the QuickSubmit plugin

Use the form once for each submission.

1.  Choose **Submission Language**, if applicable
2.  Choose appropriate **Section**
3.  Full title goes in **Title**
4.  Add the **Abstract**, if applicable
5.  For each contributor, Click **Add Contributor** (button to the right of "List of Contributors")
    1.  In the Add Contributor window, enter the author’s **Name**.
    2.  Under **Contact**, you have two options for the email address you enter:
        1.  If this is a) the first publication of the submission and b) your journal uses the ORCID plugin, you should enter the author’s email address;
        2.  if this is not the first publication of the submission (ie, it was initially published on another platform) _or_ you do not use the ORCID ID plugin, you should enter your email address or a generic address. It will not appear on the journal website and the author will not receive potentially confusing email from the system.
    3.  Select the **Country** (this is a mandatory field but does not appear anywhere on the website).
    4.  Select the **Contributor’s Role**.
    5.  Then, click **Save**.
    6.  Repeat the Add Contributor process for all authors.
6.  Upload the article text (the galley) under Galleys. Click **Add galley**.
    1.  In the Create New Galley window, enter the file format under **Galley Label** (usually "PDF") and ensure the **Language** is properly set. Click **Save**.
    2.  Select the **Article Component**. This will almost always be **Article Text**. Then either drag the file from your desktop to the window or click **Upload File** to search for it.
    3.  Once the file name appears in the window with a green check, click **Continue**.
    4.  In the next tab, click **Continue**.
    5.  In the next tab, click **Continue**.
    6.  If you have galleys in other formats, repeat steps a-e with appropriate label.
7.  Select either **Unpublished** or **Published**. (NB: the Publish/Unpublished buttons are mislabeled – they should be Scheduled/Unscheduled).
    1.  If you wish to assign the submission to a Back Issue or Future Issue, select Published and continued to step 8.
    2.  If you wish to assign the submission to an issue at a later date, select **Unpublished** and skip to step 10. You must then [find and edit the submission](#finding-and-editing-submissions-after-completing-quicksubmit) by assigning it to an issue at a later date to publish it.
8.  In the **Schedule for publication** in drop-down, select the appropriate issue.
    1.  If you assign the submission to an issue that was already published, submission will be published when you click Save. If you assign the submission to a future issue, it will only be published when you publish the issue.
9.  Enter the Date of Publication under **Published** (likely today’s date).
10.  Click **Save**. You will be brought to a confirmation screen.

#### Finding and editing submissions after completing QuickSubmit

If you need to edit a submission after creating and saving it in QuickSubmit, you can find it in one of your submissions queues. Access your submission queues by clicking **Submissions** at the top of the left-hand navigation menu.

*   If you _did not_ assign an issue in step 7, the submission will appear in **All Active**. If you are retrieved the submission with the same account that uploaded it, it will also appear in **My Active**.
*   If you _did_ assign and an issue in step 7, the submission will appear in the **Archives** queue with the Scheduled status.

Once you find the submission in the proper queue, you can edit it. To edit the submissions:

1.  Click **View** to the right of the submission entry in the queue
2.  Click the **Publication** tab to edit the submission metadata, [upload or change the galley file](#adding-and-replacing-galleys), [change the section](#changing-the-section-of-a-submission), or assign it to an issue
3.  Click **Save** at the bottom of the screen after making any changes.

At the time of the latest update to this page, dates entered in QuickSubmit do not save when the submission was published: regardless of the date entered in step 8, it will be changed to the date the issue is published when you publish it. If you need to backdate submissions, please contact the Digital Publishing Librarian.

### Adding and replacing galleys

!!! info

    **Last updated**: September 29 for OJS 3.3.0.8

The galley is the final form of the article – editing, copy edited, and laid out – that is posted to the OJS site for reading. Galleys are usually uploaded as PDFs.

#### Adding a galley

Galleys are not brought forward from the submission’s Workflow tab. They must be manually added to the Galleys facet of the Publication tab.

To upload a galley for an submission:

1.  Open the submission and navigate to the **Publication** tab, then to the **Galleys** facet.
2.  Click **Add Galley**. This opens the Create New Galley window.
3.  Add the **Galley label**. This is typically the file format.
4.  Select the **Language**
5.  Click **Save.**
6.  Select the **Article Component**. This is usually "Article Text."
7.  Drag and drop the galley file from your desktop to upload area OR click **Upload File** and select the galley file from your file directory.
8.  Click **Continue.**
9.  Rename the file if you wish, the click **Continue**.
10.  Click **Complete**.

#### Replacing a galley

If the submission has already been published, you will need to [create a new version](#editing-a-submission-after-publication) in order to replace the galley. Replacing the galley constitutes a major change and requires a new version instead of unpublishing and republishing the submission.

1.  Open the submission and navigate to the **Publication** tab, then to the **Galleys** facet.
2.  Click the blue arrow next to the galley label and click **Change File**.
3.  In the first drop-down, select the file you wish to replace.
4.  Drag and drop the galley file from your desktop to upload area OR click **Upload File** and select the galley file from your file directory.
5.  Click **Continue.**
6.  Rename the file if you wish, the click **Continue**.
7.  Click **Complete**.

### Changing the section of a submission

!!! info

    **Last updated:** July 26, 2021 for OJS 3.3

To change the section to which a submission is assigned:

1.  Open the **Production** tab for the submission
2.  Open the **Issue** tab
3.  Use the drop-down menu under **Section** to change the Section.

### Editing a submission after publication

!!! info

    **Last updated:** September 12, 2022 for OJS 3.3.0.11

Go to **Submissions > Archive** to find a list of published submissions. You can search for articles by name or by submission ID.

Alternatively, you can find a link to submissions in the tables of contents of published issues via **Issues > Back Issues**.

1.  Click the submission title in the Archive.
2.  Open the **Publication** tab.
3.  Click either **Unpublish** or **Create New Version**
    1.  Use **Unpublish** if making minor changes or adding to the metadata of a submission (eg, updating the publication date or adding a reference list).
    2.  Use **Create New Version** if you’re making more substantive changes (changing the galley file, title, or contributor info) to a submission.
4.  Make edits in the Production sub-tabs, as required. Click **Save** at the bottom of each screen as you edit.
5.  When finished, click **Schedule for Publication**. The submission will be republished to the same issue.

#### Fixing the error: "the submission must be in the Copyediting or Production stages…"

When you attempt to republish or publish new versions of very old submissions, you may encounter an error message that says, "The submission must be in the Copyediting or Production stages before it can be published" (Figure 1). This may happen when submissions have been created and published through an earlier version of the QuickSubmit plugin, especially in OJS 2.

![Screenshot of error message: the submission must be in the Copyediting or Production stages before it can be published.](/images/screenshot-edit-error-1.png)

Figure 1: a screenshot of the error message that prevents some submissions from being re-published or having new versions published.

To resolve this error, you must assign an Editor to the submission and reapprove the submission for publication:

1.  Review the status of the Workflow sub-tabs:
    1.  In Submission sub-tab, the square above Participants should say "Assign an editor to enable the editorial decisions for this stage." There should be no Editor listed in the Participants area (Figure 2)  
        
        ![The Submission sub-tab says: Assign an editor to enable the editorial decisions for this stage.](/images/screenshot-edit-error-2.png)
        
        Figure 2: the Submission sub-tab shows that there is no Editor for this Submission
        
    2.  The Review sub-tab should say "The review process has not yet been initiated" (Figure 3)  
        
        ![The Review sub-tab says: The review process has not yet been initiated.](/images/screenshot-edit-error-3.png)
        
        Figure 3: the Review sub-tab shows that the Review stage has not yet been initiated.
        
2.  Assign the Editor to the submission:
    1.  In the Submission sub-tab, next to Participants click **Assign**
    2.  In the Assign Participant window that pops up, set the drop-down menu under **Locate Role** to the appropriate editorial role for your account
    3.  In the list of names, select your user account
    4.  Ensure the predefined message template and Message fields are blank
    5.  Click **OK**.
3.  Update the decision:
    1.  In the Submission sub-tab, click **Change decision**
    2.  Click **Accept and Skip Review**
    3.  In the Accept and Skip Review window that pops up, select **"Do not send an email notification"**
    4.  Click **Next: Select Files for Copyediting**
    5.  Click **Record Editorial Decision**. The page should reload at the Copyediting sub-tab.

You should now be able to republish or publish a new version of the submission.

### Adding data sets to articles

!!! info

    **Last updated:** July 29 for OJS 3.3

To upload a data set to OJS and make it available alongside the galley:

1.  Go to submission’s **Production** tab and click **Galleys.**
2.  Click **Add Galley**.
3.  In the Create New Galley window, enter the file format under **Galley Label**. You may wish to add a descriptive title in parentheses, eg, "CSV (data set)."
4.  Click **Save**.
5.  Select the "Data Set" in the **Article Component**.
6.  Upload the data set by dragging and dropping the file or clicking **Upload File_._**
7.  Click **Continue.**
8.  Edit the **Name the** file field, if necessary.
9.  Click **Continue**.
10.  Click **Complete**.

Once published, a link to the data set will appear on the submission’s metadata page (see Figure 1).

![An article&#039;s metadata page showing the link to the data set file](/images/data-set-galley-1.jpg)

Figure 1: Once published, a link to the uploaded data set will appear below the link to the Article Text galley.

If the data set is hosted in an external repository such as [York University Dataverse](https://dataverse.scholarsportal.info/dataverse/york), it is possible to link to the external site instead of republishing the data set in OJS. To link to an external data set:

1.  Follow steps 1-3 in the list above.
2.  Check the box labelled **This galley will be available at a separate website**.
3.  Enter the URL of the data set.
4.  Click **Save**.

Once published, a link to the data set will appear on the submission’s metadata page (see Figure 2).

![Article metadata page showing a link to the external data set](/images/data-set-galley-2.jpg)

Figure 2: Once published, a link to the external data set will appear next to the link to the Article Text galley.

### Adding DOIs to submission galleys before publication

!!! info

    **Last updated:** November 19 for OJS 3.3

If your journal has been configured for DOIs, you can easily determine what the DOI will be before you publish it. This way, you can add the DOI to the galley even though it is not possible to view the DOI before publication.

See the chapter on the [structure of DOIs](#determining-the-structure-of-your-dois) to determine what a submission's DOI will be and to transform the DOI into a URL. Once you have determined the DOI and transformed it into a URL, you can add the DOI to the galley as a link that will go live once the submission is published.

### Understanding and using Categories

!!! info

    **Last updated**: May 2, 2025 for OJS 3.3 and 3.4

The Category feature is best used as a browsing tool for readers that is distinct from Issues and Sections. It should be used in conjunction with the Browse Block or with navigation menu items.

When you create a Category, you do two things:

1.  You create a page for that Category, which includes a list of all articles assigned to it, as well as an optional description and cover image. (Example: [Category browse page](https://jat.journals.yorku.ca/index.php/default/catalog/category/parent1))
2.  You add a field to the submission’s metadata page, which links to the Category page. (Example: [submission metadata page](https://jat.journals.yorku.ca/index.php/default/article/view/97))

You can also nest Categories one level using Parent Category. Both the Parent Category and the nested Category will receive their own pages. The Parent Category page will link both to the submissions assigned to it and to the pages for the nested Categories.

Unlike sections, Categories do not appear in an issue’s table of contents and cannot be used to direct submissions to a particular editor. However, Categories can be used to make related content from across multiple issues in the same place. If you wish to make your journal content browsable by section, please request that the Digital Publishing Librarian install the Browse By Section Plugin.

#### Creating Categories

Create and edit Categories at **Journal Settings > Categories**.

#### Assigning submissions to Categories

If your journal has created any Categories, they will appear in the submission process for authors as well as in the QuickSubmit form. You can also edit the Category assignment in a submission’s **Publication > Issue** tab.

#### Making Categories discoverable

Categories should be used in conjunction with the Browse Block, which can be activated at **Website Settings > Appearance > Setup > Sidebar**. This sidebar block will automatically update as Categories are added, removed, or nested.

You may also also wish to manually create [Navigation Menu Items](#navigation-menus) for your Categories. However, these will not automatically update as Categories are added, removed, or nested.

## Issues

!!! info

    **Last updated:** September 29, 2021

The issue is one of the key elements of OJS. All content must be assigned to an issue in order to be published.

Even if you wish to use a continuous publication model in where you publish new submissions as soon as they are ready, you must assign the submissions to a published issue.

### Creating an issue

!!! info

    **Last updated:** July 26, 2021 for OJS 3.3

1.  Click **Issue** > **Future Issues** > **Create Issue**
2.  Enter the **Volume, Number, Year**, and **Title** information, as applicable to your journal
    1.  Follow the conventions previous established to identify each issue.
    2.  Use the checkboxes to select which of these 4 elements will be used to identify the issue in the issue title and in the list of issues in the Archive.
3.  Add a **Description** and upload a **Cover image** if desired
    1.  The Description will appear ahead of the Table of Contents for the issue and in the list of back issues in the Archives on the front end.
4.  Click **Save**.

You can now assign articles to the issue, but it will not be published yet.

### Publishing an issue

!!! info

    **Last updated:** July 26, 2021 for OJS 3.3

1.  Click **Issue** > **Future Issues**
2.  Click the small triangle to the left title of the issue you want to publish. You will now see several buttons below the title.
3.  Click **Publish Issue**.

### Reordering the issue Table of Contents

!!! info

    **Last updated:** July 26, 2021 for OJS 3.3

1.  Click **Issue** > **Back Issues** > **\[issue\]**. This will show you the details about the issue, opening on the Table of Contents Tab
2.  Click **Order**
3.  Drag and drop the articles into the correct order then click **Done**.

### Setting your Current Issue

!!! info

    **Last updated:** February 17, 2026 for OJS 3.3

Your Current Issue is that issue that:

*   displays on the journal’s homepage, and
*   is linked to from the **Current** item in the main navigation menu.

By default, your Current Issue is the most recently published issue. However, you may need to designate another issue as the Current Issue

!!! warning

    If you unpublish your Current Issue, no issue will be designated as Current and you will have to manually reassign it.

To manually set your current issue:

1.  In the back end, navigate to the **Back Issues** tab of the Issues page
2.  Click the blue arrow to the left of the issue you wish to make your Current Issue
3.  Click **Current Issue** under the name of the issue. _Note_: if you don’t see the Current Issue button, that means the issue is already designated as Current Issue.
4.  In the dialogue window, click **OK**.

### Changing the order of issues in your Archive

!!! info

    **Last updated:** July 20, 2020 for OJS 3.3.0.11

1.  Click **Issue** > **Back Issues**
2.  Click **Order**
3.  Drag and drop the issues into the correct order then click **Done**.

The issue at the top of the list of issues does not automatically become your Current Issue. If required, you should [update your Current Issue](#setting-your-current-issue) after changing the order.

### Adding a full-issue PDF galley

!!! info

    **Last updated:** July 28, 2025 for OJS 3.3 and 3.4

Never upload a PDF of your full issue as a submission. Instead, upload it as an _issue galley_.

To upload an issue galley:

1.  In the back end, go to **Issues**
2.  If the issue has not been published yet, stay on the **Future Issues** view; if it has already been published, click **Back Issues**
3.  Click the title of the issue to open the Issue Management window
4.  Click the **Issue Galleys** tab
5.  Click **Create Issue Galley**
6.  Upload the issue galley by clicking **Upload File** or by dragging and dropping the file from your desktop
7.  Under **Galley Label**, add the file format – usually, this will be "PDF"
8.  Select the **Language** of the issue. If multiple languages, choose the one that appears most often. You may also create multiple issue galleys if you have them in multiple languages.
9.  Click **Save**.

## Digital Object Identifiers (DOI)

!!! info

    **Last updated:** November 19, 2021
	
!!! warning

    This section describes DOI management and YDJ configuration in OJS 3.3. DOI management changed significantly as 3.4. the DOI creation mechanism was overhauled in OJS 3.4 and the workflow described on this page does not apply. Please see [the section on DOIs](https://docs.pkp.sfu.ca/learning-ojs/journal-managers/en/other-tools) from Learning OJS 3.5 for Journal Managers.

[Digital Object Identifiers](https://www.doi.org/) (DOIs) may be available for your journal. Please contact your Digital Publishing Librarian to find out if your journal is eligible.

YDJ registers DOIs through York University Libraries’ [Crossref](https://www.Crossref.org/) membership. Our membership specifies that we are obligated to publish [reference lists](https://www.Crossref.org/services/reference-linking/) for submissions which receive DOIs. This section includes a chapter on [how to upload and publish reference lists](#uploading-and-publishing-reference-lists).

### Determining the structure of your DOIs

This chapter explains the syntax of a DOI, how to determine the submission ID (a part of the DOI syntax), and how transform the DOI into a URL.

### DOI syntax

There are two parts to a DOI: a prefix and a suffix, separated by a slash.

The prefix for all YDJ DOIs is "10.25071."

The suffix for all YDJ DOIs is:

*   the ISSN of the journal
*   a period
*   the OJS submission ID.

For example, 10.25071/1920-7336.40655 is the DOI of a YDJ article. "1920-7336" is the ISSN of the journal and "40655" is the submission ID assigned by OJS.

OJS assigns every submission a unique, numeric ID as soon as it is created. By using the ISSN in combination with the submission ID, we ensure that there is no duplication of DOIs across journals or within the same journal.

### How to determine the submission ID

You can determine the submission ID by viewing the submission in the back end of OJS. The submission ID appears in two places (see Figure 1):

*   the portion of the URL following "/index/"
*   the running header of the submission, to the left of the author’s name

![The OJS interface showing the location of the submission IDs with red arrows](/images/find-submission-ID.png)

Figure 1: The location of the submission ID is indicated by the two red arrows. In this case, the submission ID is 40655.

The submission ID also appears in the URL of the submission once published.

### Turning a DOI into a URL

A DOI transforms into a URL by adding "http://doi.org/" at the start of the DOI. This sting is technically not part of the DOI; however, DOIs must be transformed into URLs to be useful to most readers.

For example, the URL for the DOI 10.25071/1920-7336.40655 is [http://doi.org/10.25071/1920-7336.40655](http://doi.org/10.25071/1920-7336.40655).

[_DOI Handbook_. 2: Numbering.](https://www.doi.org/doi_handbook/2_Numbering.html)

### Uploading and publishing reference lists

!!! info

    **Last updated:** November 19, 2021 for OJS 3.3.0.8
	
!!! info

    All journals receiving DOIs are obligated to publish reference lists in the metadata of articles with citations.

YDJ registers DOIs through York University Libraries’ [Crossref](https://www.Crossref.org/) membership. Our membership specifies that we are obligated to [publish reference lists](https://www.Crossref.org/services/reference-linking/) for submissions which receive DOIs. This chapter explains how to publish reference lists with your submissions in order to comply with this requirement.

If your journal provides DOIs but does not publish reference lists for new submissions, YDJ may need to cease provision of DOIs for your journal.

#### Reference list setup

To publish reference lists, you must first make a policy decision and then make a corresponding change to the configuration of OJS.

The policy decision is a choice between three alternatives:

1.  Are editors solely responsible for uploading reference lists?
2.  Are authors _requested_ to upload reference lists with their initial submission? In this case, editors are responsible for uploading reference lists if the author does not.
3.  Are authors _required_ to upload reference lists with their initial submission?

If you chose the options 2 or 3, you may wish to update your Submission Checklist and Author Guidelines.

Once you have made your policy decision, you must implement this in OJS:

1.  Go to **Workflow Settings** > **Submission** > **Metadata**
2.  Under References, check the box for **Enable references metadata**
3.  Select the radio button corresponding to your policy choice
4.  Click **Save**.

If you chose policy options 2 or 3, the references metadata field will now appear in the regular submission and [QuickSubmit](#using-the-quicksubmit-plugin) interfaces. In all cases, the reference metadata field will now appear in the Metadata facet of the submissions Production tab.

#### Reference list format

The reference lists are style-agnostic. This means the reference lists can be uploaded in any citation agnostic.

Each reference in the list should start on a new line.

!!! tip

    We recommend that you or your authors remove all DOIs from the reference lists prior to publication. The Crossref Reference Linking Plugin, which the Digital Publishing Librarian will configure when setting you up for DOIs, will automatically search for and include DOI links for any reference in the list with a DOI. If there are already DOIs in the reference list, those references may display 2 DOI links.

#### Publishing the reference lists

The reference lists are published with the submission metadata as soon as the submission is published. The editors only need to get involved if the authors do not provide the reference lists themselves.

### Creating and registering DOIs

!!! info

    **Last updated:** June 4, 2025 for OJS 3.3.0.19

There are two steps to adding DOIs to your submissions:

1.  [Creating DOIs](#creating-dois) (also called "minting"): creating and assigning a unique DOI for the submission, which includes the DOI prefix for YUL and the unique string to identify the submission.
2.  [Registering DOIs](#registering-dois): registering DOI with Crossref (the registration agency with whom YUL is partnered) is required to make DOI links behave like DOIs and redirect to the OJS page for the submission.

In most cases, you will create DOIs manually and DOIs will register automatically; however, in some cases you will need to register DOIs manually.

#### How to create and register DOIs according to publication model

| Publication model | Creating DOIs | Registering DOIs |
| --- | ---| --- |
| Standard publication: new submissions are published for the first time via a new issue | Manual | Automatic |
| Online First/Forthcoming publication or rolling publication: new submissions are published for the first time after the issue is published | Manual | Manual |

In rare cases, you may need to [create DOIs in bulk](#optional-creating-dois-in-bulk). In OJS 3.3, this can only be done after publication.

#### Creating DOIs

In most cases you create DOIs for each submission manually when preparing for publication. Using this method, you should create the DOI to the submission _before_ publishing it; otherwise you will need to [edit each submission after publishing](#editing-a-submission-after-publication) unless you use the bulk method described below.

To manually create a DOI for a submission:

1.  In the back end of OJS, go to the submission’s **Publication** tab
2.  Click the **Identifiers** tab
3.  On the Identifiers tab, you should see the heading DOI with a blank text input field below it and a button labeled Assign. Click **Assign**.
4.  When you click Assign, a DOI will appear in the input field. Click **Save** to finish.

Once the submission is published, the DOI must be [registered](#registering-dois).

##### Optional: creating DOIs in bulk

If you create DOIs to multiple submissions after publication, you can use the bulk method. In OJS 3.3, this can only be done _after_ publishing the submissions.

To create DOIs in bulk:

1.  In the back end of OJS, click **Tools** near the bottom of the left sidebar
2.  In the list of tools, click **Crossref XML Export Plugin**
3.  In the Settings tab of the Crossref XML Export Plugin, click **DOI Plugin Settings**
4.  In the DOI Plugin Settings window, click **Assign DOIs.** The page will appear to be loading for several moments once you do this
5.  Click **Save**. You will now return to the Crossref XML Export Plugin page.
6.  Follow the instructions for Registering DOIs manually, below.

After you create DOIs in bulk, you must [register them manually](#manual-doi-registration) (described below).

#### Registering DOIs

Once you have created  the DOIs, you must register them to ensure that they function as DOIs. This allows the DOI URL to redirect to the publication page, and allows Crossref to track citations.

##### Automatic DOI registration

If your journal uses the standard, basic form of publication (submissions are published for the first time when a new issue is published), the DOIs should automatically be registered once a new issue is published.

However, sometimes the DOIs don’t register automatically for unknown reasons; if this happens, you will need to register the DOIs manually. Note: DOI registration takes some time to complete; please wait up to an hour before checking to see if the DOIs have registered.

##### Manual DOI registration

If your journal uses an Online First/Forthcoming or a rolling publication model, or if the DOIs do not register manually, you will need to _create and assign_ and _register_ the DOIs manually.

To register DOIs manually:

1.  1.  In the back end of OJS, click **Tools** near the bottom of the left sidebar
    2.  In the list of tools, click **Crossref XML Export Plugin**
    3.  On the plugin page, click the **Articles** tab. If your journal has a large number of articles, it may take some time to load
    4.  In the Articles tab, click **Search**. This will show several new drop-down menus above the list of articles
    5.  Select that drop-down menu that says **Any Status** and change it to **Not Deposited**
    6.  Click **Search**. You should now see a list only of published submissions that have DOIs assigned but are not registered
    7.  Check the boxes for each submission you wish to register in the Select column
    8.  Click **Deposit**

If you received any error messages that you cannot understand and address, please contact the Digital Publishing Librarian for assistance.

### DOIs and QuickSubmit

!!! info

    **Last updated:** July 28, 2025 for OJS 3.3.0.19

After you add submissions to a future issue through [QuickSubmit](#using-the-quicksubmit-plugin), you should manually assign the DOIs for each article before publishing the issue.

To find the submissions and assign DOIs:

1.  In the back end, go to **Issues > Future Issues**
2.  Click the title of the issue to view the assigned submissions
3.  In the table of contents, click the blue triangle to the left of the submission title to see the additional options
4.  Click **Submission** to see the submission workflow and publication metadata
5.  Click **Publication** to open the publication tab
6.  Click **Identifiers**
7.  Under the DOI heading, click **Assign** next to the blank text box. The predetermined DOI will appear in the text box
8.  Click Save
9.  Repeat steps 3-8 for all submissions assigned to the issue.

The DOIs will register automatically upon publication of the issue.

## Alternative publication models

!!! info

    **Last updated:** November 18, 2021 for OJS 3.3.0.8

There are two common alternatives to the regular, full issue publication model: online first, and rolling.

In the **online first** publication model (also called "forthcoming"), you publish each submission as soon as it is ready. Later, you assign these submissions to a regular, numbered issue – often with additional contents such as reviews, editorial, etc. You can [use an online first model](#publishing-submissions-in-advance-of-regular-issues-online-first-or-forthcoming) in OJS but this requires several added steps.

In the **rolling publication** model (also called "continuous publication"), you [create](#creating-an-issue) and "open" a new, regular issue by [publishing it](#publishing-an-issue) at the beginning of a publication cycle – often, the calendar year. You then add each new submission to the issue as soon it is ready. At the end of the cycle, you "close" the issue and open a new one. To close an issue, just stop adding submissions.

The key distinction between this models is these:

*   with an online first model, you "move" submissions from the online first collection to a regular, numbered issue at a certain point;
*   with a rolling publication schedule, the articles stay assigned to the same issue.

In both cases, the URLs for the submissions stay the same once published in OJS.

Online first and rolling publication both introduce two small complications for OJS:

1.  **DOIs.** Normally, OJS assigns and registers DOIs for submissions when a new issue is published. However, in both of the models, issues are published before the articles. That means you have to [manually assign and register DOIs](#adding-dois-for-online-first-or-rolling-publication-models) for submissions.
2.  **Notifications**. OJS gives you the option of notifying your journal’s regular users about the publication of a new issue. Because the submissions are published separately from the issues, you cannot notify your users about the publication of new submissions. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

### Publishing submissions in advance of regular issues: "online first" or "Forthcoming"

!!! info

    **Last updated:** February 21, 2025 for OJS 3.3 and 3.4

**Important update:** the [Forthcoming plugin](https://github.com/ajnyga/forthcoming) has been updated for OJS 3.3 and 3.4 and is a much simpler solution than the instructions provided below. These instructions are retained for reference.

Please contact the Digital Publishing Librarian to have the plugin installed and configured.

OJS does not have a dedicated mechanism for publishing "online first"/"forthcoming" articles but it’s possible to cheat the issue publication process to mimic the feature. The following steps explain how to publish submissions under the label "Online First" in advance of a regular, numbered issue.

Here’s what you get by following this process:

*   New submissions published as soon as they are ready
*   Stable links and DOIs (if applicable) for the submissions
*   Links to Online First through the navigation menu, the Archive, and through a custom sidebar block (optional)
*   Your most recent, regular issue appears as your Current Issue.

There are three components to this process:

1. [Initial setup of Online First](#initial-setup-of-online-first)
2. [Publishing submissions to Online First](#publishing-submissions-to-online-first)
3. [Reassigning submissions to a regular issue](#reassigning-submissions-to-a-regular-issue)
4. [Reordering issues in archives](#changing-the-order-of-issues-in-your-archive)

#### Initial setup of Online First

Follow these steps just once, when you commit to using an online first publication model.

You must create and publish your Online First issue, and create a Navigation Menu Item linked to that issue. You can also create a custom sidebar block linked to Online First as well.

1.  Create your Online First issue:
    1.  Follow the [steps for creating an issue](#creating-an-issue)
    2.  In Step 2 of Creating an Issue, use the title "Online First" and select only the **Title** checkbox.
2.  [Publish](#publishing-an-issue) the Online First issue.
3.  Change your Current Issue back to your most recent, regular issue:
    1.  Go to **Issues** > **Back Issues**
    2.  Click the blue arrow beside the title of your most recent, regular issue
    3.  Click **Current Issue**
    4.  Click **OK**.
4.  Create the Navigation Menu Item:
    1.  Go to **Website Settings** > **Setup** > **Navigation**
    2.  Next to Navigation Menu Items, click **Add Item**
    3.  In the **Title** field, write "Online First"
    4.  Under **Navigation Menu Type**, select **Remote URL**
    5.  In the **URL** field that just appeared, paste the full URL of your Online First issue  
        **Note for multilingual journals:** you must paste the same URL in the field for each language activated for your journal.
    6.  Click **Save**.
5.  Add the Navigation Menu Item to the Primary Navigation Menu:
    1.  Under Navigation, click **Primary Navigation Menu**
    2.  Drag Online First from the **Unassigned Menu Items** column to the **Assigned Menu Items** column
    3.  Ensure that the container box for Online First is flush against the left-hand side of the Assigned Menu Items column; if it is indented, it will be nested under the menu item above it
    4.  Click **Save**.
6.  Optional: create a custom sidebar block:
    1.  Follow the steps for [creating a custom block](#adding-custom-blocks-to-the-right-sidebar) with the title "Online First"
    2.  In the **Content** field, write "Online First"
    3.  Link the text in the Content field to your Online First issue
    4.  Keep the box under **Show Name** unchecked.

Online First is now a published issue without any submissions that appears in the navigation menu, in the Archives and, optionally, in a custom block in the right sidebar. You can now publish submissions to this issue as they are ready.

#### Publishing submissions to Online First

Follow these steps every time you wish to publish a new submission to Online First.

When you have completed the editorial and production workflow for the submission, you can assign it the Online First issue to have it published immediately.

1.  If your journal’s submissions receive DOIs, manually [assign the DOI](#creating-dois) to the submission
2.  Go to **Production** > **Issue** for the submission
3.  Under the Issue heading, click **Assign to Issue**
4.  Select Online First from the drop-down menu
5.  Click **Save**
6.  A notification saying "All publication requirements have been met" will appear. Click **Publish.**
7.  If your journal’s submissions receive DOIs, manually [register the DOI](#register-the-doi-with-crossref).

The submission will now be published in Online First. If the submission has a DOI, the DOI will now be registered and functional.

You cannot use OJS’s built-in notification to notify your readers about newly published submissions – it only sends notifications for new issues. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

#### Reassigning submissions to a regular issue

Follow these steps when you are ready to publish a complete, regular issue.

You must reassign the articles from Online First to the new issue, publish the new issue, and then reorder your list of issues.

1.  [Create a new, regular issue.](#creating-an-issue)
2.  Unpublish the submissions from Online First:
    1.  Go to **Issues** > **Back Issues**
    2.  Click Online First
    3.  In the Table of Contents, click the blue arrow next to the title of the submission your wish to reassign and then click **Remove**
    4.  Repeat step 2.iii for all submissions you wish to reassign to the new, regular issue.
3.  Reassign the submissions to the new issue:
    1.  Find the submission(s) you wish to reassign in **Submissions** > **My Queue** or **Submissions** > **All Active**
    2.  For each submission, go to **Production** > **Issue**
    3.  Under the Issue heading, click **Change Issue**
    4.  Select the new issue from the drop-down menu
    5.  Click **Save**
    6.  A notification saying "All publication requirements have been met" will appear; however, the submission will not be republished until you publish the new issue. Click **Publish.**
    7.  If you are updating the galley to include volume, issue, and page number, you may now do so in the **Galleys** tab. Under the galley file name, click **Change File** and follow the process to replace the file.
    8.  Repeat steps 3.i-3.vii for all submissions you wish to reassign to the new, regular issue.
4.  [Publish the new issue](#publishing-an-issue).
5.  Reorder your list of issues:
    1.  Go to **Issues** > **Back Issues**
    2.  Click **Order**
    3.  Drag Online First to the top of the list of issues
    4.  Click **Done**.

The submissions that were previously published in Online First will now appear in OJS as part of the new issue. However, the URLs and DOIs for the published submissions will remain unchanged.

You cannot show the contents of both your Online First issue and your most recent, regular issue on your journal’s homepage. OJS only displays the contents of the Current Issue on your journal’s homepage, and only one issue can be designated at the Current Issue. You must therefore designate either Online First or your most recent, regular issue as your Current Issue; YDJ advises designated the regular issue as the Current Issue. While it may be _technically_ possible to display more than one table of contents but YDJ does not have the resources to customize OJS like this or to support the customization.

If you skip this step, the empty Online First issue will appear on your OJS homepage. This may create the impression that your journal is inactive or that there is a problem with the website.

By default, each newly published issue appears at the top of the list of issues in the Archive. This step ensures that Online First remains that the top of the list in the Archive.

### Continuous publication in a regular issue: "rolling publication"

!!! info

    **Last updated:** November 18, 2021 for OJS 3.3.0.8

OJS allows you to assign a submission to an issue that has already been published. Doing so immediately publishes the submission. Therefore, implementing a rolling publication model is simple in OJS.

To implement a rolling publication model:

1.  Determine your publication cycle (e.g., annual).
2.  At the beginning of the publication cycle, [create a new issue](#creating-an-issue).
3.  [Publish the issue](#publishing-an-issue).
4.  When you have completed the editorial and production workflow for a submission, publish it be assigning it to the current issue in **Publication** > **Issue**. The submission will now appear be live on the OJS site.
5.  Repeat step 4 until the end of the publication cycle.
6.  At the end of the publication cycle, return to step 2.

If your journal provides submissions with DOIs, you must [manually assign and register the DOI](#adding-dois-for-online-first-or-rolling-publication-models) for each new submissions you publish.

If you use the rolling publication model, you cannot use OJS’s built-in notification to notify your readers about newly published submissions – it only sends notifications for new issues. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

You may wish to delay publication of the new issue until you have a submission ready to publish in the new publication cycle. This will prevent OJS from displaying an empty table of contents on your journal’s homepage.

Unless you have assigned a submission when you first publish the issue (see footnote 1). In this case, OJS will automatically assign and register the DOI.

#### Adding DOIs for online first or rolling publication models

!!! info

    **Last updated:** November 12, 2021 for OJS 3.3.0.8

If you publish a submission after the publication of the issue – for example, if you have a rolling publication schedule – the DOIs will not be automatically assigned and registered. You must perform two small tasks to do this manually.

##### Assign the DOI prior to publishing the submission

1.  Open the submission’s **Publication** tab
2.  Go to the **Identifiers** facet
3.  Click **Assign**, next to the DOI field
4.  Click **Save**.

**Note:** if you forget to assign the DOI prior to publication, you can perform these steps by [editing the submission after publication](#editing-a-submission-after-publication).

##### Register the DOI with Crossref

1.  In the back end of OJS, click **Tools** in the left-hand menu
2.  Open the **Crossref XML** Export Plugin in the list of Tools
3.  Click the **Articles** tab. Your newly published submission should appear at the top of the list with the status Not Deposited
4.  Click the checkbox for the submission
5.  Scroll to the bottom of the page and click **Deposit**
6.  Wait for the page to reload. If registration is successful, you have completed the process. If you get an error message, please notify the Digital Publishing Librarian.

**Note:** this must be performed by a user with the Journal Editor or Journal Manager role

### Bypassing the editorial workflow in OJS

!!! info

    **Last updated:** July 28, 2025 for OJS 3.3 and 3.4

This page is intended for journal editors who perform the editorial workflow (submission, review, copyediting, or layout production) outside OJS and only wish to use OJS to host the finished materials.

The individual steps of this process are covered elsewhere in this guide but linked here:

1.  [Create a new issue](#creating-an-issue): before uploading the journal contents, you want to create the future issue in which they will be published. This is because the QuickSubmit plugin (step 2) allows you to assign the contents directly to an issue.
2.  [Upload the contents using QuickSubmit](#using-the-quicksubmit-plugin): use the QuickSubmit plugin to upload each new submission (article, editorial, review, etc.) to OJS. Do _not_ use this to upload a single, full-issue galley.
    1.  In step 7, you will want to select **Published** in order to assign the content to the new, unpublished issue you created previously.
3.  [Assign the DOIs to the articles](#dois-and-quicksubmit): do this after you have uploaded all the contents.
4.  [Upload the full-issue galley (optional)](#adding-a-full-issue-pdf-galley): if you have a single galley file containing all the issue contents, upload it here.
5.  [Publish the issue](#publishing-an-issue): once you have added all contents to the new issue, you can publish the issue.

### Publishing audio or video journal content

!!! info

    **Last updated:** March 31, 2026 for OJS 3.3.0-22

YDJ allows you to publish audio or video media content in a journal issue by embedding it in an HTML galley.

There are three parts to this:

*   Submission and review
*   Hosting the media files, and
*   Embedding the stream in a galley.

#### Submission and review

OJS is not well-equipped to accept large media files as submissions files. Therefore, if your journal accepts multimedia submissions, YDJ recommends creators share their media files with the editors outside of OJS.

#### Hosting the media files

Media files may be hosted locally through [York University Digital Library (YUDL)](https://digital.library.yorku.ca/) or externally via third-party service. If possible, YDJ prefers to host a copy of the media file in YUDL. This ensures that the media will be preserved in accordance with the YUL’s [Digital Preservation Policy](https://www.library.yorku.ca/web/about-us/library-policies/digital-preservation-policy/) and that the link will remain stable.

Content creators/owners must agree to the York University Digital Library Distribution Licence (available upon request) to have their material preserved in YUDL. If they do not agree to the terms, the media files must be hosted elsewhere.

##### Hosting through York University Digital Library

If hosting with YUDL, the editor must return the YUDL Distribution Licence and the following information to YDJ:

*   Copyright holder
*   Rights statement, such as a [Creative Commons license](https://creativecommons.org/share-your-work/cclicenses/), [RightsStatement.org statement](https://rightsstatements.org/en/), or [Traditional Knowledge label](https://localcontexts.org/labels/traditional-knowledge-labels/)

The Digital Publishing Librarian will direct you on the best method for sharing the media file.

##### External hosting

It is also possible to link to an external host (such as YouTube, Vimeo, or Soundcloud). Externally hosted media is subject to the provider’s terms of use. External hosts may not provide media files with a stable URL or preserve them indefinitely; therefore, it is possible that the media stream in OJS breaks. It is the journal’s responsibility to monitor the media stream and to have the galley updated, if required.

#### Embedding the stream in a galley

However you choose to host the media files, please provide the following metadata to the Digital Publishing Librarian:

*   Title
*   Author/creator(s)
*   Text description

YDJ will embed the stream to the media file in an HTML galley. YDJ will create the media galley and share it with the editor for uploading.

The galley will include:

*   The title of the work
*   The creator(s) of the work
*   A text description of the work.
*   Publication and issue information.

The media is embedded in such a way that, if it fails to render properly, it will be replaced by a link to the original media file.

## Accessibility

!!! info

    **Last updated:** September 24, 2021.

As of January 1, 2021, all YDJ sites and article galleys published after January 1, 2012 must comply with the [_Accessibility for Ontarians with Disabilities Act_ (AODA)](https://www.ontario.ca/laws/statute/05a11).

AODA requirements for websites are based on the [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/standards-guidelines/wcag/) version 2.0, level AA. You can find a quick reference guide called [How to Meet WCAG](https://www.w3.org/WAI/WCAG21/quickref/) online but you may find that this is overly technical and complex for your purposes: WCAG covers content types and technologies not used with OJS, and many WCAG requirements are covered by the OJS platform itself.

The best starting point for making accessible, AODA compliant content in OJS is PKP’s [Creating Accessible Content: A Guide for Journal Editors and Authors](https://docs.pkp.sfu.ca/accessible-content/en/) guide. Although the guide does not cite AODA, it is based on the WCAG standards used by AODA. The guide is most applicable to article galleys, but the same principles apply to content on the OJS site itself.

You should also refer to the [Inclusive and Accessible Theming](https://docs.pkp.sfu.ca/designing-your-journal/en/inclusive-and-accessible-theming) guide to understand how to keep make and keep your OJS pages accessible.

### Accessible styling in Word

!!! info

    **Last updated:** September 24, 2021

One of the most important things you can do to make your article galleys accessible is to tag the title and headings in your article galley. This structures your document so that it can be parsed and browsed by readers using assistive technologies such as screen readers.

In Word, you add these title and heading tags by using styles. The easiest way to access styles is through the Styles pane in the Home toolbar (Figure 1).

![The Styles pane in Microsoft Word](/images/Word-Styles-pane-marked-1.jpg)

Figure 1: the Styles pane in Microsoft Word.

Styles have two functions:

1.  they dictate the design and layout of the text, and
2.  they apply semantic tags that structure the document.

The second function is the most important one for accessibility purposes.

If you have already chosen the font and paragraph layout for your headings you haven’t applied the styles, you can match the style to your design by following the steps described in [Updating styles to match formatted text](#updating-styles-to-match-formatted-text), below.

#### Applying styles to text

To apply styles to your text, select the relevant text and then click the appropriate style in the Styles pane. Alternatively, you can click on a style and then start typing: the text you type will use that style.

In more recent versions of Word, a button to access styles may appear automatically alongside other formatting options above highlighted text.

See also: [Apply styles](https://support.microsoft.com/en-us/office/apply-styles-f8b96097-4d25-4fac-8200-6139c8093109) from the Microsoft Word Help & Training site.

#### Heading structure

Your title and heading styles must be applied in a hierarchical and logical way. The title of the article must use the Title style; first-level headings must use the Heading 1 style; second-level headings must use the Heading 2 style, etc. You must not skip heading levels for the sake of design.

#### Updating styles to match formatted text

If you have already formatted your text before applying the styles, you can update the appearance of the title and heading styles to match your formatting.

To update styles based on your document formatting:

1.  Select the text of your title or a heading (number 1 in Figure 2)
2.  Right-click the appropriate style in the Styles pane (number 2 in Figure 2)
3.  Click "Update \[style\] to Match Selection" (number 3 in Figure 2)

![The styles pane in Word, showing the option to update a style to match text formatting](/images/word-styles-modify-1.png)

Figure 2: when you right-click a style in the Style pane, you have the option to update the style to match selected text.

Once you have updated your styles, you can then select all of the title and heading text in your document and apply the styles where required (see [Applying styles to text](#applying-styles-to-text), above).

See also: [Customize or create new styles](https://support.microsoft.com/en-us/office/customize-or-create-new-styles-d38d6e47-f6fc-48eb-a607-1eb120dec563) from the Microsoft Office Support site.

#### Creating article templates in Word

!!! info

    **Last updated:** August 20, 2025

Although doing article design and layout in Microsoft Word may not seem like a professional approach, there are significant advantages to using it:

*   **Design features:** Word features Themes that configure design elements such as font family, colours, and styles so that the articles won’t look like default Word output. You can also customize and create new Themes for your journal. Learn more about [Styles and Themes](https://support.microsoft.com/en-us/office/design-and-edit-in-word-bc819ecd-9887-4a15-8eda-d90cbc58f8fb) and about [customizing Themes](https://support.microsoft.com/en-us/office/change-a-theme-and-make-it-the-default-in-word-or-excel-c846f997-968e-4daa-b2d4-42bd2afef904) in Word.
*   **Templates:** You can create article templates in Word that you can apply to your submissions and that you can share with your fellow editors. Templates include Theme and Style information, and allow you to lay out standard elements such as journal information, article metadata, and copyright/licensing info. Learn more about [working with templates](https://support.microsoft.com/en-us/office/create-a-template-86a1d089-5ae2-4d53-9042-1191bce57deb) in Word.
*   **Accessibility:** Word includes many features to help you make documents accessible. Tools include [title, sub-title, and heading styles](https://support.microsoft.com/en-us/office/make-your-word-documents-accessible-to-people-with-disabilities-d9bf3683-87ac-47ea-b91a-78dcacb3c66d#bkmk_builtinheadings_win), easily editable [alt-text for images figures](https://support.microsoft.com/en-us/office/make-your-word-documents-accessible-to-people-with-disabilities-d9bf3683-87ac-47ea-b91a-78dcacb3c66d#bkmk_altvisuals_win), and an [Accessibility Checker](https://support.microsoft.com/en-us/office/improve-accessibility-with-the-accessibility-checker-a16f6de0-2f39-4a2b-8bd8-5ad801426c7f#PickTab=Windows&picktab=windows). You can preserve many of these accessibility features in your galley PDF by using the option to save a file as a PDF (_not_ printing as PDF). Learn more about [creating accessible documents in Word](https://support.microsoft.com/en-us/office/make-your-word-documents-accessible-to-people-with-disabilities-d9bf3683-87ac-47ea-b91a-78dcacb3c66d) more generally, and see also PKP’s guide on [creating accessible journal content](https://docs.pkp.sfu.ca/accessible-content/en/).
*   **Sustainability:** Word is widely used and most editors already have some experience with it. The learning curve for features such as Styles, Designs, and Templates will be move quicker than for more specialized software. Because it is so widely used, you can easily search the web for help and ideas. In addition, many universities provide students and faculty with free or discounted access to the Word. Other software such as InDesign is difficult to learn, requires significant work to make its outputs accessible, and may be prohibitively expensive.

## Metrics

This section discusses the various metrics available to you as a YDJ journal.

### Altmetric Explorer

!!! info

    **Last updated:** March 3, 2022 for OJS 3.3.0.8

YDJ journals have access to altmetric data through [YUL’s subscription to Altmetric Explorer](https://www.library.yorku.ca/web/research-metrics/altmetric-explorer/). York-affiliated editors can access [Altmetric Explorer directly](https://www.altmetric.com/explorer/login). Editors without a York University affiliation can request reports for their journal from the [Digital Publishing Librarian](mailto:tmrozews@yorku.ca).

In order to get altmetric data for your journal in Altmetric Explorer, your journal must:

1.  Receive [DOIs](#digital-object-identifiers-doi), and
2.  Be tracked by Altmetric.

The Digital Publishing Librarian can make sure that your journal is tracked by Altmetric.

At present, there is no functional integration of Altmetric Explorer and OJS. This means that it isn’t possible to display data from Altmetric on your journal’s OJS site.

## Configuring subscription settings

!!! info

    **Last updated:** January 24, 2022 for OJS 3.3.0.8

This page tells you how to configure the 2 parts of OJS required to properly use the subscription module:

1.  [The Payments tab under Distribution Settings](#distribution-payments-page), and
2.  [The Payments page in the left-hand menu](#payments-page).

You must enable payments via Distribution > Payments in order for the Payments _page_ to appear.

You must complete both of these tasks for the Subscriptions page to appear on the front-end of the OJS site. By default, Subscriptions will appear in the About menu. If a link to the Subscriptions page does not appear under the About menu, you should ensure that both of these tasks are complete. You should also ensure that Subscriptions appears in the Assigned Menu Items list of your [navigation menu](https://docs.pkp.sfu.ca/learning-ojs/en/settings-website#navigation).

### Distribution > Payments page

1.  In the back end, click **Distribution** in the left-hand menu
2.  Click on the **Payments** tab
3.  Click the checkbox under **Enable.** Additional content will now appear on the page
4.  Using the **Payment Plugins** dropdown, select either **Paypal Fee Payment** or **Manual Fee Payment**
5.  Complete the fields for Paypal Fee Payment or Manual Fee Payment, as appropriate
6.  Click **Save.**

Once you complete step 6, a new link called **Payments** will appear in the left-hand navigation menu under Submissions, Issues and, if it is active, Announcements (see Figure 1).

![The Payments link appears after the links for Submissions, Issues, and Announcements.](/images/left-menu-link-to-Payments-page.jpg)

Figure 1: The Payments link appears after the links for Submissions, Issues, and, Announcements (if  active).

### Payments Page

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


## Glossary

[Current Issue]: The Current Issue is the issue that appears on the front page of your OJS site. When a new issue is published, it is automatically set as Current Issue. However, you can manually set the Current Issue through the Back Issues page in the back end.

[galley]: The galley is the final form of the article - editing, copy edited, and laid out - that is posted to the OJS site for reading.

[issue]: Along with submissions, one of the building blocks of OJS. All submissions (articles, reviews, editorials, etc.) must be assigned to an issue in order to be published.

[QuickSubmit]: QuickSubmit is a tool for uploading submissions that bypasses all stages of the workflow.

[YDJ]: York Digital Journals - the York University Libraries program that provides journal hosting services.
