---
sidebar_position: 2
---

New deprecations
================

:::caution TODO

This page is unfinished, please use the **Edit this Page** link at the bottom of this page to help make it more useful.

:::

All the new deprecations that should be aware of and what you should now be using instead.

# Language strings

File: `administrator/language/en-GB/com_content.ini`

Strings will be removed in 6.0: 
* `COM_CONTENT_RUN_TRANSITION`, use `JWORKFLOW_RUN_TRANSITION` instead 
* `COM_CONTENT_WORKFLOW_STAGE`, use `JWORKFLOW_STAGE` instead 

# Class deprecations

Planned to be removed in Joomla! 7.0.

### Banner component helper

File: `components/com_banners/src/Helper/BannerHelper.php`

Replacement: no replacement

The function `BannerHelper::isImage($url)` has been replaced with a combination of 
`Joomla\CMS\Helper\MediaHelper::isImage($url)` for pixel-based image files and
`Joomla\CMS\Helper\MediaHelper::getMimeType($url) === 'image/svg+xml'` for vector based image files
after being sanitized with the helper function `Joomla\CMS\HTML\HTMLHelper::cleanImageURL($imageurl)`