![QA Tool](https://github.com/cirept/NextGen/blob/master/images/QA_tool_layout.png)<br>

# **Tool Descriptions**<br>
## Page Information Panel :new: [Jump To Instructions](#page-information-panel)
:one: [Dealer Name](#dealer-name)<br>
:two: [Web-ID](#web-id)<br>
:three: [Page Name](#page-name)<br>
:four: [H Tags](#h-tags)<br>

## QA Tools Panel :new:<br>
:one: [Image Checker](#image-checker)<br>
:two: [Link Checker](#link-checker) :sparkles:<br>
:three: [Spell Checker](#spellcheck-page)<br>
:four: [WebPageTest](#web-page-test)<br>
:five: [404 Link Checker](#404-link-checker) :sparkles:<br>

## Other Tools Panel :new:<br>
:one: [Show Navigation](#show-navigation)<br>
:two: [SEO Simplify](#seo-simplify)<br>

## Toggles Panel :new:<br>
:one: [Refresh Button](#refresh-button)<br>
:two: [Hide Preview Toolbar](#hide-preview-toolbar)<br>

## URL Modifiers Panel :new:<br>
:one: [Auto Apply Modifiers](#auto-apply-parameters)<br>
:two: [NextGen Parameter](#nextgen-parameter)<br>
:three: [Show Autofill Tags](#show-autofill-tags)<br>

<br>
<br>

---
---

<br>
<br>

# **Page Information Panel**<br>

![Page Information](https://github.com/cirept/NextGen/blob/master/images/QA_tool_layout_pageinformation.png)<br>

- This panel shows all important information for the current CDK website you are viewing.<br>

### Features<br>

![Page Information Highlight Feature](https://github.com/cirept/NextGen/blob/master/gifs/pageInfoHighlight_paste.gif)<br>

- Clicking on the info area will copy the text to your clipboard.<br>
***There will be no notification.***

<br>
<br>

---

<br>
<br>

## **Dealer Name**<br>

![Dealer Name](https://github.com/cirept/NextGen/blob/master/images/dealerNameFocus.png)<br>

- This area will display the current dealer's ***NAME*** of the CDK site you are viewing.<br>
- This dealer name should be the same name as the dealer's "Account" name in Salesforce.<br>

<br>
<br>

---

<br>
<br>

## **Web ID**<br>

![Web ID](https://github.com/cirept/NextGen/blob/master/images/webIDFocus.png)<br>

- This area will display the current dealer's ***WEB-ID*** of the CDK site you are viewing.<br>
- This web-id should be the same name as the dealer's "WebID" name in Salesforce.<br>
- This is also used to navigate to the dealer's site in WSM for editting.

<br>
<br>

---

<br>
<br>

## **Page Name**<br>

![Page Name](https://github.com/cirept/NextGen/blob/master/images/pageNameFocus.png)<br>

- This area will display the current ***PAGE NAME*** of the CDK site you are viewing.<br>
- This information is what the 'generic' page name of the page is called.<br>
- This will help navigate to a specific page while editting the site in WSM.<br>

*e.g. LandingPage, HoursAndDirections, MiscPage.*<br>

<br>
<br>

---

<br>
<br>

## **H Tags**<br>

![H Tag](https://github.com/cirept/NextGen/blob/master/images/hTagFocus.png)<br>

- This area will display the current h tags on the current page you are viewing.<br>
- Any h tags that have a Zero (0) value will be highlighted in orange.<br>

### ***Clicking on the area will bring a pop up with all the h tags displayed***<br>

![H Tag Display](https://github.com/cirept/NextGen/blob/master/gifs/htagdisplay_DEMO.gif)<br>

<br>
<br>

---
---

<br>
<br>

# **QA Tools Panel**<br>

- This panel has the main QA tools for checking the site.<br>

![QA Tools Panel](https://github.com/cirept/NextGen/blob/master/images/QA_tool_layout_qatools.png)<br>

## **Show Navigation**<br>

![Show Navigation DEMO](https://github.com/cirept/NextGen/blob/master/gifs/showNavDEMO.gif)<br>

### TIP:<br>
>*Show Navigation + Link Checker can and should be used together to verify links in the navigation are correct.*

- This tool will allow the user to see all of the navigation menu without having to hover over the main navigation item.<br>
- All subnavigation items will display for easier QA checking.<br>
- When you are done using the tool, simply click the "turn off" on the legend and the tool will turn itself off.<br>
***This tool works for both TETRA and NEXTGEN***<br>

### Turning the tool on:<br>

- Click the 'show navigation' button inside the 'qa tools' panel.<br>

### Turning the tool off:<br>

- When you are done using the tool, simply click the "turn off" on the legend and the tool will turn itself off.<br>


### **Features**<br>

| Show Navigation Functionality |
| --- |
| ![Show Navigation Functionality](https://github.com/cirept/NextGen/blob/master/images/showNavigation.png) |
| When clicking on any subnavigation item, it will turn the link a different color to signify that you have checked the link.<br>***Added to help keep track of what links you have already checked.*** |


| Show Navigation Legend |
| --- |
| ![Show Navigation Legend](https://github.com/cirept/NextGen/blob/master/images/showNavigationLegend.png) |
| ***The "major page" color will only be applied when the tool is run on a TETRA site.  NEXTGEN has this feature disabled.*** |


<br>
[Back to Top](#tool-descriptions)<br>
<br>

---
---

<br>
<br>


## **Link checker**<br>

![Link Checker DEMO](https://github.com/cirept/NextGen/blob/master/gifs/linkCheckerDEMO.gif)<br>

### TIP:<br>

>*Show Navigation + Link Checker can and should be used together to verify links in the navigation are correct.*

- All links on the page will be highlighted with specific colors according to the validity of the link.<br>
- There are various factors that the tool will use to categorize each link.<br>
- More detail on those factors are stated below.<br>
***This tool works for both TETRA and NEXTGEN***

### Turning the tool on:<br>

- Click the 'link checker' button inside the 'qa tools' panel.<br>

### Turning the tool off:<br>

- When you are done using the tool, simply click the "turn off" on the legend and the tool will turn itself off.<br>

### **Features**<br>

| Link Checker Legend |
|---|
| ![Link Checker Legend](https://cdn.rawgit.com/cirept/NextGen/5567c3d4/images/linkCheckerLegend.png) |
| ***'HAS NO title text'*** |
| All links that DO NOT HAVE title text in the link will be flagged |
| ***'HAS title text'*** |
| All links that HAVE title text in the html code will be flagged |
| ***'OPENS IN A NEW WINDOW'*** |
| All links that have 'targets' with these values will be flagged<br>_blank<br>_new<br>custom<br> |
| ***'EMPTY OR UNDEFINED URL'*** |
| All links that do not contain an href value will be flagged |
| ***'CHECK URL'*** |
| All links that have href these values will be flagged<br>&#35;<br>f_<br>>www<br>http |
| ***'PAGE NOT SUPPORTED'*** |
| All links that lead to a page that is no longer supported on NEXTGEN will have this border.<br>Please update the link to lead to a related page that is supported on NEXTGEN.<br><br>**Pages No Longer Supported on NEXTGEN**<br>1.	NewVehicleSearch<br>2.	PreOwnedVehicleSearch<br>3.	NewVehicleInfoForm<br>4.	PreOwnedVehicleInfoForm<br>5.	ExtendedProtection<br>6.	ExtendedProtectionDetails<br>7.	Affiliate<br>8.	AboutSpecials<br><br>***additional details to what page the links should be updated too will be coming soon***|


| Link Checker Functionality |
| --- |
| ![Link Checker Functionality](https://cdn.rawgit.com/cirept/NextGen/5567c3d4/images/linkChecker.png) |
| The links will turn a highlighted color to signify that you have checked the link.  Added for ease of use when QA'ing |

<br>
[Back to Top](#tool-descriptions)<br>
<br>

---
---

<br>
<br>


## **Image Checker**<br>

![Image Alt Checker DEMO](https://github.com/cirept/NextGen/blob/master/gifs/imageAltCheckerDEMO.gif)<br>

- All images on the page will be highlighted in specific colors that will tell the user what images **have** and **do not have** alt text.<br>
- **If using this tool on a NEXTGEN site**, please scroll all the way to the bottom of the page to allow all images to load before running the tool.<br>
- Due to lazy loading, if the tool is run and some images do not have a box around the image please turn off the tool and rerun the tool with that image in view.<br>
***This tool works for both TETRA and NEXTGEN***<br>

### Turning the tool on:<br>

- Click the 'image alt checker' button inside the 'qa tools' panel.<br>

### Turning the tool off:<br>

- When you are done using the tool, simply click the "turn off" on the legend and the tool will turn itself off.<br>

### **Features**<br>

| Image Checker Functionality |
| ----------------------------- |
| ![Show Navigation Functionality](https://cdn.rawgit.com/cirept/NextGen/5567c3d4/images/imageAltChecker.png) |
| All images on the page will be highlighted with a green or red/pink box.  These colors will signify if the image **has** and **does not have** an alt text.<br>If the image has a green color on over the image, the ALT of the image will appear at the center. |


| Image Checker Legend |
| --- |
| ![Show Navigation Legend](https://cdn.rawgit.com/cirept/NextGen/5567c3d4/images/imageCheckerLegend.png) |

<br>
[Back to Top](#tool-descriptions)<br>
<br>

---
---

<br>
<br>


## **Spellcheck Page**<br>

![Spellcheck Page](https://github.com/cirept/NextGen/blob/master/gifs/seoSimplifyDEMO.gif)<br>

- This tool will send the current page to be spell checked via third party website, W3.org.<br>

### **Features**<br>

- A new tab will open with the page already queued up for spell checking.<br>
- Once the spell checking is complete the page will autofill with all the ***possible*** miss-spelled words.<br>

| Spell Check Results Example |
| --- |
| ![Spell Check Results](https://cdn.rawgit.com/cirept/NextGen/367ce2a9/images/spellCheck.png) |
| ***Please verify that all the words on the page is in fact spelt wrong*** |


<br>
[Back to Top](#tool-descriptions)<br>
<br>

---
---

<br>
<br>


## **404 Checker**<br>

![404 Link Checker DEMO](https://github.com/cirept/NextGen/blob/master/gifs/link404CheckerDEMO.gif)<br>

- This tool will check every link on the site and highlight the link according to what the results of the test is.<br>
- All the links on the page will be tested for validity and then will be highlighted accordingly.<br>
- For the most part only links that are internal links will be eligible to be flagged as 'Link is Real' due to security restrictions.<br>
***This tool works for both TETRA and NEXTGEN***<br>

### Turning the tool on:<br>

- Click the '404 link checker' button inside the 'qa tools' panel.<br>

### Turning the tool off:<br>

- When you are done using the tool, **please refresh the page** before running any other tool.<br>

### **Features**<br>

| 404 Link Checker Legend |
| --- |
| ![404 Link Checker Legend](https://github.com/cirept/NextGen/blob/master/images/link404checkerLegend.png) |
| ***'Absolute URL*'*** |
| All links that have a complete URL (e.g. http://nitra.wip.gmpsdealer.com/content15/VehicleSearchResults?search=new) as the link will be flagged.<br> All links that lead outside the site (e.g. https://confluence.cdk.com/display/DEV/CX+Innovation) will be flagged.<br> |
| ***'f_link'*** |
| All links that force the page to be framed in.<br>**This is more common on TETRA then in NEXTGEN** |
| ***'Empty URL'*** |
| All links that have an *empty* url.<br> All links that begin with a "#". *links are usually related to anchor links OR is meant to bring the user back to the homepage.*<br> All links that are meant for mobile. *phone number links on NEXTGEN that will. *e.g. phone link in the masthead on a NEXTGEN site* |
| ***'Link is Real'*** |
| All links that lead to an actual page will be flagged. |
| ***'404 Link'*** |
| All links that result in a 404 error (link leads to a page that doesn't exist) with be flagged and should be addressed. |


<br>
[Back to Top](#tool-descriptions)
<br>

---
---

<br>
<br>


## **Web Page Test**<br>

![Web Page Test DEMO](https://github.com/cirept/NextGen/blob/master/gifs/webpagetestDEMO.gif)<br>

- This tool will send in a query to WebPageTest.org of the currently viewed page.<br>
- When clicking 'Web Page Test' button, a submenu will appear with advanced settings. These default settings will result in a typical test and should only be changed under specific circumstances.<br>
***This tool works for both TETRA and NEXTGEN***<br>

### Turning the tool on:<br>

- Click the 'web page test' button inside the 'qa tools' panel.<br>

### **Features**<br>

###### Enter Email<br>

- Filling out this field with your work email (e.g. firstName.lastName@cdk.com) will send you an email when your tests have been completed.<br>

###### Choose Browser<br>

- This setting will change the browser that your tests will be conducted in.<br>
- The three (3) major browsers are available to choose from.<br>
- By default IE11 is the ideal test candidate and should always be set as the browser to test in.<br>
- The only scenario that the browser settings should be changed is in the event that the IE11 servers are down, at which point selecting any of the remaining two (2) browsers will be necessary.

###### Choose Key<br>

- This setting has been introduced to allow additional users to send in tests using this tool.<br>
**Each key is alotted a total of 200 tests per day.**<br>
***Every query request sent by this tool results in a total of three (3) tests*** to be made, so as you can see that reaching that 200 limit per day can be quite easy.<br>
- In the event that you receive an error message upon viewing the results page on WebPageTest.org mentioning the limit has been reached for the day, please choose a different key from the drop down and send in another test.<br>

## Results<br>

- Once the setting have been set up, hit the 'send test' button and your test will be sent in.<br>
- A new tab will open with the page already queued up for speed testing.<br>
- Once the testing has been completed the results of the test will be displayed.<br>

![Web Page Test Results](https://github.com/cirept/NextGen/blob/master/images/webPageTestResults.jpg)<br>

>
>The results will show the page load times for the site. The results page will also help with determining what is causing slow load times if necessary.<br>
>
>Benchmark for desktop site = load time < 10 sec.
>

<br>
[Back to Top](#tool-descriptions)
<br>

---
---

<br>
<br>


# **Other Tools Panel**<br>

![Other Tools Panel Highlight](https://github.com/cirept/NextGen/blob/master/images/QA_tool_layout_qatools.png)

## **SEO Simplify**<br>

![SEO Simplify DEMO](https://github.com/cirept/NextGen/blob/master/gifs/seoSimplifyDEMO.gif)<br>

- This tool will aid in formatting SEO text that is taken from a live site that is formatted using css.<br>
- This tool will provide a simplified version of the code you input.  Ready for pasting into a NextGen card.<br>
***This tool works for both TETRA and NEXTGEN***<br>

### Turning the tool on:<br>

- Click the 'seo simplify' button inside the 'other tools' panel.<br>

### **Features**<br>

- After raw SEO text has been entered, a pop up will display with the 'simplified' SEO text.<br>
- All styles, italics, bold, center, underline, span tags will be removed.<br>
- The pop up will have display the SEO text according to the styles of the current page you are on.<br>
- Clicking in the text area will allow the user to copy all of the html code of the new SEO text.<br>

- To remove the pop up, click on the 'remove' button at the top of the pop up.<br>

<br>
[Back to Top](#tool-descriptions)
<br>

---
---

<br>
<br>


# **Toggles Panel**<br>

![Toggles Panel](https://github.com/cirept/NextGen/blob/master/images/QA_tool_layout_toggles.png)

- These tools are here to make for convenience's sake.<br>

## **Refresh Button**<br>

![Refresh Button DEMO](https://github.com/cirept/NextGen/blob/master/gifs/refreshButtonDEMO.gif)

- This tool will allow access to a refresh button that will provide a similar functionality as using the keyboard shortcut ctrl+f5 on a webpage.<br>
- To hide/show the button, switch the control on/off.<br>
**This tool works for both TETRA and NEXTGEN.**


<br>
<br>


## **Hide Preview Toolbar**<br>

![Hide Preview Toolbar DEMO](https://github.com/cirept/NextGen/blob/master/gifs/hidePreviewToolbarDEMO.gif)

- This tool will hide the PCE toolbar that appears at the top of CDK sites.<br>
- To hide/show the button, switch the control on/off.<br>
**This tool works for both TETRA and NEXTGEN.**<br>


<br>
<br>

----
----

<br>
<br>


# **URL Modifiers Panel**<br>

![URL Modifier Panel Highlight](https://github.com/cirept/NextGen/blob/master/images/QA_tool_layout_urlModifiers.png)

## **Auto Apply Modifiers**<br>

This tool allows the tool to automatically apply the URL parameters of the URL modifications within this panel.  When switching this toggle on, it will determine if the current page you are viewing has the desired URL parameters added to it.  If the URL is missing a parameter the page will automatically refresh with the URL parameter added to it.

Test Scenario<br>
- e.g. *current URL* = http://nitra.proof.gmpsdealer.com/content15<br>
- I want to see the NEXTGEN version of my sandbox TETRA site and also want to make sure that all subsequent windows that I open are also the NEXTGEN version of my sandbox site.<br>
1.   I switch the **'nextgen parameters?'** toggle **ON**<br>
2.   Then I switch the **'auto apply modifiers?'** toggle **ON**.

- This will cause the page to refresh and the NEXTGEN version of the site visible.<br>
- *new URL* = http://nitra.proof.gmpsdealer.com/content15?nextGen=true<br>
- These settings will also automatically apply 'nextGen=true' to all windows that I open from now on, until I turn the 'auto apply modifiers?' toggle ***off***


<br>
<br>


## **Nextgen Parameters?**<br>

This tool controls the logic of the 'auto apply modifiers' toggle.  When switching this toggle into the **ON** or **OFF** position will cause the main tool to act differently.  **This tool works in both TETRA and NEXTGEN.  **This is also how you control which version of the tool you want touse.**

### ON position *pic here

This will cause the 'auto apply modifiers' tool (when switched on) to search the current URL and see if ***"nextGen=true"*** is present in the URL.


- If the parameter is not detected the tool will refresh the page with the parameter added to it.
     - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15~~
     - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?nextGen=true
- If ***"nextGen=false"*** is detected in the URL, the page will refresh with the parameter now having a ***false*** value.
    - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15?nextGen=false~~
    - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?nextGen=true
- If  ***"nextGen=true"*** is detected in the URL, nothing will happen.  :]
    - **URL** = http://nitra.proof.gmpsdealer.com/content15?nextGen=true

<br>
### OFF position *pic here

This will cause the 'auto apply modifiers' tool (when switched on) to search the current URL and see if ***"nextGen=false"*** is present in the URL.
- If the parameter is not detected the tool will refresh the page with the parameter added to it.
    - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15~~
    - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?nextGen=false
- If ***"nextGen=true"*** is detected in the URL, the page will refresh with the parameter now having a ***false*** value.
     - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15?nextGen=true~~
    - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?nextGen=false
- If ***"nextGen=false"*** is detected in the URL, nothing will happen. :]
    - http://nitra.proof.gmpsdealer.com/content15?nextGen=false


<br>
<br>


## Show Autofill Tags?<br>

This tool controls the logic of the 'auto apply modifiers' toggle.  When switching this toggle into the **ON** or **OFF** position will cause the main tool to act differently.  **This tool works in both TETRA and NEXTGEN.**

### ON position *pic here

This will cause the 'auto apply modifiers' tool (when switched on) to search the current URL and see if ***"disableAutofill=true"*** is present in the URL.


- If the parameter is not detected the tool will refresh the page with the parameter added to it.
     - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15~~
     - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?disableAutofill=true
- If ***"disableAutofill=false"*** is detected in the URL, the page will refresh with the parameter now having a ***false*** value.
    - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15?disableAutofill=false~~
    - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?disableAutofill=true
- If  ***"disableAutofill=true"*** is detected in the URL, nothing will happen.  :]
    - **URL** = http://nitra.proof.gmpsdealer.com/content15?disableAutofill=true

<br>
### OFF position *pic here

This will cause the 'auto apply modifiers' tool (when switched on) to search the current URL and see if ***"disableAutofill=false"*** is present in the URL.
- If the parameter is not detected the tool will refresh the page with the parameter added to it.
    - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15~~
    - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?disableAutofill=false
- If ***"disableAutofill=true"*** is detected in the URL, the page will refresh with the parameter now having a ***false*** value.
     - **OLD URL** = ~~http://nitra.proof.gmpsdealer.com/content15?disableAutofill=true~~
    - **NEW URL** = http://nitra.proof.gmpsdealer.com/content15?disableAutofill=false
- If ***"disableAutofill=false"*** is detected in the URL, nothing will happen. :]
    - http://nitra.proof.gmpsdealer.com/content15?disableAutofill=false
