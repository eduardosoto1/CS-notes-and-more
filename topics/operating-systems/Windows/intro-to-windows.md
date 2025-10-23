# Intro to Windows

Windows is a popular operating system (OS) with many abilities involving system files, utilities, settings, and features.  
This page covers the basics of navigating the OS — focusing on **Windows 10**.

> 💡 **Note:** Windows Server 2025 is the server-oriented version of the Windows OS.

---

## 🖥️ The Desktop (Graphical User Interface)

The **GUI (Graphical User Interface)** is the screen that lets you interact with software when you log in.  
Main components include:

- Desktop  
- Start Menu  
- Search Box  
- Task View  
- Taskbar  
- Toolbars  
- Notifications  

---

## 📂 File System

🔗 [Learn more about file systems](https://learn.microsoft.com/en-us/troubleshoot/windows-client/backup-and-storage/fat-hpfs-and-ntfs-file-systems)

### NTFS (New Technology File System)

Modern versions of Windows use **NTFS**.  
Earlier systems used **FAT16/FAT32 (File Allocation Table)** and **HPFS (High Performance File System).**

#### Key Features of NTFS:
- **Journaling file system** — can repair folders/files using log file data (unlike FAT)
- Supports files **larger than 4GB**
- Allows **specific permissions** on folders and files
- Enables **compression** and **encryption** (EFS)

#### NTFS Permissions
Permissions control access to files and folders:

| Permission | Description |
|-------------|-------------|
| **Full Control** | Read, write, change, and delete files and subfolders |
| **Modify** | Read/write files and subfolders; allows deletion |
| **Read & Execute** | View, access, and execute files |
| **List Folder Contents** | View files/subfolders and execute files (for folders) |
| **Read** | View/access file or folder content |
| **Write** | Add files/subfolders and write to a file |

---

### ⚙️ Alternate Data Streams (ADS)

**ADS (Alternate Data Streams)** is a file attribute unique to NTFS.

- Every file has one data stream: `$DATA`
- ADS allows multiple data streams within a single file
- Not visible in Windows Explorer (third-party tools or PowerShell required)

#### Uses of ADS:
- Malware can hide data in ADS  
- Used legitimately to store metadata (e.g., download source tags)

---

### 🔍 Viewing File System Type

**To check your file system:**
1. Open **File Explorer**
2. Go to **This PC**
3. Right-click a drive → **Properties**
4. Look for **File System:** (e.g., NTFS)

**To check file/folder permissions:**
1. Right-click → **Properties**
2. Go to the **Security** tab
3. Select a user/group to view permissions

---

## 🧠 The Windows\System32 Folder

The **Windows folder (C:\Windows)** contains core operating system files.  
It’s usually located on the **C:** drive but can vary.

- Access via **%windir%** environment variable  
- **Environment variables** store system info (like paths, processor count, and temp folders)

### 🗂️ System32
**Location:** `C:\Windows\System32`  
Contains vital files and executables required by Windows.

> ⚠️ **Warning:** Do not delete or modify files in System32 — it can break your system.

---

## 👤 User Accounts, Profiles, & Permissions

Windows has two main types of user accounts:
- **Administrator** — full system control (can add/delete users, modify settings)
- **Standard User** — limited control, mainly for personal files/folders

---

### User Accounts Overview

To manage users:
1. Open **Start Menu** → search for **Other users**
   - *(Standard Users may not see this option)*
2. Select **Add someone else to this PC**
3. Choose the account type

When a user is created, a **profile folder** appears under `C:\Users`.

Each user folder contains:
- Desktop  
- Documents  
- Downloads  
- Music  
- Pictures  

---

### Local User and Group Management

To access:
1. **Right-click Start Menu** → **Run**
2. Type `lusrmgr.msc`
3. Click **Groups** to view local groups and their permissions

- Each group has defined permissions
- Users can belong to **multiple groups**

---

## ⚙️ Settings & Control Panel

- **Settings** handles most common configuration options  
- **Control Panel** allows for deeper, system-level changes  
- Some **Settings** pages will redirect you to the **Control Panel**

---

## 🧾 Task Manager

**Task Manager** shows running apps, background processes, and system performance (CPU, RAM, etc.)

### Access Methods:
- **Right-click Taskbar** → **Task Manager**
- Press **Ctrl + Shift + Esc**
- Click **More details** for full view

---

✅ **Summary**
- Windows uses **NTFS** for its file system  
- **System32** holds essential OS files  
- User accounts define system permissions  
- Use **Task Manager**, **Settings**, and **Control Panel** for management and troubleshooting  

---
