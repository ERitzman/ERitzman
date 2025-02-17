# Lesson 3: iOS and iPadOS File Storage Structure
## Goal
Understand iOS and iPadOS file storage structure and how data is stored, organized, and secured.
## Video
https://youtu.be/TmSH7NJRUQE

[![Watch the video](https://i.ytimg.com/vi_webp/TmSH7NJRUQE/sddefault.webp)](https://youtu.be/TmSH7NJRUQE)

## Key Points
- The iOS and iPadOS file system contains two volumes.
  - The system volume contains the operating system and only system data can be written to this location.
  - The data volume contains user data. Information stored on the data volume is encrypted only when the device is protected with a passcode.
- Using Shared iPad divides the data differently on an device, allowing multiple users to sign in to the same device by creating separate data volumes.
- Apps exist within an app sandbox to prevent them from accessing or modifying the contents of other apps without permission from the user.
- Information created and stored by an app during use is called app data.
  - App data might include the high score of a game or the contents of a document.
  - Some apps back up data to iCloud or another server.
  - Local app data is removed when an app is deleted. However, data may still exist in iCloud or a third-party server.
## Review
<details>
   <Summary> 1 How many volumes are there in the iOS and iPadOS file system by default?</Summary>
   iOS and iPadOS contain two volumes: a system volume and a data volume.
 </details>
 <details>
   <Summary> 2 If an iOS app is deleted, does the data remain on the device?</Summary>
   Deleting an iOS app will remove all local data associated with that app, including preferences.
 </details>
 <details>
   <Summary> 3 Are apps allowed to access data from other apps without permission?</Summary>
   Without explicit permission from the user, apps are sandboxed and may not access data from other apps or affect the system.
 </details>

 ## Resources
<em>Jamf Pro Documentation - [Apple Education Support Settings](https://learn.jamf.com/en-US/bundle/jamf-pro-documentation-current/page/Apple_Education_Support_Settings.html)</em></br>
Apple - [Role of Apple File System](https://support.apple.com/guide/security/role-of-apple-file-system-seca6147599e/1/web/1)</br>
Apple - [App security overview](https://support.apple.com/guide/security/app-security-overview-sec35dd877d0/1/web/1)</br>
Apple - [iCloud security overview](https://support.apple.com/guide/security/icloud-security-overview-secacde2d0da/1/web/1)</br>
Apple - [Shared iPad overview](https://support.apple.com/guide/deployment/shared-ipad-overview-dep9a34c2ba2/web)</br>
