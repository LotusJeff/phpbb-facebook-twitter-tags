phpbb-facebook-twitter-tags
===========================

phpBB Dynamic Facebook and Twitter Header Tags


This phpBB modification will:
Install Facebook Open Graph Meta Tags.
Install Twitter Cards Meta Tags.
Use first posting content of a topic to populate the og:description and twitter:description meta tag. It will use the board description for all secondary pages.
Use the first image posted, if present, to populate the og:image and twitter:image meta tag. It will use a default image if no image is present.
Will work on all pages within the forums.

Requirements: 
This mod requires the Canonical URL modification. (if you have another canonical mod, it will also work, like php-SEO.)

Features:
Use real content from the first topic posting to populate the description field. Makes each Facebook and Twitter post custom.
Uses the first photo from the posting, to populate the Facebook. This enables your Facebook page to have unique photos for each topic.

Demo URL: This modification has been implemented on this forum. http://www.lotuselan.net/forums 

This modification will end with the following items populated within your header:
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
