# SilverStripe 4 CMS Tweaks
Module to add a series of tweaks/modifications to the SilverStripe CMS.
The goal is to make the CMS less confusing for non-technical users, removing
functionality some they can't use (ie: non SITETREE_REORGANISE users).

## Modifications (PHP,css/JavaScript) includes
- Move MetaDescription and ExtraMeta to it's own "Advanced tab"
- Adds MetaKeywords for those wanting to use them
- Page name, URL Segment, Navigation label not shown to users without `SITETREE_REORGANISE` permissions
  - Meta Title is displayed on the Advanced tab if no `SITETREE_REORGANISE` permissions
  - "Page name" renamed "Meta Title" to avoid confusion

- Always have the Advanced tab on the right (floated after all other tabs)
- JavaScript word/character count for MetaDescription
- Clean MetaDescription for any new lines and double-spaces upon save
- Dependent pages (if any) displayed on Advanced tab
- Hide add/Archive page buttons when user has no `SITETREE_REORGANISE` permissions
- Hide CMS ErrorPages to non-admin users in CMS as well as file/link selectors
- Remove SiteTree drag handle when user has no `SITETREE_REORGANISE` permissions
- Remove "Duplicate" content menu when user has no `SITETREE_REORGANISE` permissions
- Prevent accidental form submission in CMS when the enter key is used
- Add "Remove formatting" button to TinyMCE to clean code
- Link logo in CMS to website homepage rather than silverstripe.org
- Remove "Help" link

## Metadata Tab
The MetadataTab extension (by default) moves the Metadata information from below the Content field into its own tab.
Please refer to the [Metadata Tab documentation](docs/en/MetadataTab.md) for configuration options.

## Requirements
- SilverStripe ^4.0
