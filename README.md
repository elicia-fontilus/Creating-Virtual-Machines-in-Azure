
<p align="center">
  
 ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/8c3f0153-8cc8-4ffb-97cf-774df272896c)

</p>

<h1>Create Virtual Machines within Azure</h1>
This tutorial outlines how to create virtual machines in Azure for beginners.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (22H2)

<h2>High-Level Steps</h2>

- Step 1: Go to https://portal.azure.com - Login or create a new account 
- Step 2: Create a Resource Group
- Step 3: Create a Windows 10 Virtual Machine (VM)
  -  While creating the VM, select the previously created Resource Group
  -  While creating the VM, allow it to create a new Virtual Network (Vnet) and Subnet
- Step 4: Use Remote Desktop to connect to your Windows 10 VM
 

<h2>Deployment and Configuration Steps</h2>

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/c05b416f-7900-4a22-a853-83392fb83795)

</p>
<p>
First, login into Azure Portal https://portal.azure.com and this is what your home/dashboard should look like or very similar to.
</p>
<br />

![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/c5294156-d4a7-47d6-b02b-905414d95f91)

<p>
</p>
<p>
Next, to create a resource group you'll want to search for it in the search box at the top. 
</p>
<br />

![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/dcc9ec07-dd1a-4d0e-b7f7-6b35688fcaf1)
 Select "Create Resource Group" to start.

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/9427b15c-d8f5-432c-8719-0f5fb1976d4b)

</p>
<p>
I named my resource group "RG-Lab" and chose the region that was closest to me, you can name and choose whichever region you would like, select "Review + create" (bottom left)
</p>
<br />

![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/f206ecc3-0013-466a-b8ee-88d7099a5b0a)
Once your resource group is created you'll get a notification as the one shown, so now time to now create the VM.
<p>

  
  
![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/2927c9d7-84b0-4282-88b0-e613823480af)
</p>
<p>
Now in the search bar type in "virtual" virtual machines should pop up as the first option select VM. We'll now start the actual process of setting up the VM similar to how we set up the Resource group just a little more steps.</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/1914619f-d1a2-490e-a419-8d17c20ad67b)
</p>
<p>
Create a basic VM hosted by Azure, so select the first option. </p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/9f0c81af-b46f-4383-9cbc-a0bea535cdd3)
</p>
<p>
Now, you will want to fill out everything that has a red "*" next to the box because it's most likey important for the VM to be successfully created
  
Select the previously created Resource Group in the drop down menu mine was "RG-Lab". Name your VM to whatever you want, My VM name is cclab3</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/6d149534-aff9-4591-8eb4-00f8b6693413)
</p>
<p>
You will want to ensure that your VM is in the same region as your resource group you created earlier. 
  For image select Windows 10 Pro. </p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/dbbba545-df5e-4735-ba7f-977f6315de7d)
</p>
<p>
For size choose "Standard_D4s_v3 - 4 vcpus, 16 GiB memory" (has 4 virtual CPUs and 16 GiB RAM). Create a username and password which will be used later on to login remotely. Leave everything else to it's default settings. 
</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/9042ffe9-6f77-4399-8b90-40d1a50c9474)
</p>
<p>
Lastly, make sure this box is checked at the very end of the page, continue on to next:disks. Leave everything on the disks tab to it's default settings and continue on to the networking tab.  </p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/90b7d9d2-796e-4d9f-bad2-54168f34210c)
</p>
<p>
Here in the Networking tab we see that the VM is creating a new Virtual Network (Vnet) and Subnet. Let's leave all the other default settings as is and click "Review + create" (bottom left)
 </p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/d3cfd206-7c3d-4cab-bc89-fdf1ca4f8a8f)
</p>
<p>
After the VM is created you should be able to see the overview. We will need the Public IP Address in order to login into the VM from "Remote Desktop Connection". The Public IP Address can be found in the top right of this overview page. You can copy it. 
</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/1ccf55f3-952c-4857-bc59-e6efaa1e61e4)
</p>
<p>
Open the "Remote Desktop Connection", paste your VM public IP Address and click "Connect"
</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/3d14bd53-17cf-4b25-8a77-e195c4adaeda)
</p>
<p>
The username and password you created earlier while setting up your VM is your credentials to login.
</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/86089fcc-b076-43a8-9e4c-dfaa2eee07d1)
</p>
<p>
Click "Yes"
</p>
<br />

<p>

  ![image](https://github.com/elicia-fontilus/Creating-Virtual-Machines-in-Azure/assets/149262013/33a7844e-ea16-48ba-ba9f-a1c68083dea0)
</p>
<p>
You are now in the VM that you created! Just to ensure, you can open command line and type "whoami" the username you created earlier should be what the response is.
</p>
<br />

