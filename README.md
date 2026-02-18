# Lab 7 Creating Local Users in Windows
Practice creating, managing, and removing local user accounts in Windows 11

## 📅 Date
February 18, 2026

---

## 🎯 Objective

This lab demostrates the creation and management of local user accounts in Windows 11 using both graphical and command-line administrative tools.

---

## 🖥️ Environment Details

| Component | Details |
| ----------- | -------- |
| Host OS | Windows 11 |
| VM Plateform | Oracle VirtualBox |
| Guest OS | Windows 11 (64-bit ISO) |
| CPU | 3 vCPU |
| RAM | 4 GB (4096 MB) |
| Disk | 80.00 GB |

---

## 🔧 METHOD 1: Using Computer Management (GUI) 

1. Launched the Windows 11 virtual machine.
2. Opened Computer Management from the taskbar search.
3. Navigated to Local Users and Groups.
4. Right-clicked "Users" and selected "New User"
5. Entered full name and password credentials.
6. Successfully created local user acccount.

This method demostrates how administrators can manage accounts through the graphical interface.

## 🔧 METHOD 2: Using Windows Powershell (Administrator)

1. Opened PowerShell with administrative privileges.
2. Used the New-LocalUser cmdlet to create user accounts with full name and description parameters.
3. Created secure passwords using the Read-Host -AsSecureString command to prevent plaintext exposure.

This method demostrates command-line user administration, which is commonly used in enterprise environments. 

---

## ⚠️ Issues Encountered and Resolution

**- Issue:** Newly created users did not immediately appear when attempting to enumarate accounts using standard directory commands. 

**- Resolution:** Used the Get-LocalUser command to properly enumerate local user accounts in the system.

---

## ✅ Outcome

Successfully created eight local user accounts using both GUI and PowerShell methods.

Confirmed that local accounts are created at the system level and that user profile directories are generated only upon first successful login. 

---

## 💭 Reflection

This lab strengthended my understaning of: 

- The difference between GUI-based and command-line administration in Windows environments.
- Secure password handling using SecireString to prevent plaintext exposere.
- How local user accounts are stored and managed at the operating sysem level.

Future Practice:

Next, I plan to practice modifying user permissions and adding accounts to security groups. 

---
