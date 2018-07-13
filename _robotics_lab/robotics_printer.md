---
title: Robotics Lab Printer
layout: page_with_toc
---

Students and Employees who work in the Robotics Lab can make use of the Robotics Lab printer. Intallation instructions can be found [here](/tutorials/printer).

# Ubuntu
1. Make sure the printer is turned on and not in error mode!
2. Open a terminal and type
    ```
    system-config-printer
    ```
3. Add
4. Network Printer
    ```
    LPD / LPR Host or Printer
    Host: wbmtprint.wtb.tue.nl
    Queue: Robotics01
    Forward
    Provide this PPD file
    Name: Robotics01
    Description: Robotics01
    Location: Robotics Lab
    ```

# Windows 7/8
1. Make sure the printer is turned on and not in error mode!
2. Open Control Panel
3. Go to Devices and Printers
4. Select a Shared Printer by name:
    ```
    Adress: \\wbmtprint\Robotics01
    IP: 131.155.66.17
    ```
5. The process should finish by itself, including driver installation

# Windows 10
1. Make sure the printer is turned on and not in error mode!
2. Go to `Start` and type `Run`
3. Type: 
    ```
    \\wbmtprint\Robotics01
    ```
4. Log in with your TUe account
5. Install the driver
6. The process should finish by itself