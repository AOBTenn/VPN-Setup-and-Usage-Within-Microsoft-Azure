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

![image](https://github.com/user-attachments/assets/bc562773-8604-4db7-9e2b-c8c37d8b8dc0)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/a613c192-56f1-4e2f-b756-62087ee4ea75)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/609b6d25-8b06-433c-81e1-5a28fcf91405)
 <p>  
</p>

2) Get VM public Ip address -> Connect using Remote Desktop
 <p>  
</p>

 ![image](https://github.com/user-attachments/assets/c478e9a2-472a-469f-9517-c03507750263)
  <p>  
</p>

 ![image](https://github.com/user-attachments/assets/1f8037b3-5b98-4b63-b3e3-248d5f66dcbe)
 <p>  
</p>

3) Browse from your personal computer to "https://whatismyipaddress.com" -> Record IPv4 address and info under "My Ip information" in notepad for comparison later

![image](https://github.com/user-attachments/assets/5bc420c5-40d0-4e69-a5fe-7e9bbf26afce)
 <p>  
</p>

4) From within the virtual machine browse to "https://whatismyipaddress.com" -> Record IPv4 address and info under "My Ip information" in the same notepad for comparison also

![image](https://github.com/user-attachments/assets/052d55a1-cc1d-4e73-b96f-e1aa1fb5d046)
 <p>  
</p>

5) Browse and sign up for a free trial account from your personal computer to "https://account.protonvpn.com/signup?plan-free&language=en"

![image](https://github.com/user-attachments/assets/25ad6814-3ed8-4b6d-9271-7f8f61680457)
 <p>  
</p>

6) After creating an account with Proton VPN, download the connection sotfware inside of the virtual machine, not on your personal computer

![image](https://github.com/user-attachments/assets/c5d659b9-0c8d-432d-b7a4-d13a7e1f781e)
 <p>  
</p>

![image](https://github.com/user-attachments/assets/a4f4d47d-ca09-44eb-ac46-b15cf4416cfc)
 <p>  
</p>

7) Copy and save your login password in notepad -> Login ->  Click "Quick Connect" to connect to a VPN server

8) Re-browse within the virtual machine while connected to "https://whatismyipaddress.com" -> Record IPv4 address and info under "My Ip information" in the same notepad for comparison as well

![image](https://github.com/user-attachments/assets/a8453581-4822-45ea-b0f1-a3f93ff9a1f7)

 <p>  
</p>
 <p>  
</p>

Recap

  As we compare the different Ip information listed on the note pad, we see that the Ip information changed each time we went to "https://whatismyipaddress.com." From the personal computer the website states our generalized "physical" location based on the server/router connenction. When we browsed from the virtual machine within Microsoft Azure to check the ip address this changed our supposed "physical" location within the United States. This is because Nicrosoft Azure  in a sense acted like a virtual private network tunnel. Lastly when you rebrowse to "https://whatismyipaddress.com" for the final time while connected to a VPN server we see that the Ip address and our location completely changed as though we were sitting in another country. As you can observe a VPN can allow you to browse on the Internet as thought you are sitting in the location of the region of that server while you are actually and physically be in another part of the world. This can be useful if need be for you to access certain websites with particular content that are only accessable or not accessable from a certain region. To demostrate this we will browse to "Netflix.com" and compare the difference in the webpage and user interface (UI).  

 9) Browse to Netflix.com from within your personal computer ->  Browse to Netflix.com from within the virtual achine while connected to the VPN server

  As we can see both websites have noticable changes. There are different line-up of English or Japanese tv shows and movies in the backdrop, English or Japanese text graphics, and also English or Japanese currency changes between both sites from the same company "Netflix.com".

  This concludes the lab project demonstrating how to install and use a virtual private network in addition to what VPNs can be used for on the world wide web.


