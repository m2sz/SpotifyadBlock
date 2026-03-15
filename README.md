# 🎵 BlockTheSpot Auto-Installer

An automated, one-click installer to easily deploy the famous [BlockTheSpot](https://github.com/mrpond/BlockTheSpot) patch on the Spotify desktop app for Windows.

## 💡 Why this project?
Installing the BlockTheSpot patch manually requires downloading several `.dll` files, placing them in hidden Windows folders (`AppData`), renaming system files, and repeating the process every time Spotify updates. 

This small utility does **absolutely everything for you**. It uses the official BlockTheSpot files from `mrpond` but automates the entire deployment process.

## ✨ Features
* 📥 **Auto-Download:** Fetches and downloads the latest `.dll` files directly from `mrpond`'s official GitHub API.
* 🔧 **Clean Installation:** Closes Spotify, renames the original `chrome_elf.dll` file, and places the new files in the correct directory.
* 🛑 **Update Blocker (Permanent):** Locks the Spotify `Update` folder at the Windows permission level to prevent the software from overwriting the patch.
* 🚀 **Fast & Invisible:** Everything runs in the background in just a few seconds.

## ⚙️ Prerequisites
1. You must be using the official **Spotify for Windows** desktop application (downloaded from the Spotify website).
2. ⚠️ **Note:** This script does **not** work with the Microsoft Store version of Spotify.

## 🚀 How to use
1. Close Spotify if it is currently running.
2. Double-click the executable. It will ask for **Administrator privileges** (this is required to lock the Spotify update folder).
3. Wait a few seconds... Spotify will automatically restart, fully patched and ad-free!

## 🛡️ Antivirus Note (False Positives)
The provided executable is a PowerShell script compiled using the `ps2exe` tool. Because it is not digitally signed by a corporate entity, **Windows Defender or SmartScreen may show a blue warning screen** or flag it as a threat. 
This is a **false positive**. If you have any doubts, you can check the source code (`.ps1`) provided in this repository and compile/run it yourself.

## 🙏 Credits
* All credit for the actual ad-blocking code (the DLL files) goes to **[mrpond](https://github.com/mrpond/BlockTheSpot)** and the contributors of the original BlockTheSpot project. 
* This repository only contains the wrapper script to make the installation easier for everyday users.
