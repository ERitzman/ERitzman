# Interview questions for JAMF & macOS Support

**How would you design a Jamf solution to manage a large number of Macs in an enterprise environment?**
 - create a comprehensive inventory of all Macs in the environment
    - model
    - serial number
    - operating system version
    - hardware specifications
 - create a comprehensive set of policies and procedures for managing the Macs
    - patching
    - software installation and removal
    - security settings
    - user access
 - create a system for deploying software and updates to the Macs
    - can be done using Jamf's software distribution tools (ie: JAMF Pro)
 - create a system for monitoring the Macs
    - can be done using Jamf's software distribution tools (ie: JAMF Pro)
       - status
 	  - identify any potential issues or vulnerabilities
 	  - remotely manage the Macs
___
**Describe the process of creating a Jamf package and deploying it to a fleet of Macs.**
 - create the package
    - using the Jamf Pro Package Builder
       - create packages from a variety of sources
 	     - disk images
 		 - applications
 		 - scripts
 		 - more...
 - create a policy in Jamf Pro to deploy the package
    - policy should include
       - package
 	  - any other settings or configurations
 	  - (opt) scope of the policy, such as which computers or users it should apply to
    - Once the policy is created, you can deploy it to the fleet of Macs. This can be done manually, or you can use Jamf Pro's automated deployment features to deploy the policy to the Macs on a schedule. 
 - monitor the deployment of the package to ensure that it is successful. Jamf Pro provides detailed reporting and analytics to help you track the deployment of the package and any other policies you have deployed
___
**What challenges have you faced when developing Jamf solutions?**
 - One of the biggest challenges faced when developing Jamf solutions is ensuring that the solutions are secure and compliant with industry standards.
    - requires a deep understanding of the security protocols and best practices that are in place for Jamf
    - requires a a thorough understanding of the specific requirements of the customer
    - ensure that the solutions are scalable and can handle the customer's needs as they grow
 - Another challenge faced is ensuring that the solutions are user-friendly and intuitive.
    - requires a deep understanding of the user experience and how to design solutions that are easy to use and understand.
    - ensure that the solutions are compatible with the customer's existing infrastructure and can integrate seamlessly with their existing systems.
 - Finally, I have to ensure that the solutions are cost-effective and can be implemented within the customer's budget.
    - requires a deep understanding of the customer's needs and budget
    - requires an understanding of the cost of the various components of the solution
    - ensure that the solutions are optimized for performance and can handle the customer's workloads.
___
**How do you troubleshoot Jamf issues?**
 - identify the source of the issue
    - can be done by gathering information from the user
       - what they were doing when the issue occurred
 	  - what type of device they are using
 	  - any error messages they may have received
    - review the Jamf logs to see if any errors are present
       - If errors are present, they should be analyzed to determine the cause of the issue
 - review the Jamf configuration
    - ensure that all settings are correct
    - ensure that the Jamf server is properly configured
       - network settings
 	  - Jamf database
 	  - any other settings that may be relevant
 - test the issue in a test environment
    - create a test user account and replicate the issue in the test environment
 - contact Jamf Support for assistance
___
**How do you ensure that Jamf policies are secure and compliant with industry standards?**
 - ensure that all policies are written with security in mind
    - use secure coding practices
       - input validation
 	  - encryption
 	  - authentication
    - make sure that all policies are tested for vulnerabilities and that any identified issues are addressed promptly
 - stay up to date on industry standards and best practices
    - read industry publications
    - attend conferences
    - participate in online forums
    - regularly review the Jamf documentation
 - use Jamf's built-in security features
    - use Jamf's built-in encryption
    - use Jamf's built-in authentication
    - use Jamf's built-in access control features
    - use Jamf's reporting and auditing features to monitor policy compliance and detect any potential security issues
___
**What strategies do you use to optimize Jamf performance?**
 - Utilize Jamf Pro's built-in performance tools
    - can be used to identify and address performance issues
       - Performance Analyzer
 	     - used to identify and troubleshoot performance issues
       - Performance Tuner
 	     - used to optimize Jamf Pro's performance
 - Optimize the Jamf Pro database
    - Jamf Pro database is the backbone of the system, and optimizing it can have a significant impact on performance
       - ensure that the database is properly indexed
 	  - ensure that queries are optimized
 	  - ensure that the database is regularly backed up and maintained
 - Optimize the Jamf Pro server
    - Jamf Pro server is the core of the system, and optimizing it can have a significant impact on performance
       - ensure that the server is properly configured
 	  - ensure that the server is running the latest version of Jamf Pro
 	  - ensure that the server is regularly monitored and maintained
___
**How do you use Jamf to manage user accounts and access control?**
 - Jamf can be used to create and manage user accounts
    - creating new user accounts
    - setting up user profiles
    - managing user access rights
    - set up user groups and access rights for each group
 - Jamf can be used to manage access control
    - set up authentication methods
       - passwords
 	  - biometrics
 	  - two-factor authentication
    - set up access control policies
       - require users to change their passwords periodically
 	  - restrict access to certain applications or websites
 - Jamf provides a comprehensive solution for managing user accounts and access control
    - allows administrators to easily create and manage
       - user accounts
 	  - access control policies
 	  - monitoring of user activity
___
**How do you use Jamf to manage software updates and patches?**
 - use Jamf Pro to create policies that can be used to deploy software updates and patches to managed devices
    - policies can be configured to deploy updates and patches automatically
    or
    - policies can be configured to prompt the user to install the updates and patches
 - use Jamf Pro to create Smart Groups that can be used to target specific devices for software updates and patches
    - allows easy deployment of updates and patches to specific devices, such as those running a specific version of an operating system or those in a specific location
 - use Jamf Pro to create scripts that can be used to automate the process of deploying software updates and patches
 - use Jamf Pro to create Self Service policies that can be used to allow users to install software updates and patches on their own devices
___
**What is Jamf Pro, and how does it differ from other MDM solutions?**
 - Jamf Pro is a comprehensive Mobile Device Management (MDM) solution specifically designed for Apple devices. It stands out from other MDM solutions by offering specialized features and seamless integration with Apple's ecosystem.
___
**How do you enroll devices in Jamf Pro?**
 - Devices can be enrolled manually by users or automatically through Apple's Device Enrollment Program (DEP). 
	  This ensures that devices are securely connected to Jamf Pro, allowing us to apply policies, deploy applications, and maintain compliance with organizational standards.
___
**Explain the difference between Configuration Profiles and Restriction Profiles in Jamf Pro**
 - Configuration Profiles are used for deploying settings like Wi-Fi configurations, VPN, and email accounts. 
	  On the other hand, Restriction Profiles focus on controlling access to specific device features, ensuring a secure and tailored user experience.
___
**How do you troubleshoot device enrollment issues in Jamf Pro?**
 - When troubleshooting enrollment issues, I start by checking the device's network connectivity and ensuring Apple services like Device Enrollment Program (DEP) are accessible.
	  Additionally, I review Jamf Pro logs for any error messages or inconsistencies that might hinder the enrollment process.
___
**Can you explain the concept of Smart Groups in Jamf Pro?**
 - Smart Groups are dynamic groups in Jamf Pro that automatically include devices based on specified criteria, such as OS version or installed applications. 
	  They streamline management by automating the categorization of devices and allowing for targeted policies.
___
**Explain how Configuration Profiles override settings on iOS and macOS devices.**
 - Configuration Profiles follow a hierarchy, and settings are overridden based on payload priority. 
	  The most specific payload takes precedence. For example, a user-specific profile will override a device-wide profile, ensuring granular control over settings.
___
**What's a profile? How do you manage profiles?**
 - A profile is a document with the filename extension .mobileconfig that contains system settings as defined by an administrator. When you open a profile document, macOS High Sierra installs the profile and configures the settings. You can manage installed profiles through Profiles preferences.
___
**Which terminal command should you use to perform the following?**
 - *Print working directory:* `pwd`
 - *List:* `ls`
 - *Change directory:* `cd`
 - *Indicate parent directory:* `..`
 - *Indicate current user home folder:* `~`
 - *Create a folder:* `mkdir`
 - *Run the command with root account access:* `sudo`
 - *Clear the Terminal screen:* `clear` or press Control-L
___
**Which utilities are available when you start up from macOS Recovery?**
 - Restore from Time Machine Backup
 - Install/Reinstall macOS
 - Get Help Online through Safari
 - Disk Utility
 - Startup Disk
 - Firmware Password Utility
 - Network Utility
 - Terminal
 - Reset Password
___
**What are the different macOS Recovery options and start up key combinations?**
 - *Command-R*:: Install the latest macOS that was installed
 - *Option-Command-R*:: Upgrade to the latest macOS that is compatible with your Mac.
 - *Shift-Option-Command-R*:: Install the macOS that came with your Mac.
___
**How can you create an external macOS installation disk?**
 - You can create a macOS Recovery disk that includes the macOS High Sierra tools and installation assets with the `createinstallmedia` command-line tool in macOS Installer.
___
**What are the types of local user accounts in macOS High Sierra? How are they different?**
 - *Administrator*:: Administrator user accounts are part of the admin group and are allowed full access to all apps, preferences, and shared resource locations
 - *Standard*:: Standard users are allowed to take advantage of nearly all the resources and features of a Mac, but they generally can't change things that might affect other users.
 - *Managed with parental controls*:: A managed account is a standard account with parental controls enabled.
 - *Guest*:: The default guest account is similar to a standard user, but it doesn't require a password. When a guest user logs out, the home folder is deleted, including any home folder items that would normally be saved, like preference files or web browser history.
 - *Sharing only*:: "Sharing only" accounts allow you to share files with someone on a different computer, but they can't log in to your Mac
 - *System Administrator (root)*:: The System Administrator account has unlimited access to almost everything on a Mac. It is turned off by default on macOS.
 - *Group*:: A group account is a list of user accounts that gives you greater control over file and folder access.
___
**What are account attributes?**
 - Account attributes are the individual pieces of information used to define a user account. Examples include
    - User ID
    - group
    - account name
    - full name
    - login shell
    - home directory
    - universally unique ID (UUID)
    - Apple ID
    - aliases
___
**How can you limit a user account from having full access to all apps?**
 - You can use parental controls to restrict what users can do. Examples of limitations include
    - enforcing a simple Finder
    - limiting apps
    - limiting App Store content
    - setting time limits
    - privacy settings
    - more...
___
**Which folders, by default, are contained in a user's home folder?**
 - Desktop
 - Documents
 - Downloads
 - Movies
 - Music
 - Pictures
 - Public folders
___
**What options do you have when you delete a local user account?**
 - Save the home folder in a disk image
 - Don't change the home folder
 - Delete the home folder
___
**If a macOS installation fails, where can you find out more about why it failed?**
 - Open Console
 - `cd /var/log/`
 - Open `install.log`
___
**How do you make macOS Sierra associate a new local user account with a manually migrated or restored user's home folder?**
 - Copy the restored user's home folder to the `/Users` folder
 - Open *System Preferences*
 - Click on the *Users and Groups* pane
 - Create a new local user account with the same account name that was used for the user's home folder. macOS prompts you to associate the new local user account with the restored home folder.
___
**Which types of items can you store in a keychain?**
 - Resource passwords
 - digital certificates
 - encryption keys
 - Safari AutoFill information
 - Internet Account settings
 - secure text notes
___
**How does the Keychain Access help protect your information?**
 - Keychain manages encrypted files that are used to securely save your items. By default, users have login and Local Items keychains that use the same password as their account. Not even other administrative users can access your keychain secrets unless they know the keychain password.
___
**Where are keychain files stored?**
 - Each user starts with a login keychain saved at `/Users/username/Library/Keychain/login.keychain` and a Local Items/iCloud keychain saved in the `/Users/username/Library/Keychains/UUID` folder. Administrative users can manage macOS authentication assets with the `/Library/Keychain/System.keychain`. Apple maintains several items in `/System/Library/Keychains/` for macOS use.
___
**How can you reset a user's lost account password?**
 - You can reset local account passwords
    - in Users & Groups
    - by the master password at login
    - by a FileVault recovery key at startup
    - by the Reset Password assistant in macOS Recovery.
    - Users with local accounts with an **Apple ID and password** can manage their Apple IDs and passwords at <https://appleid.apple.com> or <https://iforgot.apple.com>
___
**How does resetting a user's account password affect that user's login keychain?**
 - The account password reset process won't change any keychain passwords. Therefore, the user's keychains don't automatically open when the user logs in with a new password. The user will have to manually change the keychain passwords using the Keychain Access utility
___
 
