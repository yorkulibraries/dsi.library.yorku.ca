# Configuring and reviewing journal setup 

!!! info

    **Last updated:** August 24, 2026

## Before starting 

This section walks you through the journal settings page-by-page and tab-by-tab. The most important journal-level settings are configured through the links under _Settings_ in the left sidebar in the dashboard: _Journal_, _Website_, _Workflow_, _Distribution_, _Users & Roles_.  

Whether your journal is already established with YDJ or you are new to the program, you should review the settings and ensure that they reflect your journal’s identity, practices, and policies as fully and as transparently as possible. YDJ recommends that you follow every item in this section in order, following up on items later if required. 

Any fields not listed here may be considered optional. ==Items deemed by YDJ to be particularly important are highlighted in yellow==. Please [contact YDJ](ydj-contact.md) if you require a more accessible form of highlighting.

!!! tip "Making changes in OJS"

    !!! tip "Tip &num;1"

        There’s a Save button at the bottom of virtually every page in the settings. Make sure you use it!  

    !!! tip "Tip &num;2"

        When you see a blue arrow to the left of an article, issue, checklist item, plugin, or other interface item, that’s where you click to expose menu options such as Edit, Settings, Delete, or other. 

Finally, a suggestion: the [DOAJ application form](https://doaj.org/account/login?redirected=apply) can be taken as guidelines for transparency. Once you’ve taken a pass at setting up your journal, you might want to have a look at the form to see if there’s anything you could add. Some of the questions are technical and might not make sense but focus on the ones that ask for transparency around editorial membership and process. Once eligible, you should consider [applying for inclusion in DOAJ](getting-started-with-indexing#directory-of-open-access-journals-doaj).

## 1. Journal settings  

### 1.1 Masthead  

* ==_Journal title_==: it’s the single most important piece of info on the website and gets used EVERYWHERE.  
* ==_Journal initials_==: these are particularly visible when OJS sends email
* ==_Country_==: required  
* ==_Publisher_==: optional whether you identify your academic unit or York University Library  
* ==_URL_==: the publisher URL (not the journal URL)  
* ==_Online ISSN_== and _Print ISSN_: if you don’t have one yet, you can apply for one after your first issue. If you have both online and print ISSNs, enter both. If you have had multiple ISSNs, enter the most recent; you may wish to include previous ISSNs in _About the Journal_ (below) 
* ==_Editorial History_==: important for transparency’s sake. List editorial positions and board members.

!!! info

    YDJ has a [custom implementation](what-to-expect-in-ojs-35#alternative-implementation-to-editorial-masthead-for-ydj) for an Editorial Team page as an alternative to the default Editorial Masthead page in OJS 3.5, which draws on data entered in the _Editorial History_ field. Editors experienced with prior versions of OJS 3 will find that this looks and behaves like the pre-existing Editorial Team page.

* ==_Journal Summary_==: less important than _About the Journal_ (below). Can be made to appear on the homepage ([see OJS homepage layout (Default template), #8](ojs-site#ojs-homepage-layout-default-theme)) – but keep it short!  
* ==_About the Journal_==: appears on the _About the Journal_ page on the front end. YDJ advises including more information about the journal’s scope, mandate, history, and operations than not – this is also important for transparency’s sake. You may also wish to indicate the date of last update at the bottom of the blurb.  

### 1.2 Contact  

* ==_Name_ and _Email (Principal Contact)_==: very important. These appear on the front end.
* _Name_ and _Email (Technical Support Contact)_: since most technical questions must be resolved by the platform host, we advise using YDJ as a technical contact, with the name “York Digital Journals (YDJ)” and address "diginit@yorku.ca." 

### 1.3 Sections  

Everything published in OJS belongs to a section. Issue contents are organized by section. Some parameters controlled at the section level are:  

* Whether the contents are peer reviewed (very important for indexing)  
* Whether the contents require abstracts  
* Section-specific policies, that will be publicly displayed in the submission guidelines.  

**If your journal is new to YDJ**, ==you may not need to set these up right away but they’re very important and you should know how they work==. 

**If your journal has already been established with YDJ**, ==you should review each section to see if a Section Editor is assigned==. When a Section Editor is designated, new submissions for that section will be assigned directly to that User, and the Journal Editors will not be notified about the new submission.  

See _Learning OJS 3.3_ for more about [sections](https://docs.pkp.sfu.ca/learning-ojs/3.3/en/journal-setup#sections) (although this refers to an older version of OJS, this content is still pertinent to OJS 3.5).  

### 1.4 Categories  

These may not be immediately useful. Learn more at [Understanding and using Categories](submissions#understanding-and-using-categories).  

## 2. Website Settings

### 2.1 Appearance  

#### 2.1.1 Theme  
  
* _Colour_: if you change the colour of the header, you may need to refresh the browser cache to get it to display on the front page.  
* _Journal Summary_: the checkbox toggles whether the journal summary from the Masthead (see [1.1](#11-masthead), above) appears on the home page. I would recommend doing this.  

#### 2.1.2 Setup  

* ==_Logo_ and _Homepage Image_==: the logo will be dynamically sized with the site. If you have a large or highly detailed logo, I’d recommend using the Homepage Image instead. You can use both, however.  See ([see OJS homepage layout (Default template), #3 and #6](ojs-site#ojs-homepage-layout-default-theme)) to learn more. ==Be sure to use alternative text to describe the images, for accessibility purposes==.
* _Page footer_: this can be a great place to include persistent information across the whole journal site. You might want to repeat journal title, publisher info, and ISSN as well as sponsors, mottos, or land acknowledgments.  
* _Sidebar_: toggles which block appear in the right sidebar. Language Toggle Block is an important one if your journal is multilingual (if so, it should activate automatically). This is also where you toggle Custom Blocks (see [Sidebar blocks](ojs-site#sidebar-blocks)).  

#### 2.1.3 Editorial Masthead

Disregard. See _Editorial History_ ([1.1](#11-masthead), above) for YDJ's alternative implementation.

#### 2.1.4 Advanced  

See [Understanding the OJS homepage layout (Default Theme)](ojs-site#understanding-the-ojs-homepage-layout-default-theme) and [Managing your site's appearance](ojs-site#managing-your-sites-appearance) from _OJS for YDJ_ and PKP's [Designing your journal](https://docs.pkp.sfu.ca/designing-your-journal/en/) to learn more about the options for styling your journal. 

### 2.2 Setup  

#### 2.2.1 Information  

These fields populate the Information Block under Sidebar (see [2.1.2](#212-setup), above). The pre-populated information here is so generic as to be useless. YDJ advises only using these fields if you’re going to populate them with meaningful, journal-specific info; otherwise, you can deactivate them in the Sidebar settings (_Website settings_ > _Appearance_ > _Setup_ > _Sidebar_). 

#### 2.2.2 Languages  

Website languages appear here once activated by YDJ. [Contact YDJ](ydj-contact.md) if you need more languages activated. You can add or remove submission languages yourself on this page. 

* _Website languages_

    * _UI_: governs the languages in which the user interface (UI) of the OJS front end site and dashboard may appear. Activates the _Language Toggle Block_ (see [2.1.2](#212-setup), above).
    * _Forms_: governs the languages in which you can enter information in the OJS settings fields (i.e, the material covered in this document).

* _Submission languages_

    * _Submissions_: governs the languages which authors can designate for their manuscripts.
    * _Metadata_: governs the langauges in which submission metadata (e.g. title, abstract)  may be entered.
    
!!! info

    Toggling the UI language will change the language in which structural elements of the website are rendered (e.g., page titles and navigational elements). It does _not_ translate your journal's website content for you.
     

#### 2.2.3 Navigation  

Very important for site interaction, but you may not need to make any changes here. See [Navigation menus](ojs-site#navigation-menus) for information.  

#### 2.2.4 Announcements  

==Very handy for most active journals==. YDJ advises using announcements for calls for proposals and for information about editorial board changes, among others. Toggling this will add a new item called _Announcements_ to the left sidebar of the dashboard (you may need to refresh the page), where you can create and post announcements. 

#### 2.2.5 Highlights

A [new feature](https://docs.pkp.sfu.ca/learning-ojs/about-ojs/en/#highlights) in OJS 3.5 that allows you to highlight content on your journal homepage.

### 2.3 Plugins  

You can enable/disable some plugins and change settings for some in _Installed Plugins_ but, as a rule, you shouldn’t unless you really know what you’re doing. [Contact YDJ](ydj-contact.md) for help with these. 

The _Plugin Gallery_ will show you what’s available to install or to upgrade, but only the Digital Publishing Librarian as admin can perform these actions. YDJ monitors plugin upgrades for all journals. 

### 2.4 Static Pages

**If your journal is new to YDJ**, this tab should not appear.

**If your journal has already been established with YDJ**, YDJ had implemented the Static Pages plugin for several, older journals. However, we now advise using Navigation menus (see [2.2.3](#223-navigation), above) to create new pages as required.

## 3. Workflow Settings  

### 3.1 Submission  

#### 3.1.1 Disable Submissions  

You may want to toggle this if you want to prevent users from making submissions if you’re ready to accept them.  

!!! warning

   Toggling _Disable Submissions_ will add text to the Submissions page that says, "This journal is not accepting submissions at this time." If your journal has disabled submissions in OJS because you prefer to use an alternative submission pipeline, this may convey the wrong message. [Contact YDJ](ydj-contact.md) to discuss alternatives. 

#### 3.1.2 Author Guidance

* ==_Author Guidelines_==: very important. This feild appears both on the Submissions page of the front end and on the first page of the submissions workflow. Include all generic guidelines for submissions to all sections here; use the Section Policies (see [1.3](#13-sections), above) for section-specific guidelines.
* ==_Submission Checklist_: this list appears both on the Submissions page on the front end and on the first page of the submission process.
* ==_Copyright Notice_==: EXTREMELY IMPORTANT. This is the basis of your agreement with the authors. See the documentation and help links at the beginning of the document for information about copyright and licensing. This appears during the submission, and it’s where the author agrees to the terms of copyright (e.g., they retain copyright and grant you permission to publish and archive under CC license). It should be related to but distinct from the License terms (see [4.1](#41-license), below)  

#### 3.1.3 Metadata  

Enables you to enable or disable metadata fields for submissions. Once a field is enabled, you will have 3 options:  

* "Do not request coverage metadata from the author during submission": makes the field invisible during the submission process, and editors will add metadata to this field in the dashboard. 
* "Ask the author to suggest coverage metadata during submission": makes the field optional for authors, and editors can add or edit the metadata afterward.  
* "Require the author to suggest coverage metadata before accepting their submission": makes the field required for authors, and editors can add or edit the metadata afterward.  

YDJ will enable _Reference_ metadata so that authors can add their bibliographies (see [Publish reference lists for new content](services-for-journals#publish-reference-lists-for-new-content-journals-receiving-dois-only)). References are optional because some works (especially creative or multimedia) will not have references. However, for scholarly works that cite others, please ensure that the authors are directed to paste their bibliographies here.  

#### 3.1.4 Components  

The pre-populated article components may be overkill for most YDJ journals; however, the submission process directs authors to mark submissions as _Article Text_ by default. Therefore, you can probably ignore this.  

### 3.2 Review  

#### 3.2.1 Setup  

Review and change these settings as required.  

#### 3.2.2 Reviewer Guidance  

**If your journal uses the peer review functionality in OJS**, use the ==Review Guidelines== to tell your peer reviewers how you’d like them to evaluate and can outline pragmata they should be aware of. If you don’t already have reviewer guidelines, you can review and adapt guidelines from other journals.  

You may also include guidelines for your reviewers to identify and disclose competing interests.

#### 3.2.3 Review Forms  

**If your journal uses the peer review functionality in OJS**, use ==Review Forms== to create fillable forms that will be available for reviewers to complete. They work like standard web forms.  

### 3.3 Publisher Library  

Use this to store files that you want to make accessible internally or externally. For example, if you want to host PDF poster of a call for submissions, you could store it here for linking from your announcement. You may also host internal policy and procedure documents for your fellow journal editors. 

**If your journal is new to YDJ**, YDJ will store a copy of your signed hosting agreement here.

### 3.4 Emails  

* _Signature_

    * **If your journal is new to YDJ**, ==create an email signature for the journal’s outgoing email==. 
    * **If your journal has already been established with YDJ**, ==review the email signature and, if necessary, edit==. 

Review and change other settings as required. 

!!! warning

    Please consult with YDJ before changing the email templates. It is possible to remove necessary information from the templates or to delete required templates, which would have significant and detrimental impacts on your journal's operations.

## 4. Distribution Settings 

### 4.1 License  

==All fields are very important==.

_License_ terms should be similar to the _Copyright Notice_ (see [3.1.2](#312-author-guidance), above) but directed toward readers and, say, librarians who want to archive the work and instructors who may want to post copies of the article to a course site.  

### 4.2 DOIs

Do not touch. YDJ manages these settings.

### 4.3 Payments  

Do not touch, unless you seriously change the way your journal operates.  

### 4.4 Access  

Do not touch, unless you seriously change the way your journal operates.  

### 4.5 Archiving  

YDJ recommends using Scholars Portal Journals for [long-term preservation and access](services-for-journals#enable-long-term-preservation-and-access), which does not rely on these settings. 

Your journal is welcome to make independent arrangements for you journal to use the services configured on this page. [Contact YDJ](ydj-contact.md) complying with the requirements of these

## 5. Users & Roles  

### 5.1 Users 

**If your journal is new to YDJ**, ==use this section to add your co-editors and other journal staff who need access==. 

**If your journal has already been established with YDJ**, ==review the Users with Journal Editor and Journal Manager roles==. Remove those roles from the people who shouldn't have them. Accounts with these roles can make unauthorized changes to your site and published content.  

To review user accounts according to their role, use the search box next to _Current Users_. Search for "Journal manager" and "Editor" (there are several types of editor role that will be returned by this search) to review the relevant user accounts.

To remove a role from a user account:

1. Click three dots to the right of the user's name to expose available options for that account.
2. Click _Edit_. This will open user information page.
3. Click _Remove Role_ next to the role you wish to remove.
4. Confirm the removal.

A user account must have at least one role - you cannot remove a user's last role without adding a new one. However, you cannot add a role directly to an account (e.g., to add the Reader role so you can remove the Journal Editor role) and must instead invite them to the new Role.

If the user does not accept the invitation, you can either Disable the account or Remove it. In cases where you do not want to do this, you can [contact YDJ](ydj-contact.md) for assistance.

!!! warning

    Do not try to remove accounts for YDJ administrators. As of August 2026, these include Tomasz Mrozewski (usually with the admin username and tmrozews@yorku.ca address, but sometimes includes testing accounts) or Ted Belke (usually tbelke tbelke@yorku.ca).

### 5.2 Roles  

Do not touch.  

### 5.3 Site Access Options  

* **User Registration**: use this to toggle whether users can create their own accounts. If your journal is operational, you likely want authors and reviewers to create their own accounts.

### 5.4 ORCID

Do not touch.
