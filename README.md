<p align="center">
<img src="https://i.imgur.com/Wy1FSRk.png" alt="img"/>
</p>

<h1>Observing the Effects of a VPN on IP Addressing</h1>
In this lab, we will observe the effects of a VPN (virtual private network), such as Proton VPN, on IP addresses, geographical locations, and web browsing behavior.
 
<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Proton VPN
- Whatsmyipaddress.com

<h2>Operating Systems Used </h2>

- Windows 10 Pro (22H2)

<h2>High-Level Steps</h2>

- Use https://nordvpn.com/what-is-my-ip/deal-site/ to grab your current IP address
- Create a Virtual Machine in Microsoft Azure
- Log into the virtual machine using Remote Desktop Connection
- Use https://nordvpn.com/what-is-my-ip/deal-site/ to grab your VM IP address
- Download Proton VPN, then connect to any VPN
- Use https://nordvpn.com/what-is-my-ip/deal-site/ to grab your new Proton VPN IP address


<h2>Actions and Observations</h2>

<p align="center">
<img src="https://i.imgur.com/ygaFjEv.png" height="80%" width="80%" alt="img"/>
</p>

On your web browser, go to https://nordvpn.com/what-is-my-ip/deal-site/ and grab your current IP Address. 

Note down your current IP address and the city.

<p align="center">
<img src="https://i.imgur.com/DnFRTsK.png" height="80%" width="80%" alt="img"/>
</p>

Go to https://portal.azure.com/ and search "virtual machine" in the search bar, and click "Virtual machines".

<p align="center">
<img src="https://i.imgur.com/vir8b1g.png" height="80%" width="80%" alt="img"/>
</p>

Click "Create", and click "Azure virtual machines".

<p align="center">
<img src="https://i.imgur.com/qrlG7dp.png" height="80%" width="80%" alt="img"/>
</p>

Select your Azure subscription, and a resource group will be created for us. Use "vpn-practice as the virtual machine name, and select a region that's not your current location. In this case, we selected "(Africa) South Africa North". Select "No infrastructure redundancy required", and "Standard". Select "Windows 10 Pro version 22H2 - x64 Gen2" for the image, and "Standard_E2s_v3 - 2 vcpus, 16 GiB memory for size. Check the license box and click the "Review + Create" button.

<p align="center">
<img src="https://i.imgur.com/DESUZFx.png" height="80%" width="80%" alt="img"/>
</p>

We got the "validation passed" message; go ahead and click the "Create" button in the bottom left.

<p align="center">
<img src="https://i.imgur.com/OFirV8e.png" height="80%" width="80%" alt="img"/>
</p>

The message "Your deployment is complete" confirms that our VM has been created.

Click "Go to resource".

<p align="center">
<img src="https://i.imgur.com/JpF9xA7.png" height="80%" width="80%" alt="img"/>
</p>

Copy your VM's public IP address.

<p align="center">
<img src="https://i.imgur.com/Na2gOfc.png" height="80%" width="80%" alt="img"/>
</p>

Open Remote Desktop, paste the copied IP address, and click "Connect" as shown in the image above.

<p align="center">
<img src="https://i.imgur.com/ggh8gCA.png" height="80%" width="80%" alt="img"/>
</p>

Click "More choices" > "Use a different account", Input your VM's username and password, which we used when we created our VM, and click the "Ok" button.

<p align="center">
<img src="https://i.imgur.com/VE02Es2.png" height="80%" width="80%" alt="img"/>
</p>

At the prompt, click "Yes".

<p align="center">
<img src="https://i.imgur.com/ypTy31O.png" height="80%" width="80%" alt="img"/>
</p>

We are now connected to our VM via RDP. Select "No" for all the options and click the "Accept" button.

<p align="center">
<img src="https://i.imgur.com/8JyvCc2.png" height="80%" width="80%" alt="img"/>
</p>

On your VM, click the Microsoft Edge app shortcut on your desktop.

Go to https://nordvpn.com/what-is-my-ip/deal-site/ and click Enter on your keyboard.

<p align="center">
<img src="https://i.imgur.com/9bJLeTa.png" height="80%" width="80%" alt="img"/>
</p>

Remember, when we were creating our VM in Azure, we selected "(Africa) South Africa North" as our location.

As you can see from the image above, our location is South Africa. Note the IP address.

<p align="center">
<img src="https://i.imgur.com/5GVoheM.png" height="80%" width="80%" alt="img"/>
</p>

Next, we will create a free Proton VPN account. 

On your local computer web browser (not your VM's browser), search for "Proton vpn sign up", and click "Proton NPN: Sign-up".

<p align="center">
<img src="https://i.imgur.com/JKsOFyj.png" height="80%" width="80%" alt="img"/>
</p>

Click "Sin up for free".

<p align="center">
<img src="https://i.imgur.com/bpNYe6z.png" height="80%" width="80%" alt="img"/>
</p>

Click "Continue with free VPN" to create your free Proton VPN account.

<p align="center">
<img src="https://i.imgur.com/xfnZgAH.png" height="80%" width="80%" alt="img"/>
</p>

After creating your Proton VPN account on your local computer, go to your VM's web browser and log into your proton VPN account.

Go to "VPN apps" and click "Download" for Windows.

<p align="center">
<img src="https://i.imgur.com/LkDPJFh.png" height="80%" width="80%" alt="img"/>
</p>

Click "Download Proton VPN" to download the Proton VPN application.

<p align="center">
<img src="https://i.imgur.com/UWMZsh4.png" height="80%" width="80%" alt="img"/>
</p>

After it's downloaded, open "File Explorer", click the "Downloads" folder, and double-click "ProtonVPN" to install it.

<p align="center">
<img src="https://i.imgur.com/nvPR6lA.png" height="80%" width="80%" alt="img"/>
</p>

The Proton installation window will pop up. Click 'Ok" > "Next" > "Next" > "Next' > "Install". 

Log in using your username and password.

<p align="center">
<img src="https://i.imgur.com/ZFFNcOj.png" height="80%" width="80%" alt="img"/>
</p>

Within your Proton VPN, click "Quick Connect".

<p align="center">
<img src="https://i.imgur.com/ZFFNcOj.png" height="80%" width="80%" alt="img"/>
</p>

After clicking the "Quick Connect" button, I was connected to a Proton VPN server in the Netherlands. This means that all of my web browsing traffic on the VPN will be routed through the Proton VPN server

NOTE: You might be connected to a different location by the time you are doing this lab.

<p align="center">
<img src="https://i.imgur.com/Mk7HLI4.png" height="80%" width="80%" alt="img"/>
</p>

Go back to https://nordvpn.com/what-is-my-ip/deal-site/ or refresh the web page if you still have it open.

As shown in the image above, you can see our IP address changed and our location changed from South Africa to the Netherlands.

In conclusion, when we connected to our VM via RDP (Remote Desktop), we were actually connecting to a VM located in South Africa. This means that our traffic appeared to be coming from South Africa, even though we were physically located elsewhere. In this sense, it was as if we were using a VPN.












