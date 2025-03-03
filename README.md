 ![image](https://github.com/user-attachments/assets/4ae1f81a-293f-4be8-a86e-210d6a47326a) 

This project details the steps to use a Virtual Private network (VPN) within Microsoft Azure. The VPN we wil be using is a free trial account from Proton VPN. We will also check what happens while using a VPN on the internet.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Proton VPN
- Personal Computer

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

Project Guide Steps

1) Create Virtual Machine

  -Create Resource Group -> Select a Name for the VM -> Select a Region -> Select Security Type -> *Note* Select Size of VM 2vcps/8gib memory -> Enter a Username and Password -> Check Licensing box -> Click next to Disk, Next to Networking -> Click Review and Create



2) Get VM public Ip address and connect using Remote Desktop

3) Browse from your personal computer to "https://whatismyipaddress.com" -> Record IPv4 address and info under "My Ip information" in notepad for comparison later

4) From within the virtual machine browse to "https://whatismyipaddress.com" -> Record IPv4 address and info under "My Ip information" in the same notepad for comparison also

5) Browse and sign up for a free trial account from your personal computer to "https://account.protonvpn.com/signup?plan-free&language=en"

6) After creating an account with Proton VPN, download the connection sotfware inside of the virtual machine, not on your personal computer

7) Copy and save your login password in notepad -> Login ->  Click "Quick Connect" to connect to a VPN server

8) Re-browse within the virtual machine while connected to "https://whatismyipaddress.com" -> Record IPv4 address and info under "My Ip information" in the same notepad for comparison as well

Recap

  As we compare the different Ip information aon the note pad, we see that the Ip information changed each time we went to "https://whatismyipaddress.com." From the personal computer the website states our generalized "physical" location bsed on the server/router connenction. When we browed from the virtual machine within Microsoft Azure to check the ip address this changed our supposed "physical" location within the United States. This is because Nicrosoft Azure created or acted like a private network tunnel in a sense. Lastly when you rebrowse to "https://whatismyipaddress.com" for the final time while connected to a vpn server we see that the Ip address and our location completely changed as though we were sitting in another country. As you can observe that a VPN can all you to browse as thought you are sitting in located within the region of that server even though to can physically be on another part of the world. This can be useful you waant to access certain websites that are only accessable ithin a certain region or not if need be. To demostrate this we will browse to "Netflix.com" and compare the difference in the webpage and user interface (UI).  

  Browse to Netflix.com from within your personal computer ->  Browse to Netflix.com from within the virtual achine while connected to the VPN server

  As we can see both websites have noticable changes. There are different line-up of English or Japanese tv shows and movies in the backdrop, English or Japanese text graphics, and also English or Japanese currency changes between both sites from the same company "Netflix.com".

  This concludes the lab project demonstrating how to install and use a virtual private network in addition to what VPNs can be used for on the world wide web.

  <p>
</p>
