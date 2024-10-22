# Windows Services restart Script

This batch script automates several tasks related to the restart of the service, the script was created as a workaround, when the remote server filed to getback online beacuse remote control service wasn't starting after a scheduled server reboot.


## Features

Features
Checks if the service is running before attempting to stop it.
Restarts the service only if necessary.
Logs all operations (start, stop, success, and failure) to a specified log file.
Designed to work on Windows systems with minimal dependencies.

Requirements
Windows OS (Batch scripts are native to Windows).
The service name must be correctly specified.
Sufficient privileges to start/stop services on the system.
