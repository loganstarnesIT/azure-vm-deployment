<p align="center">
<img src="https://images.icon-icons.com/2699/PNG/512/microsoft_azure_logo_icon_168977.png" width="60%" alt="active directory logo"/>
</p>

<h1>Microsoft Azure - Deploying a Virtual Machine and Virtual Network</h1>
This tutorial outlines the general deployment of an Azure Virtual Machine & Virtual Network.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure 
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 11 Pro x64 24H2 </b> 

<h2>List of Prerequisites</h2>

- A Microsoft Azure account
- Internet Connection

<h2>Deployment Steps</h2>
Note: You can click images to enlarge them if they are too small to view
<p>

<h3> Creating a Resource Group </h3>
<p float="left">
  <img align="center" src="https://i.imgur.com/7YHE2C7.png" width="49%" />
  <img align="center" src="https://i.imgur.com/1i8YIrU.png" width="49%" />
</p>
<p>
1. Before we begin creating and deploying our Virtual Machine and VNet, it's important to know how to create an independent "Resource Group". 
A "Resource Group" enables you to group the services you wish to use and deploy for easier management.

  When you arrive at the Azure landing screen on sign-in, select the search bar at the top of the page and search for 
"Resource Group". You'll select it from the dropdown menu that appears and, on the next page, click "➕ Create" in the [TOP LEFT]. Set the name of the resource group, 
using hyphens in between words, then "Review + Create" and create the group.
</p>
<br />

<h3> Configuring our Virtual Machine </h3>
<p float="left">
  <img align="center" src="https://i.imgur.com/yP4Iwiz.png" width="29%" />
  <img align="center" src="https://i.imgur.com/FHKFyEy.png" width="19%" />
  <img align="center" src="https://i.imgur.com/uB7u8we.png" width="49%" />
  <img align="center" src="https://i.imgur.com/sAAx4hv.png" width="39%" />
</p>
<p>
2. Now that we have a group ready, we can start to add a virtual machine to the group and configure its settings. Navigate to your list of Resource Groups and select the one you created to open a new
window pane on the right. Similarly to how the group was created, select the "➕ Create" in the Top Left of the new pane that just opened and it will open the Azure Marketplace. 

Don't be intimidated all of the options, as we're only here to use the search bar on the top left to look for "Virtual Machine".

  Once you type it in the bar, press enter. Now you should have an option that looks like what's shown in Image 2; It should be the first option. 
If it looks correct, select "Create" and click "Virtual machine". You will be met with the settings for the Virtual Machine, and it should look similar to the settings in Image 3. 

Of particular note, ensure that the "OS Image" is compatible with the "Zone" you have selected. If you receive an error about the zone of the VM 
and the Image not working properly, change the "Zone" from "Zone 1" to "Zone 2" by only having Zone 2 enabled in the dropdown.

  Ensure that the "Size" of the system is sufficient. For basic usage, it is typically recommended "2 Vcpus" & "8 GiB Memory" to run smoothly. Set the "Administrator account" details (write the login credentials down or remember them
for later if you wish to remote connect to the VM) and make sure to check the "Licensing" box as shown in Image 4. After you have completed that, we'll move to the next step.
</p>
<br />

<h3> The Network Tab - Virtual Network Settings </h3>
<p float="left">
  <img align="center" src="https://i.imgur.com/RWnqh5W.png" width="39%" />
  <img align="center" src="https://i.imgur.com/rayJ0VE.png" width="29%" />
<p>
  <img align="center" src="https://i.imgur.com/55kPq2O.png" width="49%" />
</p>
<p>
3. For this section, we'll move from the "Basics" tab at the top of the configuration screen to the "Networking" tab. There isn't much to change here for the time being, however it is important to know some details you are 
able to change within this menu. For instance, if you were to select the "Edit virtual network" option below the selected Vnet, you can edit the name and subnet for it. 

When you have finished looking around the Networking tab, you can click "Review + Create" and once all of the checks pass, you can deploy both the VM and Vnet.

It will take some time for the systems to be fully deployed. Afterwards, you can head over to the landing page of Azure and see the list of recent resources you've created.

<h2> Congrats, you've officially deployed a Virtual Machine and a Virtual Network! </h2>
</p>
<p>
<br />
