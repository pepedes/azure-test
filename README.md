# azure-test
Deployment of Red Hat Enterprise Linux VM (RHEL 7.2 or RHEL 6.7)
<a href="https://github.com/pepedes/azure-test/blob/master/azuredeploy.json" target="_blank"> <img src="http://azuredeploy.net/deploybutton.png"/> </a> <a href="https://github.com/pepedes/azure-test" target="_blank"></a>

This template allows deploying a Red Hat Enterprise Linux VM (RHEL 7.2 or RHEL 6.7), using the latest image for the selected RHEL version. This will deploy a Standard D1 VM in the location of your chosen resource group with an additional 100 GiB data disk attached to the VM.

Independently form this template you can deploy a blank RHEL VM using the following Azure CLI commands (adjust parameters as needed):

azure config mode arm
azure group create TestCLIRG EastUS
azure vm quick-create TestCLIRG vm1 EastUS Linux RedHat:RHEL:7.2:latest azureuser
Note: this template and the above commands use RHEL Pay-As-You-Go VM image which carries an additional charge in addition to the base Linux VM price. Check out RHEL VM pricing for more details.
