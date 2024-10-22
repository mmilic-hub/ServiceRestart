# Windows Services restart Script

This batch script automates several tasks related to the restart of the service, the script was created as a workaround, when the remote server filed to getback online beacuse remote control service wasn't starting after a scheduled server reboot.


## Features

- **Checks if the service is running before attempting to stop it.
- **Restarts the service only if necessary.
- **Logs all operations (start, stop, success, and failure) to a specified log file.
- **Designed to work on Windows systems with minimal dependencies.

## Requirements
- **Windows OS.**
- **The service name must be correctly specified.**
- **Sufficient privileges to start/stop services on the system.**
## How to Use

- **Download**
- **Modify the Script:**
- **Open the restart_service.bat file in a text editor.**
- **Replace "ServiceName" with the actual name of the service you want to restart.**
- **To run the script manually, double-click on the restart_service.bat file.**
- ** Script can be used with task scheduler**
- **Schedule the Script on Startup, If you'd like the script to run automatically on system startup:**
- **Open Task Scheduler on your Windows machine.**
- **Create a new task and set the trigger to At startup.**
- **In the action settings, point to the restart_service.bat file.**
 ## Example Log Output
 - **If the service has been stopped.**
 CHEKING THE STATUS OF THE SERVICE "XboxGipSvc" 

Tue 10/22/2024 18:33:02.46 - The service "XboxGipSvc" is not running. No need to stop it. 

Tue 10/22/2024 18:33:02.47 STARTING THE SERVICE "XboxGipSvc" 

The Xbox Accessory Management Service service is starting.

The Xbox Accessory Management Service service was started successfully.

Tue 10/22/2024 18:33:05.20 - Service restart completed.

- **If the service is running**
  
CHEKING THE STATUS OF THE SERVICE "XboxGipSvc"

18:30:46.18 Tue 10/22/2024 THE SERVICE "XboxGipSvc" is running Attempting to stop it

The Xbox Accessory Management Service service is stopping.

The Xbox Accessory Management Service service was stopped successfully.

Tue 10/22/2024 18:30:49.30 STARTING THE SERVICE "XboxGipSvc" 

The Xbox Accessory Management Service service is starting.

The Xbox Accessory Management Service service was started successfully.*

Tue 10/22/2024 18:30:51.37 - Service restart completed.


