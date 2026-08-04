# Submissions

!!! info

    **Last updated:** September 29, 2021

The submission is the other key element in OJS. As a noun, "submission" is a generic term that includes articles, book reviews, and art. A submission has its own page, one or more galleys, and metadata. It will appear in the table of contents for an issue when assigned to a published issue.

## Using the QuickSubmit Plugin

!!! info

    **Last updated:** July 28, 2025 for OJS 3.3.0.19 and OJS 3.4.0.7

QuickSubmit is a tool for uploading submissions that bypasses all stages of the workflow. Use it to upload content that does not required review (such as editorials) or if you conduct your review and editorial workflow outside of OJS.

**Important note:** do _not_ use this process to upload a single galley file of your full issue. Instead, see the instructions for [Adding a full-issue PDF galley](issues#adding-a-full-issue-pdf-galley).

Contents:

*   [Published or Unpublished: which option to use for your publication model](#published-or-unpublished-which-option-to-use-for-your-publication-model)
*   [Finding the QuickSubmit plugin](#finding-the-quicksubmit-plugin)
*   [Uploading submissions with the QuickSubmit plugin](#uploading-submissions-with-the-quicksubmit-plugin)
*   [Finding and editing submissions after completing QuickSubmit](#finding-and-editing-submissions-after-completing-quicksubmit)

### Published or Unpublished: which option to use for your publication model

All publication in OJS happens at the _issue_ level, so using QuickSubmit alone does not necessarily publish the submission. There are three ways to publish the submission, depending on your publication model:

1.  In Step 7 below, select **Published** and then, in Step 8, assign the submission to a Back Issue or the Current Issue that has already been published: when you complete the process, the submission will immediately appear online as part of that issue.
2.  In Step 7 below, select **Published** and then, in Step 8, assign the submission to a Future Issue that has not yet been published: when you complete the process, the submission will appear online when you [publish the issue](issue#publishing-an-issue).
3.  In Step 7 below, leave the selection as **Unpublished**: you can then [find the submission at a later date](#finding-and-editing-submissions-after-completing-quicksubmit) and edit the details later to assign it to an issue.

### Finding the QuickSubmit plugin

Once logged in, click **Tools** in the left-hand sidebar. This brings you to the Import/Expert tab of the Tools page. You should see **QuickSubmit Plugin** in the list of tools – if you do not, contact [contact YDJ](ydj-contact.md) to have the plugin upgraded.

### Uploading submissions with the QuickSubmit plugin

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

### Finding and editing submissions after completing QuickSubmit

If you need to edit a submission after creating and saving it in QuickSubmit, you can find it in one of your submissions queues. Access your submission queues by clicking **Submissions** at the top of the left-hand navigation menu.

*   If you _did not_ assign an issue in step 7, the submission will appear in **All Active**. If you are retrieved the submission with the same account that uploaded it, it will also appear in **My Active**.
*   If you _did_ assign and an issue in step 7, the submission will appear in the **Archives** queue with the Scheduled status.

Once you find the submission in the proper queue, you can edit it. To edit the submissions:

1.  Click **View** to the right of the submission entry in the queue
2.  Click the **Publication** tab to edit the submission metadata, [upload or change the galley file](#adding-and-replacing-galleys), [change the section](#changing-the-section-of-a-submission), or assign it to an issue
3.  Click **Save** at the bottom of the screen after making any changes.

At the time of the latest update to this page, dates entered in QuickSubmit do not save when the submission was published: regardless of the date entered in step 8, it will be changed to the date the issue is published when you publish it. If you need to backdate submissions, please [contact YDJ](ydj-contact.md).

## Adding and replacing galleys

!!! info

    **Last updated**: September 29 for OJS 3.3.0.8

The galley is the final form of the article – editing, copy edited, and laid out – that is posted to the OJS site for reading. Galleys are usually uploaded as PDFs.

### Adding a galley

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

### Replacing a galley

If the submission has already been published, you will need to [create a new version](#editing-a-submission-after-publication) in order to replace the galley. Replacing the galley constitutes a major change and requires a new version instead of unpublishing and republishing the submission.

1.  Open the submission and navigate to the **Publication** tab, then to the **Galleys** facet.
2.  Click the blue arrow next to the galley label and click **Change File**.
3.  In the first drop-down, select the file you wish to replace.
4.  Drag and drop the galley file from your desktop to upload area OR click **Upload File** and select the galley file from your file directory.
5.  Click **Continue.**
6.  Rename the file if you wish, the click **Continue**.
7.  Click **Complete**.

## Changing the section of a submission

!!! info

    **Last updated:** July 26, 2021 for OJS 3.3

To change the section to which a submission is assigned:

1.  Open the **Production** tab for the submission
2.  Open the **Issue** tab
3.  Use the drop-down menu under **Section** to change the Section.

## Editing a submission after publication

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

### Fixing the error: "the submission must be in the Copyediting or Production stages…"

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

## Cleaning up unwanted submissions in the editorial queues

!!! info

    **Last updated:** July 16, 2026 for OJS 3.5
	
You may end up with several kinds of unwanted submissions:  
- incomplete submissions abandoned by the authors,  
- duplicate submissions created in error,  
- submissions created for purposes of testing, training, or troubleshooting

The method of cleaning these up depends on whether the submissions are [complete](#declining-completed-submissions) (have gone through the entire Submission Wizard and are awaiting editorial review) or are [incomplete](#deleting-incomplete-submissions).

### Declining completed submissions

If a submission is complete, you must decline it. You must do this individually.

This is the case for submissions at any stage of the Workflow, inlcuding those that have completed Production (this will be the case for submissions made through QuickSubmit). The process will vary slightly, depending which Workflow stage it has reach and if it has been scheduled for publication.

In summary, you must revert any editorial decisions until you reach either the Submission or Review stage of the workflow, and then decline the submission as an editorial decision.

To decline a completed submission:

1.  Find the submission in your editorial queue and click **View**  
2.  If the submission information opened to *Publication: Title & Abstract* (or any other tab whose title starts with *Publication*), click the **Production** tab in the left-hand menu  

    a.  if it did not, skip to step 3  
   
3.  If you are now at *Workflow: Production*, click **Back to Copyediting**  

    a.  if you are not, or if the *Back to Copyediting* button does not appear, skip to step 5  
   
4.  On the resulting page, click **Record Decision** and then click past the confirmation  
5.  If you are now at *Workflow: Copyediting*, click **Cancel Copyediting**  

    a.  if you are not, or if the *Cancel Copyediting* button does not appear, skip to step 7  
   
6.  On the resulting page, click **Record Decision** and then click past the confirmation  
7.  If you are at *Workflow: Submission* or *Workflow: Review*, click **Decline Submission**  
8.  On the resulting page, click **Record Decision**  
9.  If prompted, you may opt to send the email notification to the author or skip it.  

Upon completing this process, the submission will move to the *Declined* queue.

### Deleting incomplete submissions

If a submission is incomplete, you may delete it outright. This is process can be done in bulk to multiple submissions simultaneously.

To delete incomplete submissions:  

1.  Go to the *All in Submission Stage* queue  
2.  Click the icon with three dots next to the *Filters* button  
3.  The **Delete Incomplete Submissions** button will appear. Click it  
4.  Follow any resulting prompts as appropriate.  

Deleted incomplete submissions will be purged from the system.

## Adding data sets to articles

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

## Adding DOIs to submission galleys before publication

!!! info

    **Last updated:** November 19 for OJS 3.3

If your journal has been configured for DOIs, you can easily determine what the DOI will be before you publish it. This way, you can add the DOI to the galley even though it is not possible to view the DOI before publication.

See the chapter on the [structure of DOIs](dois#determining-the-structure-of-your-dois) to determine what a submission's DOI will be and to transform the DOI into a URL. Once you have determined the DOI and transformed it into a URL, you can add the DOI to the galley as a link that will go live once the submission is published.

## Understanding and using Categories

!!! info

    **Last updated**: May 2, 2025 for OJS 3.3 and 3.4

The Category feature is best used as a browsing tool for readers that is distinct from Issues and Sections. It should be used in conjunction with the Browse Block or with navigation menu items.

When you create a Category, you do two things:

1.  You create a page for that Category, which includes a list of all articles assigned to it, as well as an optional description and cover image. (Example: [Category browse page](https://jat.journals.yorku.ca/index.php/default/catalog/category/parent1))
2.  You add a field to the submission’s metadata page, which links to the Category page. (Example: [submission metadata page](https://jat.journals.yorku.ca/index.php/default/article/view/97))

You can also nest Categories one level using Parent Category. Both the Parent Category and the nested Category will receive their own pages. The Parent Category page will link both to the submissions assigned to it and to the pages for the nested Categories.

Unlike sections, Categories do not appear in an issue’s table of contents and cannot be used to direct submissions to a particular editor. However, Categories can be used to make related content from across multiple issues in the same place. If you wish to make your journal content browsable by section, please request that the Digital Publishing Librarian install the Browse By Section Plugin.

### Creating Categories

Create and edit Categories at **Journal Settings > Categories**.

### Assigning submissions to Categories

If your journal has created any Categories, they will appear in the submission process for authors as well as in the QuickSubmit form. You can also edit the Category assignment in a submission’s **Publication > Issue** tab.

### Making Categories discoverable

Categories should be used in conjunction with the Browse Block, which can be activated at **Website Settings > Appearance > Setup > Sidebar**. This sidebar block will automatically update as Categories are added, removed, or nested.

You may also also wish to manually create [Navigation Menu Items](ojs-site#navigation-menus) for your Categories. However, these will not automatically update as Categories are added, removed, or nested.
