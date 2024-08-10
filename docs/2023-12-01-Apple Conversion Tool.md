# 2023-12-01-Apple Conversion Tool

Tool converts a Chrome Extension to a Safari Extension.

Apple conversion tool:  
https://developer.apple.com/documentation/safariservices/safari_web_extensions/converting_a_web_extension_for_safari

Run:
```
xcrun safari-web-extension-converter \
/Users/gturner/Developer/Work/dangerboard-browser-chrome/dangerboard-browser-chrome \
--macos-only
```

```
Xcode Project Location: /Users/gturner/Developer/Work/dangerboard-browser-safari
App Name: Dangerboard New Tab Start Page
App Bundle Identifier: com.yourCompany.Dangerboard-New-Tab-Start-Page
Platform: All
Language: Swift
Warning: The following keys in your manifest.json are not supported by your current version of Safari. If these are critical to your extension, you should review your code to see if you need to make changes to support Safari:
	newtab
	options_page
	storage
	manifest_version
	version
	description
	name
	icons
```
