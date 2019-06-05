MyFontAwesomeIcons

Lets you implement custom Font-Awesome 5 icons for your forums.

Created by Ethan DeLong & Vintagedaddyo

This is a highly modified version of the plugin: MyForumIcons - Custom Forum Icons by Ethan DeLong

Specifically modified by Vintagedaddyo for Font-Awesome implementation after several user requests for something of the sort.


This will allow you to add custom Font-Awesome icons for your forums.


You can specify a css name to your forum's custom font-awesome icon by going to the ACP => Forum Management => Edit Forum.


localization support:

-english 
-englishgb
-espanol
-french
-italiano

What is new in version 1.2?

- updated css to reflect the past lock to close change
- Font Awesome upgrade from 4.7 to FA5
- input changed from previous example: fa-comments to fas, far, fab for example: fas fa-comments or far fa-comments or fab fa-discord etc, etc.


To Install:

1) Upload The Files, And Go to Admin CP And Activate it!

2) Edit Index template:

Home » Template Sets » Default Templates » Edit Template: index

find:

{$boardstats}

<dl class="forum_legend smalltext">
	<dt><span class="forum_status forum_on" title="{$lang->new_posts}"></span></dt>
	<dd>{$lang->new_posts}</dd>

	<dt><span class="forum_status forum_off" title="{$lang->no_new_posts}"></span></dt>
	<dd>{$lang->no_new_posts}</dd>

	<dt><span class="forum_status forum_offclose" title="{$lang->forum_closed}"></span></dt>
	<dd>{$lang->forum_closed}</dd>

	<dt><span class="forum_status forum_offlink" title="{$lang->forum_redirect}"></span></dt>
	<dd>{$lang->forum_redirect}</dd>
</dl>
<br class="clear" />


replace with:

{$boardstats}

<dl class="forum_legend smalltext">
  <dt><div class="forum_status forum_on" title="{$lang->new_posts}"><i class="fas fa-comments"></i></div></dt>
  <dd>{$lang->new_posts}</dd>

  <dt><div class="forum_status forum_off" title="{$lang->no_new_posts}"><i class="fas fa-comments"></i></div></dt>
  <dd>{$lang->no_new_posts}</dd>

  <dt><div class="forum_status forum_offclose" title="{$lang->forum_closed}"><i class="fas fa-lock"></i></div></dt>
  <dd>{$lang->forum_closed}</dd>

  <dt><div class="forum_status forum_offlink" title="{$lang->forum_redirect}"><i class="fas fa-link"></i></div></dt>
  <dd>{$lang->forum_redirect}</dd>
</dl>
<br class="clear" />



3) Go to forums Management Edit Forum Settings and edit each forum with your specific Font Awesome Icon.

The CSS name for the font awesome icon. For example: fas fa-comments

You can specify a css name to your forum's custom font-awesome icon by going to the ACP => Forum Management => Edit Forum.
