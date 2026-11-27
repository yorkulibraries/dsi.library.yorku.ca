# Alternative publication models

!!! info

    **Last updated:** November 25, 2026 for OJS 3.5.

There are two common alternatives to the regular, full issue publication model: online first, and rolling. OJS 3.5 does not support these models by default, although it is possible to make them work with the somewhat complex processes outlined in this chapter. Note that these functions should be supported natively as of [OJS 3.6](https://pkp.sfu.ca/2026/11/17/ojs-omp-and-ops-3-6-in-a-nutshell/).

In the **online first** publication model (also called "forthcoming"), you publish each submission as soon as it is ready. Later, you assign these submissions to a regular, numbered issue – often with additional contents such as reviews, editorial, etc. You can [use an online first model](#publishing-submissions-in-advance-of-regular-issues-online-first-or-forthcoming) in OJS but this requires several added steps.

In the **rolling publication** model (also called "continuous publication"), you [create](issues#creating-an-issue) and "open" a new, regular issue by [publishing it](issues#publishing-an-issue) at the beginning of a publication cycle – often, the calendar year. You then add each new submission to the issue as soon it is ready. At the end of the cycle, you "close" the issue and open a new one. To close an issue, just stop adding submissions.

The key distinction between this models is these:

*   with an online first model, you "move" submissions from the online first collection to a regular, numbered issue at a certain point;
*   with a rolling publication schedule, the articles stay assigned to the same issue.

In both cases, the URLs for the submissions stay the same once published in OJS.

Online first and rolling publication both introduce two small complications for OJS:

1.  **DOIs.** Normally, OJS registers DOIs for submissions when a new issue is published. However, in both of the models, issues are published before the articles. That means you have to [manually register DOIs](#doi-registration) for submissions.
2.  **Notifications**. OJS gives you the option of notifying your journal’s regular users about the publication of a new issue. Because the submissions are published separately from the issues, you cannot notify your users about the publication of new submissions. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

## Publishing submissions in advance of regular issues: "online first" or "Forthcoming"

!!! info

    **Last updated:** November 25, 2026 for OJS 3.5.0-5.
    
    !!! warning
    
        This version differs significantly from the instructions developed for OJS 3.3.

!!! info

    At the time of writing, the 3rd party [Forthcoming plugin](https://github.com/tsv-fi/forthcoming) has been newly updated for OJS 3.5. This plugin's updates have previously lagged significantly behind OJS's development cycle, so there is a risk that an OJS upgrade breaks it. YDJ recommends it with caution. Please [contact YDJ](ydj-contact) to discuss installation of the plugin.

OJS does not have a dedicated mechanism for publishing "online first"/"forthcoming" articles but it’s possible to cheat the issue publication process to mimic the feature. The following steps explain how to publish submissions under the label "Online First" in advance of a regular, numbered issue.

Here’s what you get by following this process:

*   New submissions published as soon as they are ready
*   Stable links and DOIs (if applicable) for the submissions
*   Links to Online First through the navigation menu, the Archive, through a Highlight (optional) and through a custom sidebar block (optional)
*   Your most recent, regular issue appears as your Current Issue.

Once you have done initial setup, there are three components to this online first publication:

1. [Initial setup of Online First](#initial-setup-of-online-first)
2. [Publishing submissions to Online First](#publishing-submissions-to-online-first)
3. [Reassigning submissions to a regular issue](#reassigning-submissions-to-a-regular-issue)
4. [Reordering issues in archives](#changing-the-order-of-issues-in-your-archive)

### Initial setup of Online First

Follow these steps just once, when you commit to using an online first publication model.

You must create and publish your Online First issue, and create a Navigation Menu Item linked to that issue. You can also create a custom sidebar block linked to Online First as well.

1.  Create your Online First issue:

    1.  Follow the [steps for creating an issue](issues#creating-an-issue)
    2.  In Step 2 of Creating an Issue, use the title "Online First" and select only the **Title** checkbox.

2.  [Publish](issues#publishing-an-issue) the Online First issue.
3.  Change your Current Issue back to your most recent, regular issue:

    1.  Go to **Issues** > **Back Issues**
    2.  Click the blue arrow beside the title of your most recent, regular issue
    3.  Click **Current Issue**
    4.  Click **OK**.

4.  Create the Navigation Menu Item:

    1.  Go to **Settings** > **Website** > **Setup** > **Navigation**
    2.  Next to Navigation Menu Items, click **Add Item**
    3.  In the **Title** field, write "Online First"
    4.  Under **Navigation Menu Type**, select **Remote URL**
    5.  In the **URL** field that just appeared, paste the full URL of your Online First issue  
        **Note for multilingual journals:** the URL for issues are different in each language. Ensure that you have linked the appropriate issue in the appropriate URL field.
    6.  Click **Save**.

5.  Add the Navigation Menu Item to the Primary Navigation Menu:

    1.  Under Navigation, click **Primary Navigation Menu**
    2.  Drag Online First from the **Unassigned Menu Items** column to the **Assigned Menu Items** column
    3.  Ensure that the container box for Online First is flush against the left-hand side of the Assigned Menu Items column; if it is indented, it will be nested under the menu item above it
    4.  Click **Save**.

6.  Review and adjust DOI settings at **Settings** > **Distribution** > **DOIs**:

    1. In the **Setup** tab, **Automatic DOI Assignment** must be set to **Upon Reaching Copyediting**.
    2. In the **Registration** tab, **Enable automatic depositing** must be checked

7.  [Reset the Current Issue](issues#setting-your-current-issue) to your most recent, regular issue
8.  Optional: create a custom sidebar block:

    1.  Follow the steps for [creating a custom block](ojs-site#adding-custom-blocks-to-the-right-sidebar) with the title "Online First"
    2.  In the **Content** field, write "Online First"
    3.  Link the text in the Content field to your Online First issue
    4.  Keep the box under **Show Name** unchecked.

9.  Optional: use [Highlights](https://docs.pkp.sfu.ca/learning-ojs/journal-managers/en/appearance.html#highlights) to make Online First more prominent on the journal's homepage.

Online First is now a published issue without any submissions that appears in the navigation menu, in the Archives and, optionally, in a custom block in the right sidebar. You can now publish submissions to this issue as they are ready.

### Publishing submissions to Online First

Follow these steps every time you wish to publish a new submission to Online First.

When you have completed the editorial and production workflow for the submission, you can assign it the Online First issue to have it published immediately.

1.  Go to **Production** > **Issue** for the submission
2.  Under the Issue heading, click **Assign to Issue**
3.  Select Online First from the drop-down menu
4.  Click **Save**
5.  Click **Schedule for Publication**
6.  A notification saying "All publication requirements have been met" will appear. Click **Publish**
7.  If your journal receives DOIs, manually [register the DOI](#doi-registration)

The submission will now be published in Online First. If the submission has a DOI, the DOI will now register and soon become functional.

You cannot use OJS’s built-in notification to notify your readers about newly published submissions – it only sends notifications for new issues. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

### Reassigning submissions to a regular issue

Follow these steps when you are ready to publish a complete, regular issue.

1.  [Create a new, regular issue](issues#creating-an-issue)
2.  Create a new version for each submission:

    1.  While on one of the **Publication** tabs, click **Create a New Version**
    2.  Click the **Issue** tab for the new version
    3.  Under the Issue heading, click **Change Issue**
    4.  Select the new issue from the drop-down menu and click **Save**
    5.  Click **Publish**
    6.  A notification saying "All publication requirements have been met. This will be published when \[issue name\] is published. Are you sure you want to schedule this for publication?" Click **Schedule for Publication**

3.  [Publish the new issue](issues#publishing-an-issue)
4.  Unpublish the initial version of each submission:

    1.  While on one of the **Publication** tabs, select the initial version from the drop-down
    2.  Click **Unpublish**

5.  [Sync the DOIs](#syncing-dois-online-first-only) for the articles:

    1.  Go to the **DOIs** page. All reassigned submissions should be listed if you click the **Needs Sync** filter
    2.  Click **Deposit All**

The articles that were previously published in Online First will now appear in OJS as part of the new issue. However, the URLs and DOIs for the published submissions will remain unchanged.

### Changing the order of issues in your archive
By default, each newly published issue appears at the top of the list of issues in the Archive. This process ensures that Online First remains that the top of the list in the Archive, which will look less awkward than having it interspersed among the regular issues.

1.  Go to **Issues** > **Back Issues**
2.  Click **Order**
3.  Drag Online First to the top of the list of issues
4.  Click **Done**.

## Continuous publication in a regular issue: "rolling publication"

!!! info

    **Last updated:** November 21, 2026 for OJS 3.5.0-5.
    
    !!! warning
    
        This version differs significantly from the instructions developed for OJS 3.3.

OJS allows you to assign a submission to an issue that has already been published. Doing so immediately publishes the submission. Therefore, implementing a rolling publication model is simple in OJS.

To implement a rolling publication model:

1.  Determine your publication cycle (e.g., annual)
2.  If applicable, review and adjust DOI settings at **Settings** > **Distribution** > **DOIs**:
    
    1.  In the **Setup** tab, **Automatic DOI Assignment** must be set to **Upon Reaching Copyediting**.
    2.  In the **Registration** tab, **Enable automatic depositing** must be checked

3.  At the beginning of the publication cycle, [create a new issue](issues#creating-an-issue)
4.  [Publish the issue](issues#publishing-an-issue)
5.  When you have completed the editorial and production workflow for a submission, publish it be assigning it to the current issue in **Publication** > **Issue**. The submission will now appear be live on the OJS site

    1.  If applicable, see [the section on DOIs](#dois-in-online-first-and-rolling-publication), below

6.  Repeat step 4 until the end of the publication cycle.
7.  At the end of the publication cycle, return to step 2

If you use the rolling publication model, you cannot use OJS’s built-in notification to notify your readers about newly published submissions – it only sends notifications for new issues. You may wish to use the Announcements plugin or Highlights feature in order to send notifications about newly published submissions.

You may wish to delay publication of the new issue until you have a submission ready to publish in the new publication cycle. This will prevent OJS from displaying an empty table of contents on your journal’s homepage.

## DOIs in online first and rolling publication
    
If you have DOIs for online first or rolling publication models, you must first have the following settings configured:

-   **Settings** > **Distribution** > **DOIs** > **Setup**: **Automatic DOI Assignment** must be set to "Upon Reaching Copyediting"
-   **Settings** > **Distribution** > **DOIs** > **Registration**: **Enable automatic depositing** must be checked.

In testing, we have found that automatic DOI assignment and registration sometimes does not take place as it should. Therefore, you should verify whether these process have taken place and, if required, perform them manually.

### DOI assignment

Once an article has reached the Copyediting stage (i.e, at has been Accepted or been submitted via QuickSubmit), it _should_ be assigned a DOI automatically. Check the **DOIs** page to see the DOI for that submission. If a DOI has not been automatically assigned, you can assign it manually:

1.  In the list of DOIs on the **DOIs** page, check the box next to the submission title
2.  Click **Bulk Actions**
3.  In the Bulk Actions drop-down, click **Assign DOIs**

### DOI registration

The DOI _should_ also register automatically upon publication. Click the published article's DOI 5-10 minutes after publication to ensure that it has registerd. If it has not, you can register it manually:

1.  Go to the **DOIs** page
2.  Click **Deposit All**

### Syncing DOIs (online first only)

After you reassign an article from Online First to a regular issue, you must sync the DOIs to send the updated citation information to Crossref. If you do not do this, the DOI will still resolve to the article but indexes and citation tools that draw from Crossref continue to propagate outdated information about the articles.

To sync DOIs:

1.  Go to the **DOIs** page. All reassigned submissions should be listed if you click the **Needs Sync** filter
2.  Click **Deposit All**

## Bypassing the editorial workflow in OJS

!!! info

    **Last updated:** November 21, 2026 for OJS 3.5.0-5

It is possible to bypass the editorial workflow (submission, review, copyediting, or layout production) in OJS by using the [QuickSubmit plugin](submissions#using-the-quicksubmit-plugin). QuickSubmit may be useful when uploading unique article types that do not need to go through the review and production process in OJS (e.g., editorial content that does not go through peer review).

Some journal entirely bypass the editorial workflow in OJS and only use the platform to host completed articles. In this case, all journal contents should go through QuickSubmit.

Here is an overview of the issue publication process for journals bypassing the editorial workflow:

1.  [Create a new issue](issues#creating-an-issue): before uploading the journal contents, you want to create the future issue in which they will be published. This is because the QuickSubmit plugin (step 2) allows you to assign the contents directly to an issue.
2.  [Upload the contents using QuickSubmit](submissions#using-the-quicksubmit-plugin): use the QuickSubmit plugin to upload each new submission (article, editorial, review, etc.) to OJS. Do _not_ use this to upload a single, full-issue galley.

    1.  In step 7, you will want to select **Published** in order to assign the content to the new, unpublished issue you created previously.

3.  [Assign the DOIs to the articles](dois#dois-and-quicksubmit): do this after you have uploaded all the contents.
4.  [Upload the full-issue galley (optional)](issues#adding-a-full-issue-pdf-galley): if you have a single galley file containing all the issue contents, upload it here.
5.  [Publish the issue](issues#publishing-an-issue): once you have added all contents to the new issue, you can publish the issue.

## Publishing audio or video journal content

!!! info

    **Last updated:** November 21, 2026 for OJS 3.5.0-5

YDJ allows you to publish audio or video media content in a journal issue by embedding it in an HTML galley.

There are three parts to this:

*   Submission and review
*   Hosting the media files, and
*   Embedding the stream in a galley.

### Submission and review

OJS is not well-equipped to accept large media files as submissions files. Therefore, if your journal accepts multimedia submissions, YDJ recommends creators share their media files with the editors outside of OJS.

### Hosting the media files

Media files may be hosted locally through [York University Digital Library (YUDL)](https://digital.library.yorku.ca/) or externally via third-party service. If possible, YDJ prefers to host a copy of the media file in YUDL. This ensures that the media will be preserved in accordance with the YUL’s [Digital Preservation Policy](https://www.library.yorku.ca/web/about-us/library-policies/digital-preservation-policy/) and that the link will remain stable.

Content creators/owners must agree to the York University Digital Library Distribution Licence (available upon request) to have their material preserved in YUDL. If they do not agree to the terms, the media files must be hosted elsewhere.

#### Hosting through York University Digital Library

If hosting with YUDL, the editor must return the YUDL Distribution Licence and the following information to YDJ:

*   Copyright holder
*   Rights statement, such as a [Creative Commons license](https://creativecommons.org/share-your-work/cclicenses/), [RightsStatement.org statement](https://rightsstatements.org/en/), or [Traditional Knowledge label](https://localcontexts.org/labels/traditional-knowledge-labels/)

The Digital Publishing Librarian will direct you on the best method for sharing the media file.

#### External hosting

It is also possible to link to an external host (such as YouTube, Vimeo, or Soundcloud). Externally hosted media is subject to the provider’s terms of use. External hosts may not provide media files with a stable URL or preserve them indefinitely; therefore, it is possible that the media stream in OJS breaks. It is the journal’s responsibility to monitor the media stream and to have the galley updated, if required.

### Embedding the stream in a galley

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