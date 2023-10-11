# Community PPPC ScreenRecording Profile
This is structured data of a management profile for MDM of community-provided apps that are known to use ScreenRecording on macOS.

**NOTE: This payload is not intended to be used as is. The intent is to provide you, the admin, structured data to pick and choose which titles you want to allow non-admin users to approve ScreenSharing rights to.**

On macOS 11 or newer, without an MDM payload, ScreenRecording Privacy rights are only interactable by users with admin rights. For establishments that have non-admin user populations, this MDM payload data can be delivered to allow the non-admin user to allow the application to "record" the screen.

To contribute to the list:
1) Verify the application is not already in the list.  Each `<dict>` block has a `<Comment>` key specifiying the name of the app..
2) Run `codesign -dr - /path/to/app` to get the codesign designation.
3) Update your fork of the file with the pertinent information and submit a PR.
