=== Linkoption ===
Contributors: aleksander.chuyan@gmail.com
Donate link: -
Tags: links, options
Requires at least: 3.0.1
Tested up to: 5.5
Stable tag: 4.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Plugin settings page: /wp-admin/options-general.php?page=linkoption

Available plugin options and fuctions:
- Adds attributes for external links in content when outputting the_content().
- Internal links are ignored.
- Enable nofollow attribute for external links (rel="nofollow").
- Open links in a new tab (target="_blank").
- Selection of post types.
- Filter for custom content (custom fields etc.): external_links_attributes.
Example usage:
$section2 = apply_filters("external_links_attributes", get_post_meta(get_the_ID(), "section2", true)); echo $section2;