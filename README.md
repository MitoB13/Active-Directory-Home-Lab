<h1>Active Directory Home Lab: </h1>

 

<h2>🧠 Active Directory Lab Summary</h2>
Built a domain environment using VMware Workstation with Windows Server as a Domain Controller and a Windows 11 client. Configured Active Directory, created OUs, and applied key GPOs (password policy, drive mapping, USB restriction, etc.). Joined the client to the NorthSide.local domain. Set up File Services with FSRM, enabling Quota Management and File Screening to control storage and block unauthorized file types.
<br />

<h2>Environments Used </h2>

- <b>Windows 11
- Windows Server 2022
- VMware</b>

<h2>Lab walk-through:</h2>

<p>
🖥️ 1. Set Up Virtual Machines

- Installed **Windows Server** and **Windows 11** as virtual machines using **VMware Workstation**.
- The **Windows Server** acts as the Domain Controller.
- The **Windows 11 VM** will serve as the client machine.

🛠️ 2. Configure Active Directory on Windows Server

- Promoted the Windows Server to a **Domain Controller**.
- Installed and configured **Active Directory Domain Services (AD DS)**.
- Created a new domain: **`NorthSide.local`**.

🗂️ 3. Organize with Organizational Units (OUs)

- Created the following **Organizational Units** within Active Directory:
    - `Sales`
    - `HR`
    - `IT`

🔐 4. Create & Apply Group Policy Objects (GPOs)

Created and linked the following **GPOs** to relevant OUs or the domain:

- ✅ **Password Policy**
- 💾 **Drive Mapping**
- 🖼️ **Desktop Wallpaper**
- 🔒 **Disable USB Storage**
- 🚫 **Restrict Command Prompt**
- 🔁 **Account Lockout Policy**

🌐 5. Network Configuration

- Assigned a **static IP address** to the Windows Server for reliable DNS/domain services.

🧑‍💻 6. Join Windows 11 Client to the Domain

- Configured the Windows 11 client with the server’s IP as the **DNS server**.
- Joined the client to the **`NorthSide.local`** domain.
- Verified domain join was successful and applied GPOs as expected.

🧑‍💻 7. Setting Up File Services

- Created a shared folder with appropriate NTFS permissions for domain users.
- Installed and configured **File Server Resource Manager (FSRM)** to manage storage.
- Implemented **Quota Management** and **File Screening** to block restricted file types (e.g., `.mp3`, `.exe`, `.iso`).

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
