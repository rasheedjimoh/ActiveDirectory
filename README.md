# Active Directory

## Introduction
Let's embark on a modest exploration into the intricacies of Windows Server 2022 and Windows 10 Pro in our ongoing project. This endeavour humbly tackles server challenges, addressing nuances like power options and network settings. We navigate the elevation of Windows Server through roles, the creation of admin accounts, and the configuration of remote access. Witness the simplicity of account automation, establishing DHCP scopes, and seamlessly integrating Windows clients into the domain. Join us on this unassuming journey as we craft a secure and interconnected Windows environment, demonstrating reachability through ping tests and laying the groundwork for a sturdy IT infrastructure.

![domain-joined](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/3e488293-b8bd-4b05-bbf8-8533196d9f91)




## Technologies/Stacks
- Active Directory(Active Directory Domain Services and Active Directory Users and Computers)
- DHCP
- DNS
- Remote Access
- Domain Controller
- NAT/RAS
- PowerShell for Automating account creation and management

## Process/Procedure

**Windows Server**
1. Add ADDS role.
2. Promote to DC.
3. Created an Admin account.
4. Install Remote Access+Routing+Direct Access and VPN(RAS) - Configured and enabled to use 1 public IP address. User internet facing NIC as the public IP.
5. DC is automatically made the DNS server
6. Install and configure DHCP scope for the clients on the DC.
7. Automate account creation.
8. Join the client computer to the DC.

**Windows Client**
1. Setup Windows 10
2. Joined domain using private IP
3. Prove reachability by pinging Google, Cloudflare and the DC

## Verification
**IP configuration for internal network**
![ip1](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/5721282f-42c6-432e-804a-d9d6122d1f73)


**IP configuration for external network/Public IP**
![ip0](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/18b104f2-fc66-47d8-ad9e-862767d087a4)


**Joining domain**
![domain-joined](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/4bf8b102-3950-4584-b6ac-0d4252d14096)


**Automating Account Creation**
![automate-account-creation](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/13fa0a9e-4213-4aaa-a41d-9a515aa1f5c8)


**IP Configuration and reachability test**
![reachability-testing-for-client1](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/864980c4-c740-4e10-94c5-c4bc124a47ff)


**Names notepad of supposed staff members**
![names](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/0fa20f76-cf96-4b90-bdf8-801f052fdb55)


## Scripts

**Name generation script**
![generate-names](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/8d57b221-ff37-4526-9e03-572977c7f6bf)

**Account creation script**
![account-creation script](https://github.com/rasheedjimoh/ActiveDirectory/assets/157264080/7549e2af-8fd7-4742-8fc2-76182f64c3fa)


## Conclusion
In conclusion, this mini project with Windows Server 2022 and Windows 10 Pro showcases our dedication to precision and efficiency in IT management. From addressing server challenges to creating a secure Windows environment, every step reflects a commitment to excellence. The seamless integration of Windows clients, automated account creation, and DHCP scope establishment highlights our focus on user-centric design. This mini project is not just a technical accomplishment but a testament to our capacity for innovation. It fortifies our foundation for future endeavours, emphasizing our commitment to achieving excellence in IT with continuous improvement.



## Acronyms
1. **NAT (Network Address Translation):** Translates addresses for communication between different networks.
2. **RAS (Remote Access Service):** Enables secure remote connections, acting as a virtual bridge for distant access to computers.
3. **DC (Domain Controller):** Central authority managing permissions in a network.
4. **ADDS (Active Directory Domain Services):** Efficiently organizes and manages network entities for seamless operations.
5. **ADUC (Active Directory Users and Computers):** User-friendly control panel managing users, computers, and devices in a network.
6. **DHCP (Dynamic Host Configuration Protocol):** Dynamically assigns unique IP addresses, simplifying network configuration.
7. **NIC (Network Interface Card):** Essential hardware enabling computer connectivity and communication within a network.
