=== Simple Local Avatars ===
Contributors: jakemgold, 10up, thinkoomph
Donate link: https://10up.com/plugins/simple-local-avatars-wordpress/
Tags: avatar, gravatar, user photos, users, profile
Requires at least: 4.6
Tested up to: 6.0
Requires PHP: 5.6
Stable tag: 2.4.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Adds an avatar upload field to user profiles. Generates requested sizes on demand just like Gravatar!

== Description ==

Adds an avatar upload field to user profiles if the current user has media permissions. Generates requested sizes on demand just like Gravatar! Simple and lightweight.

Just edit a user profile, and scroll down to the new "Avatar" field. The plug-in will take care of cropping and sizing!

1. Stores avatars in the "uploads" folder where all of your other media is kept
1. Has a simple, native interface
1. Fully supports Gravatar and default avatars if no local avatar is set for the user - but also allows you turn off Gravatar
1. Generates the requested avatar size on demand (and stores the new size for efficiency), so it looks great, just like Gravatar!
1. Let's you decide whether lower privilege users (subscribers, contributors) can upload their own avatar
1. Enables rating of local avatars, just like Gravatar

== Installation ==

1. Install easily with the WordPress plugin control panel or manually download the plugin and upload the extracted folder to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress
1. If you only want users with file upload capabilities to upload avatars, check the applicable option under Settings > Discussion
1. Start uploading avatars by editing user profiles!

Use avatars in your theme using WordPress' built in `get_avatar()` function: [http://codex.wordpress.org/Function_Reference/get_avatar](http://codex.wordpress.org/Function_Reference/get_avatar "get_avatar function")

You can also use `get_simple_local_avatar()` (with the same arguments) to retreive local avatars a bit faster, but this will make your theme dependent on this plug-in.

== Screenshots ==

1. Avatar upload field on a user profile page

== Changelog ==

= 2.4.0 - 2022-05-10 =
* **Added:** Ability to set a default avatar. (props [@mehulkaklotar](https://github.com/mehulkaklotar), [@jeffpaul](https://github.com/jeffpaul), [@dinhtungdu](https://github.com/dinhtungdu), [@faisal-alvi](https://github.com/faisal-alvi) via [#96](https://github.com/10up/simple-local-avatars/pull/96)).
* **Fixed:** Correct plugin name in changelog. (props [@grappler](https://github.com/grappler), [@jeffpaul](https://github.com/jeffpaul) via [#117](https://github.com/10up/simple-local-avatars/pull/117)).
* **Fixed:** Avatar cache not being cleared. (props [@thefrosty](https://github.com/thefrosty), [@jeffpaul](https://github.com/jeffpaul), [@faisal-alvi](https://github.com/faisal-alvi), [@peterwilsoncc](https://github.com/peterwilsoncc) via [#118](https://github.com/10up/simple-local-avatars/pull/118) & [#120](https://github.com/10up/simple-local-avatars/pull/120)).
* **Security:** Dev dependency `@wordpress/scripts` upgraded to resolve deeper level dependency security issues. (props [@jeffpaul](https://github.com/jeffpaul), [@faisal-alvi](https://github.com/faisal-alvi), [@cadic](https://github.com/cadic) via [#119](https://github.com/10up/simple-local-avatars/pull/119)).

= 2.3.0 - 2022-04-25 =
* **Added:** Crop screen (props [@jeffpaul](https://github.com/jeffpaul), [@helen](https://github.com/helen), [@ajmaurya99](https://github.com/ajmaurya99), [@Antonio-Lagun](https://github.com/Antonio-Lagun), [@faisal-alvi](https://github.com/faisal-alvi)).
* **Added:** Avatar preview for Subscribers (props [@ankitguptaindia](https://github.com/ankitguptaindia), [@dinhtungdu](https://github.com/dinhtungdu), [@dkotter](https://github.com/dkotter)).
* **Added:** More robust multisite support and shared avatar setting (props [@adamsilverstein](https://github.com/adamsilverstein), [@helen](https://github.com/helen), [@jeffpaul](https://github.com/jeffpaul), [@dkotter](https://github.com/dkotter), [@faisal-alvi](https://github.com/faisal-alvi), [@holle75](https://github.com/holle75)).
* **Added:** Settings link to plugin action links (props [@rahulsprajapati](https://github.com/rahulsprajapati), [@jeffpaul](https://github.com/jeffpaul), [@iamdharmesh](https://github.com/iamdharmesh)).
* **Added:** Dashboard setting and WP-CLI command to migrate avatars from [WP User Avatar](https://wordpress.org/plugins/wp-user-avatar/) (props [@jeffpaul](https://github.com/jeffpaul), [@claytoncollie](https://github.com/claytoncollie), [@helen](https://github.com/helen), [@faisal-alvi](https://github.com/faisal-alvi)).
* **Added:** Option to clear cache of user meta to remove image sizes that do not exist (props [@jeffpaul](https://github.com/jeffpaul), [@ituk](https://github.com/ituk), [@dinhtungdu](https://github.com/dinhtungdu), [@sparkbold](https://github.com/sparkbold), [@thrijith](https://github.com/thrijith)).
* **Added:** Package file (props [@faisal-alvi](https://github.com/faisal-alvi), [@jeffpaul](https://github.com/jeffpaul), [@claytoncollie](https://github.com/claytoncollie), [@cadic](https://github.com/cadic)).
* **Added:** PHP Unit Tests (props [@faisal-alvi](https://github.com/faisal-alvi), [@iamdharmesh](https://github.com/iamdharmesh)).
* **Added:** "No Response" GitHub Action (props [@jeffpaul](https://github.com/jeffpaul)).
* **Changed:** Bump WordPress "tested up to" version to 5.9 (props [@jeffpaul](https://github.com/jeffpaul), [@ankitguptaindia](https://github.com/ankitguptaindia), [@dinhtungdu](https://github.com/dinhtungdu), [@phpbits](https://github.com/phpbits)).
* **Changed:** Bump WordPress "tested up to" version to 6.0 (props [@ajmaurya99](https://github.com/ajmaurya99) via [#110](https://github.com/10up/simple-local-avatars/pull/110)).
* **Changed:** Format admin script (props [@thrijith](https://github.com/thrijith), [@dinhtungdu](https://github.com/dinhtungdu)).
* **Fixed:** Media ID as string in REST API (props [@diodoe](https://github.com/diodoe), [@dinhtungdu](https://github.com/dinhtungdu), [@dkotter](https://github.com/dkotter)).
* **Fixed:**  Avatar rating text is not translated properly if a user has a custom language Set (props [@ActuallyConnor](https://github.com/ActuallyConnor), [@faisal-alvi](https://github.com/faisal-alvi)).
* **Security:** PHP 8 compatibility (props [@faisal-alvi](https://github.com/faisal-alvi), [@dkotter](https://github.com/dkotter), [@Sidsector9](https://github.com/Sidsector9)).
* **Security:** Bump `rmccue/requests` from 1.7.0 to 1.8.0 (props [dependabot@](https://github.com/dependabot)).
* **Security:** Bump `nanoid` from 3.1.28 to 3.2.0 (props [dependabot@](https://github.com/dependabot)).
* **Security:** Bump `minimist` from 1.2.5 to 1.2.6 (props [dependabot@](https://github.com/dependabot)).

= 2.2.0 - 2020-10-27 =
* **Added:** `$args` parameter to `get_simple_local_avatar` function (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/), [@heyjones](https://github.com/heyjones), [@dkotter](https://profiles.wordpress.org/dkotter/), [@sumnercreations](https://github.com/sumnercreations), [@dshanske](https://profiles.wordpress.org/dshanske/)).
* **Added:**  `Simple_Local_Avatars::get_avatar_data()`, `Simple_Local_Avatars::get_simple_local_avatar_url()`, and `Simple_Local_Avatars::get_default_avatar_url()` methods (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/), [@heyjones](https://github.com/heyjones), [@dkotter](https://profiles.wordpress.org/dkotter/), [@sumnercreations](https://github.com/sumnercreations), [@dshanske](https://profiles.wordpress.org/dshanske/)).
* **Added:** Ability to retrieve avatar with `WP_Post` object (props [@oscarssanchez](https://profiles.wordpress.org/oscarssanchez), [@blobaugh](https://profiles.wordpress.org/blobaugh)).
* **Added:** class and ID to Avatar section on Profile Page to allow easier styling (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/)).
* **Added:**  [WP Acceptance](https://github.com/10up/wpacceptance/) test coverage (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/)).
* **Changed:** Switched to `pre_get_avatar_data` filter (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/), [@heyjones](https://github.com/heyjones), [@dkotter](https://profiles.wordpress.org/dkotter/), [@sumnercreations](https://github.com/sumnercreations), [@dshanske](https://profiles.wordpress.org/dshanske/)).
* **Changed:** `assign_new_user_avatar` function to public (props [@tripflex](https://profiles.wordpress.org/tripflex/)).
* **Changed:** Split the main class into its own file, added unit tests, and set up testing GitHub action (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/), [@helen](https://profiles.wordpress.org/helen/), [@stevegrunwell](https://profiles.wordpress.org/stevegrunwell/)).
* **Changed:** New plugin banner and icon (props [@JackieKjome](https://profiles.wordpress.org/jackiekjome/)).
* **Changed:** Bump WordPress version "tested up to" 5.5 (props [@Waka867](https://github.com/Waka867), [@tmoorewp](https://profiles.wordpress.org/tmoorewp), [@jeffpaul](https://profiles.wordpress.org/jeffpaul), [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/)).
* **Changed:** GitHub Actions from HCL to YAML workflow syntax (props [@jeffpaul](https://profiles.wordpress.org/jeffpaul)).
* **Changed:** Documentation updates (props [@jeffpaul](https://profiles.wordpress.org/jeffpaul)).
* **Fixed:** Initialize `Simple_Local_Avatars` on the `$simple_local_avatars` global, enabling bundling plugin with composer (props [@pauldewouters](https://profiles.wordpress.org/pauldewouters/), [@adamsilverstein](https://profiles.wordpress.org/adamsilverstein)).
* **Removed:** `get_avatar` function that overrides the core function (props [@dinhtungdu](https://profiles.wordpress.org/dinhtungdu/), [@heyjones](https://github.com/heyjones), [@dkotter](https://profiles.wordpress.org/dkotter/), [@sumnercreations](https://github.com/sumnercreations), [@dshanske](https://profiles.wordpress.org/dshanske/)).

= 2.1.1 - 2019-05-07 =
* Fixed: Do not delete avatars just because they don't exist on the local filesystem. This was occasionally dumping avatars when WordPress uploads were stored elsewhere, e.g. a cloud service.

= 2.1 - 2018-10-24 =
* *New:* All avatar uploads now go into the media library. Don't worry - users without the ability to upload files cannot otherwise see the contents of your media library. This allows local avatars to respect other functionality your site may have around uploaded images, such as external hosting.
* *New:* REST API support for getting and updating.
* *New:* Use .org language packs rather than bundling translations.
* *Fixed:* Avoid an `ArgumentCountError`.
* *Fixed:* A couple of internationalization issues.

= 2.0 - 2013-06-02 =
* Choose or upload an avatar from the media library (for users with appropriate capabilities)!
* Local avatars are rated for appropriateness, just like Gravatar
* A new setting under Discussion enables administrators to turn off Gravatar (only use local avatars)
* Delete the local avatar with a single button click (like everywhere else in WordPress)
* Uploaded avatar file names are appended with the timestamp, addressing browser image caching issues
* New developer filter for preventing automatic rescaling: simple_local_avatars_dynamic_resize
* New developer filter for limiting upload size: simple_local_avatars_upload_limit
* Upgraded functions deprecated since WordPress 3.5
* Fixed translations not working on front end (although translations are now a bit out of date...)
* Hungarian translation added (needs further updating again with new version)
* Assorted refactoring / improvements under the hood

= 1.3.1 - 2011-12-29 =
* Brazilian Portuguese and Belarusian translations
* Bug fixes (most notably correct naming of image files based on user display name)
* Optimization for WordPress 3.2 / 3.3 (substitutes deprecated function)

= 1.3 - 2011-09-22 =
* Avatar file name saved as "user-display-name_avatar" (or other image extension)
* Russian localization added
* Assorted minor code optimizations

= 1.2.4 - 2011-07-02 =
* Support for front end avatar uploads (e.g. Theme My Profile)

= 1.2.3 - 2011-04-04 =
* Russian localization

= 1.2.2 - 2011-03-25 =
* Fix for avatars uploaded pre-1.2.1 having a broken path after upgrade

= 1.2.1 - 2011-01-26 =
* French localization
* Simplify uninstall code

= 1.2 - 2011-01-26 =
* Fix path issues on some IIS servers (resulting in missing avatar images)
* Fix rare uninstall issues related to deleted avatars
* Spanish localization
* Other minor under the hood optimizations

= 1.1.3 - 2011-01-20 =
* Properly deletes old avatars upon changing avatar
* Fixes "foreach" warning in debug mode when updating avatar image

= 1.1.2 - 2011-01-18 =
* Norwegian localization

= 1.1.1 - 2011-01-18 =
* Italian localization

= 1.1 - 2011-01-18 =
* All users (regardless of capabilities) can upload avatars by default. To limit avatar uploading to users with upload files capabilities (Authors and above), check the applicable option under Settings > Discussion. This was the default behavior in 1.0.
* Localization support; German included

= 1.0 - 2011-01-18 =
* Initial release.

== Upgrade Notice ==

= 2.1 =
*Important note:* All avatar uploads now go into the media library. Don't worry - users without the ability to upload files cannot otherwise see the contents of your media library. This allows local avatars to respect other functionality your site may have around uploaded images, such as external hosting.

= 2.0 =
Upgraded to take advantage of *WordPress 3.5 and newer*. Does not support older versions! This has also *not* been tested with front end profile plug-ins - feedback welcome. Note that several language strings have been added or modified - revised translations would be welcome!

= 1.3.1 =
Like WordPress 3.2, now *REQUIRES* PHP 5.2 or newer.
