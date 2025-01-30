# Device Model and OS History
Our SQL queries for an indept review of all Apple devices and their OS version timeframes parsed from the Health Application. 

Reviewing all devices used by an Apple ID, their OS versions, and the timeframes of the OS versions could prove extremely valuable within an investigation. It is our hope these SQL queries aid in the accurate parsing and analysis of Apple devices and OS versions.

# Where to Use:

- The SQL queries will work in most SQLite database viewers able to execute SQL queries. 
- The ConnectedDeviceHistory.xml file is a Magnet AXIOM Custom Artifact, which can be added to Magnet AXIOM Process through Tools > Manage custom artifacts > ADD NEW CUSTOM ARTIFACT. Once added, the artifacts are named Connected Device History and OS Version, Consolidated Connected Device History, and Current Device Information.
- As always, we remain a proud support of the LEAPPS project, and this will be submitted to iLEAPP as well. 

# Artifact Examples:
Device and OS Timeframe:

![Device and OS Timeframe Example](https://github.com/user-attachments/assets/346cb83c-b3fe-4d8d-bbbe-3646d74a362e)

The device ID is changed to the common name using a Case Statement, the device ID is provided, source ID assists in verifying same devices (though the same device could have multiple source ID values), the OS version is obtained, and the timeframe of the OS version is presented with start and end timestamps. 

Device Isolation:

![Device Isolation Example](https://github.com/user-attachments/assets/b5b81c28-9064-452d-a0a8-1d5382bd9d96)

Here, the same data is viewed differently. Each device ID is broken up into overall start and end timestamps for device usage. (Note, potentially if the user obtained a replacement device which was the same model the change would not be reflected here.)

Current Model and OS:

![Current Model and OS Example](https://github.com/user-attachments/assets/baa5b5ae-ac97-4ac8-93ae-adcde10759c2)

For iOS 18 and newer, this data is parsed from the healthdb.sqlite database. The current devices (Apple iPhone, Apple Watch, and/or Apple iPad) are listed with their current OS version. 

# File Location
This data pertains to Apple devices recorded within the healthdb_secure.sqlite and healthdb.sqlite databases, available through encrypted Advanced Logical and Full File System Extractions.

# iOS Support
Our Device and OS Timeframe and Device Isolation queries support iOS 15, 16, 17, and 18. Current Model and OS only supports iOS 18.

# More Details
Additional details published within 'Beyond the Logs: Using the Health App to Uncover Device Model and OS History' at [URL](https://metadataperspective.com/2025/01/30/beyond-the-logs-using-the-health-app-to-uncover-device-model-and-os-history/).
