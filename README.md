# 🚀 Titan Inject v3.0 (Beast Mode)

A powerful, standalone, and stealth-focused DLL Injector written in pure **C++ (Win32 API)**. 
Titan Inject features a custom Dark Mode GUI, multiple advanced injection methods, cloud payload delivery, and trace-cleaning capabilities.

**Developed by:** Adnan 1337w0rm ([@I337w0rm](https://github.com/I337w0rm))
<img width="405" height="477" alt="image" src="https://github.com/user-attachments/assets/7290b761-820e-4351-8886-a2c7e357da8f" />

---

## 🔥 Advanced Features

* **Multiple Injection Methods:**
  * **Standard:** Classic `CreateRemoteThread` + `LoadLibraryA` injection.
  * **APC Stealth:** Uses Asynchronous Procedure Calls (`QueueUserAPC`) to hijack existing threads and silently load the payload without creating suspicious remote threads.
  * **Process Hollowing (Base):** UI and base logic initialized for suspending and unmapping target memory.
* **☁️ Cloud Inject:** Don't want the DLL on your disk? Paste an HTTP/HTTPS direct link into the DLL path. Titan Inject will download it to a hidden Temp folder, inject it, and instantly wipe the payload from the disk.
* **🧹 Trace Cleaner:** Built-in stealth mechanism that flushes the Windows DNS cache and clears the "Recent Documents" history post-injection to leave zero traces behind.
* **⚙️ Smart Automation (Multi-threaded):**
  * **Auto-Inject:** Select a process, and the injector will wait in the background. As soon as the game/app starts, it injects automatically.
  * **Delay Inject:** Set a delay (in seconds) to wait before injecting, preventing crashes on slow-loading games.
* **🖥️ Modern Win32 GUI:** * Custom Dark Mode interface with zero external dependencies (No Qt, No ImGui).
  * **Real-time Debug Console:** Integrated log terminal to monitor every step of the injection process.
  * **Drag & Drop:** Simply drag your `.dll` file into the window.
* **🌍 Dual-Language:** Switch seamlessly between English and Bosnian on the fly.

---

## 🎮 How to Use

1. Run `TitanInject.exe` **as Administrator** (Mandatory for memory reading/writing).
2. Accept the initial disclaimer.
3. Select your target process from the dropdown (or click *R* to refresh).
4. Browse for your local `.dll` file, drag & drop it, OR paste a direct URL (e.g., `http://example.com/cheat.dll`).
5. Choose your Injection Method (Standard or APC).
6. Configure Auto-Inject, Close on Inject, or Delays if needed.
7. Click **INJECT** and check the internal console for real-time status.

---

## ⚠️ Disclaimer & Warning

**STRICTLY FOR EDUCATIONAL AND REVERSE ENGINEERING PURPOSES.**

This tool was created to understand Windows API, process memory management, and thread manipulation. The author (**Adnan 1337w0rm**) takes absolutely **NO responsibility** for:
* Potential bans in video games.
* Anti-Cheat sanctions (VAC, BattlEye, EAC, Vanguard, etc.).
* Any system instability, misuse, or damage caused by this software.

**USE AT YOUR OWN RISK!**
