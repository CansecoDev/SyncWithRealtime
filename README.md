**ID: 2180376655** | Synchronizes game time with real time  
**Version : 1.0.0**

Sync With Realtime is a mod for Conan Exiles that synchronizes game time with real time. Now you can have the immersion feel of playing late night while is dark.

Works in singleplayer/co-op and dedicated servers.

# About Sync With Realtime
This mod will keep your game time in sync with real time, no matter how long your game or server has been shut down, it will catch up with real time as soon as it starts and keep it synchronized.

# Usage
By default, it will sync with **UTC+0**, but as admin/rcon you can use this command to set your time zone:  

``
DataCmd SyncTimeOffset {zone}
``

Example usage:
- Server time is 03:15, but you are at 22:15, this means you are on UTC-5:  
``
DataCmd SyncTimeOffset -5
``

For a more in deep understanding of this command, please see [this documentation](https://github.com/srcanseco/SyncWithRealtime/blob/master/Documentation/Commands.md).


# Milestones/Features
**[✅]** Implemented real time to game time synchronization  
**[✅]** SyncTimeOffset command, see documentation for usage  
**[❌]** More commands for finetuning  

[Changelog](https://steamcommunity.com/sharedfiles/filedetails/changelog/2180376655)

# Known bugs
- None so far.
