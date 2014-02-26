phpbb-facebook-twitter-tags
===========================

phpBB Dynamic Facebook and Twitter Header Tags


###This phpBB modification will
* Install Facebook Open Graph Meta Tags.
* Install Twitter Cards Meta Tags.
* Use first posting content of a topic to populate the og:description and twitter:description meta tag. It will use the board description for all secondary pages.
* Use the first image posted, if present, to populate the og:image and twitter:image meta tag. It will use a default image if no image is present.
* Option to select the last image, based on a true/false parameter in the code.
* Will also populate a video image if [video] bbcode is used.
* Will work on all pages within the forums.

###Requirements 
* This mod requires the Canonical URL modification. (if you have another canonical mod, it will also work, like php-SEO.)
* Requires the use of [video] bbcode for video component.

###Features
* Use real content from the first topic posting to populate the description field. Makes each Facebook and Twitter post custom.
* Uses the first photo from the posting, to populate the Facebook. This enables your Facebook page to have unique photos for each topic.

###Demo URL

This modification has been implemented on this forum. http://www.lotuselan.net/forums 

### Instalation Instructions
####Step 1:

This mod requires a canonical URL modification to be installed for the og:url and twitter:url meta tags. 
phpBB does not have a template tag for the current page URL.
For this feature to work will require a dependent mod to be installed.
Options:
 * Canonical URL - This is listed in the Additional Files section to edit. This mod is written with this dependency.
 * phpBB-SEO - If you already have phpBB-SEO installed, then you can replace the {U_CANONICAL} with {SEO_CANONICAL_URL}. 
 * Other Mods - If you have some other mod that provides the current page. This can be a variety of share it type of mods.  You will need to find the corresponding tag and swap it out for the {U_CANONICAL} tag.

####Step 2:

You will need to replace "***Default image URL Goes Here***" with the URL for your default image.  Your non-topic pages and your topics that do not contain an image attachment will require a default image.  This will need to be the full url to the image including the http://.

####Step 3:

Permissions. 
Facebook uses a crawler/spider to collect the page information. If you have Facebook defined as a crawler, you will need to give crawlers access to download images. This is accomplished by going to:
1. Login to the ACP
2. Select "Permissions" tab.
3. Select "Group Permissions" in the left column.
4. Select "Crawlers" from the drop down box and click the "Submit" button.
5. Click the "Advanced Permissions" link in the right side of the white box.
6. The option called "Can download files", click the radio button for "Yes".
7. Click the "Apply Permissions" button.

####Step 4:

Test. You can go to Facebook Developers Toolbox and test your Open Graph tags at http://developers.facebook.com/tools/debug/.

###Results

This modification will end with the following items populated within your header:
```html
<meta property="og:locale" content="" />
<meta property="og:locale:alternate" content="" />
<meta property="og:type" content="" />
<meta property="og:title" content="" />
<meta property="og:url" content="" />
<meta property="og:site_name" content="" />
<meta property="og:description" content=""/>
<meta property="og:image" content="" />
<meta name="twitter:card" content="" />
<meta name="twitter:url" content="" />
<meta name="twitter:title" content="" />
<meta name="twitter:description" content=""/>
<meta name="twitter:image" content="" />
```
