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

## Features

|Function|Description|
|---|---|
|Create VM|Creates a VM by entering the name, selecting the host, datastore, network, OS, RAM, CPU, and disk size.|
|Start VM|Starts a VM selected from a list of VMs by number.|
|Stop VM|Stops a VM selected from a list of VMs by number.|
|Restart VM|Restarts a VM selected from a list of VMs by number.|
|Open VM Console|Opens the console of a VM selected from a list of VMs by number.|
|Get IP Address of VM|Gets the IP address of a VM selected from a list of VMs by number.|
|Get VM Info|Gets the raw VM info of a VM selected from a list of VMs by number.|
|VMware Tools|Submenu to install, update, or dismount VMware Tools on a VM selected from a list of VMs by number.|
|Get VM List|Outputs a list of VMs in the vCenter and their power state color coded. Green = Powered On, Red = Powered Off, Yellow = Suspended.|
|Delete VM|Deletes a VM selected from a list of VMs by number.|

## Changelog

See latest changes [here](https://github.com/Harmless05/vmware/releases/).

## License

This project is licensed under the Mozilla Public License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

* [VMware.PowerCLI](https://www.powershellgallery.com/packages/VMware.PowerCLI/12.0.0.15947286)
* [VMware.PowerCLI Documentation](https://code.vmware.com/web/dp/tool/vmware-powercli/12.0.0)
* [VMware.PowerCLI Cmdlet Reference](https://developer.vmware.com/docs/powercli/latest/products/)