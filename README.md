# CENOS Liquid Metal Stirring Installation Guideline

## Hardware requirements for CENOS Liquid Metal Stirring:

**CPU:** Intel i5 or i7 (or similar) are good enough. Your processor should have Intel VT-x, AMD-V, or ARM Virtualization technology. This feature should be enabled in the BIOS/UEFI settings.
**GPU:** Graphics card that supports OpenGL 3.3
**RAM:** We recommend having 32 GB RAM to calculate cases, a minimum of 16 GB RAM. Actually, **the more RAM you have, the bigger (more complex) cases you can simulate.** More RAM will also help to speed up general calculation times.
**Disk Space:** 10 GB disk space is required for program installation (~7 GB third-party apps, 1 GB CENOS app). For calculation results, 10GB of disk space per case is recommended; it will differ based on your geometry and settings.

## System requirements for WSL:

To enable platform-level virtualization on Windows operating systems, you must have **Windows 10 version 2004 or higher (Build 19041 or higher) or Windows 11** and enable the Virtual Machine Platform feature.
This step can be done by going to the 'Turn Windows features on or off' section in the Control Panel and selecting the 'Virtual Machine Platform' checkbox. Please note that administrator privileges are required.
Please follow the link for additional information: https://support.microsoft.com/en-us/windows/enable-virtualization-on-windows-11-pcs.
Please pay attention that hardware virtualization could be unsupported on Windows Home edition.

## First, check if WSL is installed on your system:

- Open the Command prompt or Terminal (for Windows 11)
- Execute command: `wsl --status`. If the command is not found or returns an error message, you must install WSL.

## Windows Subsystem for Linux (WSL) installation:

- Open Task Manager and check if CPU virtualization is enabled. If it is not enabled, restart your computer and go into BIOS. Under Advanced Settings, search for the CPU virtualization option and enable it.
- Enable Windows Subsystem for Linux (not required for Windows 11) and Virtual Machine Platform under Control Panel → Programs → Programs and Features → Turn Windows features on or off or Settings → System → Optional Features → More Windows features. Restart your PC to apply the changes.

## Installation on Windows 10:

\*Open the Command prompt with Administrator rights and execute the command: - `wsl --install`

\*Update WSL to enable the latest features: - Execute the command: `wsl --update`

\*Set WSL default version to 2: - Execute the command: `wsl --set-default-version 2`

\*Finally, check if the installation was successful and if WSL is configured correctly: - Execute the command: `wsl --help` - Check if `--import-in-place` is present in the argument list.

\*Restart your PC to apply WSL.

## Installation on Windows 11:

\*Open the Terminal with Admin rights and execute the command: - `wsl --install --no-distribution`

\*Update WSL to enable the latest features: - Execute the command: `wsl --update`

\*Set WSL default version to 2: - Execute the command: `wsl --set-default-version 2`

\*Finally, check if the installation was successful and if WSL is configured correctly: - Execute the command: `wsl --help` - Check if `--import-in-place` is present in the argument list.

\*Restart your PC to apply WSL.
See official Microsoft WSL documentation for additional info: https://learn.microsoft.com/en-us/windows/wsl/

## CENOS Liquid Metal Stirring installation (LMS):

Please check that you have a stable internet connection before installing LMS.

    * Download and install the CENOS Liquid Metal Stirring software.
    * Launch the LMS.
    * Fill in the license key.
    * Agree to licenses of third-party software.
    * Click on the “DOWNLOAD AND INSTALL” button.
    * Please wait until third-party software is installed on your system (installation will take approximately 20 min)
    * LMS will be reinitialized when the installation has finished.
    * If you face issues installing third-party software, please try it manually or contact support.
