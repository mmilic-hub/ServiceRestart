# Windows Services restart Script

This batch script automates several tasks related to the restart of the service, the script was created as a workaround, when the remote server filed to getback online beacuse remote control service wasn't starting after a scheduled server reboot.


## Features

- **Pinpad Connection Check**: Scans specific COM ports to verify if a pinpad is connected.
- **File Existence Check**: Ensures required files (e.g., configuration files, marker files) are present in the working directory.
- **Firmware Handling**: Checks for firmware files and renames them for easy pinpad reload.
- **Journal Logs**: Searches for specific log files and pinpad serial numbers in the logs.
- **Service Management**: Stops the Payment Service and restarts it after performing all checks.
