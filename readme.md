# Bridgy Publish #
**Contributors:** dshanske  
**Tags:** indieweb, POSSE, bridgy  
**Stable tag:** 1.2.1  
**Requires at least:** 4.7  
**Tested up to:** 4.7.1  
**License:** GPLv2 or later  
**License URI:** http://www.gnu.org/licenses/gpl-2.0.html  

[Bridgy](https://www.brid.gy) Publish Interface for your Site

## Description ##

People often post something on their web site, then post a copy elsewhere so that other people will see it.

[Bridgy Publish](https://www.brid.gy/about#publishing) is a service that will create a post on the appropriate site(Twitter, Facebook, Flickr). It 
generates the post by reading the HTML of your site. This means that the post is generates depends on your theme and any content generated by plugin.
Bridgy offers a preview mode on their site to test your theme.

This plugin is only a user interface for the Bridgy service and requires the [webmention](https://wordpress.org/plugins/webmention/) plugin to notify Bridgy
to post. It also stores a link to the syndicated version for display by [Syndication Links](https://wordpress.org/plugins/syndication-links/) or other uses.

Development/Issues/Feature Requests for the plugin only should be submitted through [Github](https://github.com/dshanske/bridgy-publish).

For development/issues/enhancements for the Brid.gy service, please submit on their [Github](https://github.com/snarfed/bridgy) page. Please read their About page 
for the features of the service prior to submission.


## Changelog ##

### Version 1.2.2 ###
	* Switch adding publish links to content to adding to footer
	* Remove async hook introduced in 1.2.0 due request
	* Errors returned by Bridgy display in the Post UI
	* Invert description for Backlink Option from Omit to Show due confusion

### Version 1.2.1 ###
	* Omit Links option not set on Micropub so will now pull from the default setting if the post setting is not enabled

### Version 1.2.0 ###
	* Add per post support for Bridgy backlink settings. Credit to @iamwebrocker for addition
	* Redo Settings Page and allow default to checked to be on a per-service basis.
	* Publish Now Works Off of a Cron Job Hook 5-10 seconds after the post is published
	* Support for Setting and Being Triggered by Micropub Syndication Requests
	* Storage of Syndication Preferences now stored in `mf2_` microformats 2 properties
	* Optionally set the Twitter post based on the post excerpt

### Version 1.1.1 ###
	* Fix compatibility with changes in Syndication Links and change storage to array from EOL separated string

### Version 1.1.0 ###
	* Remove Instagram setting as deprecated
	* Add Flickr setting as now supported
	* Change webmention support notice to activate on send_webmention per request
	* Comply with WordPress Standards

### Version 1.0.1 ###
	* Bug Fixes
	* If Indieweb Plugin is installed, move settings under that menu
	* If WP_DEBUG is set - send Publish entries to the error log

### Version 1.0.0 ###
	* Initial release
	* Takes over Syndication Links storage of Bridgy Publish links

