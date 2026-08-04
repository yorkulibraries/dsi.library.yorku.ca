# Alternative publication models

!!! info

    **Last updated:** November 18, 2021 for OJS 3.3.0.8

There are two common alternatives to the regular, full issue publication model: online first, and rolling.

In the **online first** publication model (also called "forthcoming"), you publish each submission as soon as it is ready. Later, you assign these submissions to a regular, numbered issue – often with additional contents such as reviews, editorial, etc. You can [use an online first model](#publishing-submissions-in-advance-of-regular-issues-online-first-or-forthcoming) in OJS but this requires several added steps.

In the **rolling publication** model (also called "continuous publication"), you [create](issues#creating-an-issue) and "open" a new, regular issue by [publishing it](issues#publishing-an-issue) at the beginning of a publication cycle – often, the calendar year. You then add each new submission to the issue as soon it is ready. At the end of the cycle, you "close" the issue and open a new one. To close an issue, just stop adding submissions.

The key distinction between this models is these:

*   with an online first model, you "move" submissions from the online first collection to a regular, numbered issue at a certain point;
*   with a rolling publication schedule, the articles stay assigned to the same issue.

In both cases, the URLs for the submissions stay the same once published in OJS.

Online first and rolling publication both introduce two small complications for OJS:

1.  **DOIs.** Normally, OJS assigns and registers DOIs for submissions when a new issue is published. However, in both of the models, issues are published before the articles. That means you have to [manually assign and register DOIs](#adding-dois-for-online-first-or-rolling-publication-models) for submissions.
2.  **Notifications**. OJS gives you the option of notifying your journal’s regular users about the publication of a new issue. Because the submissions are published separately from the issues, you cannot notify your users about the publication of new submissions. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

## Publishing submissions in advance of regular issues: "online first" or "Forthcoming"

!!! info

    **Last updated:** February 21, 2025 for OJS 3.3 and 3.4

   **Important update:** the [Forthcoming plugin](https://github.com/ajnyga/forthcoming) has been updated for OJS 3.3 and 3.4 and is a much simpler solution than the instructions provided below. These instructions are retained for reference.

   Please [contact YDJ](ydj-contact.md) to have the plugin installed and configured.

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
    1.  Follow the steps for [creating a custom block](ojs-site#adding-custom-blocks-to-the-right-sidebar) with the title "Online First"
    2.  In the **Content** field, write "Online First"
    3.  Link the text in the Content field to your Online First issue
    4.  Keep the box under **Show Name** unchecked.

Online First is now a published issue without any submissions that appears in the navigation menu, in the Archives and, optionally, in a custom block in the right sidebar. You can now publish submissions to this issue as they are ready.

### Publishing submissions to Online First

Follow these steps every time you wish to publish a new submission to Online First.

When you have completed the editorial and production workflow for the submission, you can assign it the Online First issue to have it published immediately.

1.  If your journal’s submissions receive DOIs, manually [assign the DOI](dois#creating-dois) to the submission
2.  Go to **Production** > **Issue** for the submission
3.  Under the Issue heading, click **Assign to Issue**
4.  Select Online First from the drop-down menu
5.  Click **Save**
6.  A notification saying "All publication requirements have been met" will appear. Click **Publish.**
7.  If your journal’s submissions receive DOIs, manually [register the DOI](dois#register-the-doi-with-crossref).

The submission will now be published in Online First. If the submission has a DOI, the DOI will now be registered and functional.

You cannot use OJS’s built-in notification to notify your readers about newly published submissions – it only sends notifications for new issues. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

### Reassigning submissions to a regular issue

Follow these steps when you are ready to publish a complete, regular issue.

You must reassign the articles from Online First to the new issue, publish the new issue, and then reorder your list of issues.

1.  [Create a new, regular issue.](issues#creating-an-issue)
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
4.  [Publish the new issue](issues#publishing-an-issue).
5.  Reorder your list of issues:
    1.  Go to **Issues** > **Back Issues**
    2.  Click **Order**
    3.  Drag Online First to the top of the list of issues
    4.  Click **Done**.

The submissions that were previously published in Online First will now appear in OJS as part of the new issue. However, the URLs and DOIs for the published submissions will remain unchanged.

You cannot show the contents of both your Online First issue and your most recent, regular issue on your journal’s homepage. OJS only displays the contents of the Current Issue on your journal’s homepage, and only one issue can be designated at the Current Issue. You must therefore designate either Online First or your most recent, regular issue as your Current Issue; YDJ advises designated the regular issue as the Current Issue. While it may be _technically_ possible to display more than one table of contents but YDJ does not have the resources to customize OJS like this or to support the customization.

If you skip this step, the empty Online First issue will appear on your OJS homepage. This may create the impression that your journal is inactive or that there is a problem with the website.

By default, each newly published issue appears at the top of the list of issues in the Archive. This step ensures that Online First remains that the top of the list in the Archive.

## Continuous publication in a regular issue: "rolling publication"

!!! info

    **Last updated:** November 18, 2021 for OJS 3.3.0.8

OJS allows you to assign a submission to an issue that has already been published. Doing so immediately publishes the submission. Therefore, implementing a rolling publication model is simple in OJS.

To implement a rolling publication model:

1.  Determine your publication cycle (e.g., annual).
2.  At the beginning of the publication cycle, [create a new issue](issues#creating-an-issue).
3.  [Publish the issue](issues#publishing-an-issue).
4.  When you have completed the editorial and production workflow for a submission, publish it be assigning it to the current issue in **Publication** > **Issue**. The submission will now appear be live on the OJS site.
5.  Repeat step 4 until the end of the publication cycle.
6.  At the end of the publication cycle, return to step 2.

If your journal provides submissions with DOIs, you must [manually assign and register the DOI](#adding-dois-for-online-first-or-rolling-publication-models) for each new submissions you publish.

If you use the rolling publication model, you cannot use OJS’s built-in notification to notify your readers about newly published submissions – it only sends notifications for new issues. You may wish to use the Announcements plugin in order to send notifications about newly published submissions.

You may wish to delay publication of the new issue until you have a submission ready to publish in the new publication cycle. This will prevent OJS from displaying an empty table of contents on your journal’s homepage.

Unless you have assigned a submission when you first publish the issue (see footnote 1). In this case, OJS will automatically assign and register the DOI.

### Adding DOIs for online first or rolling publication models

!!! info

    **Last updated:** November 12, 2021 for OJS 3.3.0.8

If you publish a submission after the publication of the issue – for example, if you have a rolling publication schedule – the DOIs will not be automatically assigned and registered. You must perform two small tasks to do this manually.

#### Assign the DOI prior to publishing the submission

1.  Open the submission’s **Publication** tab
2.  Go to the **Identifiers** facet
3.  Click **Assign**, next to the DOI field
4.  Click **Save**.

**Note:** if you forget to assign the DOI prior to publication, you can perform these steps by [editing the submission after publication](submissions#editing-a-submission-after-publication).

#### Register the DOI with Crossref

1.  In the back end of OJS, click **Tools** in the left-hand menu
2.  Open the **Crossref XML** Export Plugin in the list of Tools
3.  Click the **Articles** tab. Your newly published submission should appear at the top of the list with the status Not Deposited
4.  Click the checkbox for the submission
5.  Scroll to the bottom of the page and click **Deposit**
6.  Wait for the page to reload. If registration is successful, you have completed the process. If you get an error message, please notify the Digital Publishing Librarian.

**Note:** this must be performed by a user with the Journal Editor or Journal Manager role

## Bypassing the editorial workflow in OJS

!!! info

    **Last updated:** July 28, 2025 for OJS 3.3 and 3.4

This page is intended for journal editors who perform the editorial workflow (submission, review, copyediting, or layout production) outside OJS and only wish to use OJS to host the finished materials.

The individual steps of this process are covered elsewhere in this guide but linked here:

1.  [Create a new issue](issues#creating-an-issue): before uploading the journal contents, you want to create the future issue in which they will be published. This is because the QuickSubmit plugin (step 2) allows you to assign the contents directly to an issue.
2.  [Upload the contents using QuickSubmit](submissions#using-the-quicksubmit-plugin): use the QuickSubmit plugin to upload each new submission (article, editorial, review, etc.) to OJS. Do _not_ use this to upload a single, full-issue galley.
    1.  In step 7, you will want to select **Published** in order to assign the content to the new, unpublished issue you created previously.
3.  [Assign the DOIs to the articles](dois#dois-and-quicksubmit): do this after you have uploaded all the contents.
4.  [Upload the full-issue galley (optional)](issues#adding-a-full-issue-pdf-galley): if you have a single galley file containing all the issue contents, upload it here.
5.  [Publish the issue](issues#publishing-an-issue): once you have added all contents to the new issue, you can publish the issue.

## Publishing audio or video journal content

!!! info

    **Last updated:** March 31, 2026 for OJS 3.3.0-22

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
