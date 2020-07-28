# About Commands in general

- Any Conan Exiles command have 3 possible flags you should now about:

  - ![Client](https://img.shields.io/badge/client-blue) : Runs on the client when executed
  - ![Client](https://img.shields.io/badge/server-red) : Runs on the server when executed and can be executed from a remote console
  - ![Client](https://img.shields.io/badge/admin-purple) : This command will only be available to a logged admin

- The command prefix ``DataCmd`` is required for any Conan Exiles modded command, you will need to type it before any command.

# Sync With Realtime commands
#### SyncTimeOffset ![Client](https://img.shields.io/badge/server-red) ![Client](https://img.shields.io/badge/admin-purple)

````
DataCmd SyncTimeOffset {offset}
````

This command will set a persistent time offset that can be used to establish the time zone you are in, for a more precise offset you can use a Time Float, this equation will give you the offset you require.  

<img src="https://render.githubusercontent.com/render/math?math=h%2Bm\frac1 60 %2Bs\frac1 3600">

___

Example usage A:
- Server time is 03:15, but you are at 22:15, this means you are on UTC-5:  
````
DataCmd SyncTimeOffset -5
````

___

Example usage B (advanced):
- You want to set a positive offset of 6 hours 45 minutes and 50 seconds:  
- By the previous equation:

<img src="https://render.githubusercontent.com/render/math?math=6%2B45\frac1 60 %2B50\frac1 3600 = 6.76388888\dot{8}">

````
DataCmd SyncTimeOffset 6.7638888888888
````
