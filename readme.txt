=== BP TimeZones ===
Contributors: philopress.com
Author URI: http://philopress.com/contact/
Plugin URI: http://philopress.com/products/
Requires at least: WP 3.9, BP 2.1
Tested up to: WP 3.9, BP 2.1
Stable tag: 1.0
License: GPLv2 
  

== Description == 
BP TimeZones is a BuddyPress plugin. 
It allows a member to select a Time Zone from Profile -> Edit. 
The timestamp on their messages will reflect that timezone. 


== Installation ==

1. Unzip.

2.  A)  In loader.php -> function bp_add_timezone_list() -> $field_group_id = 1;
		 Change '$field_group_id' to the number of the the Profile Group that should include the Time Zones dropdown. 
	B)  In loader.php -> function bp_add_timezone_list() 
		 Change both instances of the name 'Time Zone' if you wish. 
	C)  In bp_timezones.php -> function bp_custom_message_date() -> $member_zone = bp_get_member_profile_data('field=Time Zone');
		 If you edit the profile field name to something other than 'Time Zone', change the field name to the new name. 
	
3. Upload the 'bp-timezones' folder to the '/wp-content/plugins/' directory

4. Activate the plugin through the 'Plugins' menu in WordPress

