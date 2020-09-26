# Technolog_MNE

![Technolog Logo](/Media/Technolog_Logo.jpg)

Technolog MNE is part of an in-house solution to a Bitlocker management solution.

## Synopsis

Once the PowerShell script is ran the user will be presented with the below form, in which they have to enter their desired password. It is advised **against** the use of special characters as the Bitlocker pre-boot environment uses a US keyboard layout. As such special characters won't line up 100% of the time.

![MNE GUI](/Samples/MNE_GUI.PNG)

Upon successfully entering a password that meets the complexity requirements the encryption process will begin. A recovery password will be generate, which can be backed up into active directory. If you're connect to the corporate network when the script is ran, this is done automatically.

## Latest Release

- v1.1
    * Complexity requirements changed to require 15 characters (previously 8)
    * Note added to not include special characters (@,#,!,$,&,etc)
    * Recovery key is now backed up to active directory after the encryption process begins

For a full list of releases please check the [Change Log](CHANGES.md)

## Notifications

#### Encryption of system volume has started

![Start Notification](/Samples/Start_Notification.PNG)

#### Encryption of system volume has completed

![End Notifiction](/Samples/End_Notification.PNG)

#### An error occured whilst trying to begin the encryption process

![Error Notification](/Samples/Error_Notification.PNG)

#### Passwords do not match

![Mismatch Error](/Samples/Mismatch_Error.PNG)

#### Password does not meet the required complexity

![Complexity Error](/Samples/Complexity_Error.PNG)