# README

Using the Apple conversion tool:  

https://developer.apple.com/documentation/safariservices/safari_web_extensions/converting_a_web_extension_for_safari

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


## Issue

Got the following issue when trying to run on MacOS:

```
Command CodeSign failed with a nonzero exit code
```

- Found:
https://developer.apple.com/library/archive/qa/qa1940/_index.html

- Used `CleanDetritus` app on images
- Then ran:

```
xattr -cr "/Users/gturner/Library/Developer/Xcode/DerivedData/Dangerboard_New_Tab_Start_Page-gtrornaepscdingmukrfikpeuazz/Build/Products/Debug/Dangerboard New Tab Start Page.app"
```

