# 🛠️ Installation Guide for Stimulator P24 Science

Follow these clear steps to properly install **Python**, **PyUSB**, and the necessary **Stimulator Driver** on your Windows PC.

---

## 📌 A. Installing Python and PyUSB Library

### 1. Download Python
Download Python 3.12.0 for Windows from the official site:
- [Python 3.12.0 (64-bit)](https://www.python.org/ftp/python/3.12.0/python-3.12.0-amd64.exe)

### 2. Installation Steps
Run the downloaded installer and ensure you tick these boxes:
- ☑️ **Install launcher for all users (recommended)**
- ☑️ **Add Python 3.12 to PATH**

> **Note:** This ensures Python is accessible via Command Prompt.

### 3. Verify Python & Pip Installation
Open **Command Prompt** (type `cmd` in Windows Search), then run:

```cmd
python --version
pip --version
```

Ensure both commands return their installed version numbers.

### 4. Install PyUSB
In the same command window, run:
```cmd
pip install pyusb
```

### 5. Reboot Your PC
Restart your computer to apply the changes.

---

## 📌 B. Installing Stimulator Driver (libusbK)

### 1. Connect the Device
Plug in your **Stimulator P24 Science** to the Windows PC.  
Ensure the LED turns **green**.

### 2. Download libusbK
Download the latest libusbK installer from:
- [libusbK (latest version)](https://sourceforge.net/projects/libusbk/files/latest/download)

### 3. Install libusbK
Run the `.exe` file and select all available tasks.

### 4. Select libusbK Driver
- Select the **libusbK** driver (typically `v3.0.7.0`) and click **Next**.

### 5. Select the USB Device
- Tick **Show All Devices**.
- Find and select the device with:
  - **VendorID:** `0x0483`
  - **ProductID:** `0x5740`
- Click **Next**, then click **Install**.

### 6. Verify Driver Installation
- After installation, click **OK** and reboot your PC.
- Verify using the **Device Manager**:
  - Right-click **Windows Icon → Device Manager**.
  - The device should be listed under:
    - **Ports (COM & LPT)**, or
    - **Universal Serial Bus devices**
  - Ensure the installed driver details correspond to **libusbK**.

---

🎉 **Installation Complete!**  
Your Stimulator P24 Science is now ready to use.
