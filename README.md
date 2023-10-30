## Start, Stop, Restart, Console (SSRC)
A script with useful functions to manage VMs in VMWare vCenter

### This script requires the VMware.PowerCLI module to be installed.

To install the module, run the following command in PowerShell:

``Install-Module -Name VMware.PowerCLI -AllowClobber -Force``

## Usage

**You may need to change the execution policy to run the script. To do this you have a few options:**

### Change the Execution Policy Temporarily

You can change the execution policy for the current PowerShell session only, without affecting the system-wide execution policy:

``Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass``

### Change the Execution Policy Permanently

You can change the execution policy permanently for all PowerShell sessions. Open a PowerShell window with “Run as Administrator” option and run:

``Set-ExecutionPolicy RemoteSigned``

This will allow running unsigned scripts that you write on your local computer and signed scripts from the Internet. Please note that this changes the policy permanently. If you want to change it back to the default, run:

``Set-ExecutionPolicy Restricted``

### Bypass Execution Policy at Run-time

You can also bypass the execution policy at run-time with this command:

``powershell.exe -ExecutionPolicy Bypass -File "C:\FILE\LOCATION\vm-ssrc.ps1"``

### Run the script

``C:\FILE\LOCATION\vm-ssrc.ps1``
