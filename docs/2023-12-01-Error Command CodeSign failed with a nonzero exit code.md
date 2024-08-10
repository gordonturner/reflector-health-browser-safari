# 2023-12-01-Error Command CodeSign failed with a nonzero exit code

## Description
Got the following issue when trying to run on MacOS:
```
Command CodeSign failed with a nonzero exit code
```

- Found:
https://developer.apple.com/library/archive/qa/qa1940/_index.html

- Used `CleanDetritus` app from root of project
https://apps.apple.com/us/app/cleandetritus/id1161108431?mt=12

- Then ran:
```
xattr -cr "/Users/gturner/Library/Developer/Xcode/DerivedData/Reflector_Health-ezfsbmighkfctzbbfqnvkjyclcar/Build/Products/Debug/Reflector Health.app"
```

```
xattr -cr "/Users/gturner/Library/Developer/Xcode/DerivedData/Dangerboard_New_Tab_Start_Page-gtrornaepscdingmukrfikpeuazz/Build/Products/Debug/Dangerboard New Tab Start Page.app"
```