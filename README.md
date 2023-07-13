# Creating-Virtual-Machines-to-block-traffic
<p align="center">

![images](https://github.com/Admiller12/Creating-Virtual-Machines-to-block-traffic/assets/138805066/35091daf-99a2-4124-86e1-1c9a8fba7ceb)



Project consists of creating a resource group for two virtual machines: one windows and one linux. The utility allows you to remotely connect to a desktop in the first virtual machine and installwireshark in the second virtual machine that will ping and observe traffic. In the second virtual macinenes network security group traffic will be blocked and stopped.




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Wireshark  

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Linux
- Powershell


<h2>Walk Through/Demonstration Steps</h2>

<p>

![Capture](https://github.com/Admiller12/Creating-Virtual-Machines-to-block-traffic/assets/138805066/0b1be1ae-7441-4874-83c2-346b4cc1f528)

</p>
<p>
In this demonstration a resource group and two virtual machines was created through Microsoft Azure. First step logged into Azure.com under account information. Created the main resource group (RGProject) reviewed and created. 
Next created the firt virtual machine under the Resource group (RGProject) created a virtual machine name (VMProjectW) selected
the region in which vm was made also created a in windows 10. Last created the usernae and password. Reviewed and created the first VM.
Follwed this step to create the second the second VM and it was created under linux (VMProjectL). 
</p>
<br />

<p>

  ![Capture2](https://github.com/Admiller12/Creating-Virtual-Machines-to-block-traffic/assets/138805066/b13978e6-cadf-4740-93f2-29db60c9655d)

</p>
<p>
In this demonstartion The virtual machine was connected through remote desktop.
First clicked on the Windows VM and copied the IP Address. Next clicked the start menu
to search the remote desktop. After, paste the IP address in the remote desktop 
search to connect remotely (connect with username and password). Then, in the remote desktop google search Wireshark was downloaded
and installed.
</p>
<br />

<p>

  ![Capture3](https://github.com/Admiller12/Creating-Virtual-Machines-to-block-traffic/assets/138805066/e205611d-be0e-48f0-904b-98d044c25999)

</p>
<p>
In this demonstartion the navigation is all remotely done through wireshark. First we connect 
to the ethernet this step is to start capturing live packets. Now observing all the live traffic
that is happening in the VM. After we filter the traffic by the ICMP (internet Control Message Protocol) to essentially stop movement.
</p>
<br />

<p>

  ![Capture4](https://github.com/Admiller12/Creating-Virtual-Machines-to-block-traffic/assets/138805066/8a534c0f-1139-4e60-8412-39882badd5ce)

</p>
<p>
In this demonstartion the connection are being made through virtual machine linux. Navagating back to Azure 
to the second VM that was created to essentially ping the Private IP address. Next opened up Poweshell typed in "ping 10.0.0.5" 
which is the second VM private IP address. Now we can see it pinging and replying from the second VM. 
</p>
<br />
