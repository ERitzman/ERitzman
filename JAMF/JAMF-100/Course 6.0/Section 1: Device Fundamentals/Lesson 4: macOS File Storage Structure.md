# Lesson 4: macOS File Storage Structure
## Goal
Understand macOS file storage structure and how data is stored, organized, and secured.
## Video
https://youtu.be/m6ul68AEDdw

[![Watch the video](https://i.ytimg.com/vi_webp/m6ul68AEDdw/sddefault.webp)](https://youtu.be/m6ul68AEDdw)
## Key Points
- By default, a macOS storage disk consists of one Apple File System (APFS) container.
  - Each container may have multiple volumes.
  - The default APFS container consists of five volumes.
- The system volume contains:
  - All necessary files to start up the Mac
  - All apps installed automatically by macOS
- The data volume contains:
  - Information found in the user's folder, including photos and documents
  - Applications installed by the user
  - Custom frameworks installed by the user or organization
- System Integrity Protection (SIP) is a security technology designed to protect critical files that are essential for the operating system to function.
  - The System directory is protected by SIP.
  - All apps pre-installed with the operating system, like System Settings and Console, are also protected.
  - Only processes signed by Apple, like Apple software updates and Apple installers, are allowed to modify these protected areas.
- Disk Utility is an app for viewing and modifying volumes on connected disks.
- Four root directories—Applications, Library, System, and Users—are separated based on how they are used.
  - The Applications and Library directories contain apps and preferences shared by all users.
  - The System directory contains system software installed by Apple in the System directory.
  - The Users directory contains files and preferences specific to each user.
    - Each user only has access to their own directory, with the exception of the Shared directory, which all users have access to.
## Review
<details>
   <Summary> 1 User files (documents, photos, and applications) are stored in which volume?</Summary>
   Documents, photos, and other user-specific files are stored in the data volume.
 </details>
 <details>
   <Summary> 2 Which technology prevents users from modifying the System directory?</Summary>
   Sensitive directories like the System directory are protected by System Integrity Protection (SIP).
 </details>

## Practice
 1. Identify how the storage space is being used on a test computer.
    - Navigate to Applications > Utilities and open the Disk Utility app. How many volumes are there on the computer?
    - In the sidebar, select Macintosh HD > Data. How much storage space is currently used by the data volume?

 2. Explore the default directories on macOS.
    - From the Desktop menu bar, select Go > Computer and then select the Macintosh HD directory.
    - Select the System directory. What apps are part of the System directory?
    - Select the Users directory. Are there other users on this test computer? If so, can you access the contents of these folders while logged in as the current user?

## Resources
Apple - [Role of Apple File System](https://support.apple.com/guide/security/role-of-apple-file-system-seca6147599e/1/web/1)</br>
Apple - [About System Integrity Protection on your Mac](https://support.apple.com/102149)</br>
Apple - [Intro to Disk Utility on Mac](https://support.apple.com/guide/disk-utility/intro-to-disk-utility-dskutl1029/mac)</br>
