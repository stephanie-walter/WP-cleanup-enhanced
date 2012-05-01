WP-cleanup-enhanced
===================

WP-cleanup-enhanced is a plugin/code snippet to clean up WordPress admin.
In this plugin I put togheter many snippets to clean up the admin part of WordPress. It was inpired by the <a href="http://wordpress.org/extend/plugins/selfish-fresh-start/">Selfish fresh Start plugin</a>
I did not provide an administration area, there are many plugins like adminize that do the job very well. This plugin is more oriented towards developers that don't need a wysiwyg interface, and just want to clean up there client's admin area from everything the client does not need

Usage: 
===================

This code is provided as a plugin, bug you can also copy/paste some snippets individually to your functions.php file. 
I highly commented the code, so you will just have to read and follow instructions to see what each snippet does.

Functionnalities
===================
- remove_dashboard_widgets  : removed the dashboard widgets you don't need
- delete_menu_items: delete entries in the dashboard for menus and submenus (you can still access them if you know the url) 
	- syntaxe for the menus:  remove_menu_page( $menu_slug )
	- syntaxe for the submenus: remove_submenu_page( $menu_slug, $submenu_slug )
- customize_meta_boxes: remove useless meta boxes from page and posts area
- custom_post_columns: removes columns from the list of posts. Syntaxe: unset($defaults['columnID'])
- custom_pages_columns: removes columns from the list of pages. Syntaxe: unset($defaults['columnID'])
- wce_admin_bar_render:  removes items from the admin bar. Syntaxes: remove_menu(‘ID sans wp-admin-bar-)
- unregister_default_widgets: removes default WordPress widgets from the widget page
- rynonuke_update_notification_nonadmins: hide notification for non admin users
- rynonuke_self_pings: disable self-tracking
- rynonuke_dolly: deletes hellodolly plugin
- rynonuke_contactmethods: adds twitter and facebook contact method to user profil

The plugin also has some basic header clean-ups (see "Security + header clean-ups" part of the code)

The plugin also comes with two style sheets : custom_admin.css enables you to custom the admin css, and custom_login.css to change the login css (for example adding the client's logo, etc.)