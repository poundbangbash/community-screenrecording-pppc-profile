# Community PPPC ScreenRecording Profile
This is a management profile for MDM of all the currently known apps that use ScreenRecording on macOS.
On macOS 11, without an MDM payload, ScreenRecording Privacy rights are only interactable by users with admin rights. For establishments that have non-admin user populations, this MDM payload can be delivered to allow the user to allow the application to "record" the screen.

To contribute to the list:
1) Verify the application is not already in the list.  Each `<dict>` block has a `<Comment>` key specifiying the name of the app..
2) Run `codesign -dr - /path/to/app` to get the codesign designation.
3) Update the new file with the pertinent information and submit a PR.
