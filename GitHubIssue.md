# “GitHub could not fetch”

Problem: The box firmware will not update and the error message is "GitHub could not fetch". This is because the system time is incorrect, so GitHub rejects the request. The latest firmware is 4.1.10.
The time is set automatically via the app, with no user interaction needed.

To fix this issue, follow the steps below:

> [!NOTE]
> Back up your project before you start, as this process will erase all your data.

## 🛠 Preparation

Before you begin, ensure you have the necessary files:

1.  **Download WebUI:** Get the latest version: [`webui_v5.1.0.zip`](https://github.com/Chauvet-Pro/WELLCONNECT/raw/refs/heads/main/firmware/webui_v5.1.0.zip).
2.  **Download Box Firmware:** Get the latest 4.1.* firmware: [`well_connect_firmware_v4.1.10.zip`](https://github.com/Chauvet-Pro/WELLCONNECT/raw/refs/heads/main/firmware/well_connect_firmware_v4.1.10.zip).

---
## Network Setup
> [!NOTE]
> The box has two IPv4 addresses: `192.168.2.1` for the WebUI (which cannot be changed),
> and one for Art-Net/sACN (typically `2.0.0.1`) that can be changed by the user.
  
* **Box IP Address:** `192.168.2.1`
*   **PC IP Address:** Set your computer to a static IP in the same range (e.g., `192.168.2.100`).
*   **Connection:** Connect your PC to the Box using a CAT-5 Ethernet cable.
---

## 📥 Installation Steps

The update process must be completed in four stages.

### Stage 1: Update the WebUI
1.  **Power on** the Box.
2.  Open a web browser and navigate to `192.168.2.1`.
3.  In the WebUI, select the **WebUI firmware file** (`.zip`) you downloaded.
4.  Click **Upgrade** and wait for the process to complete.
5.  **Reboot** the Box.

### Stage 2: Destroy Data
1. **Power on** the Box.
2. Open a web browser and navigate to `192.168.2.1`.
3. Navigate to **Upgrade**.
4. Click **Destroy Data** and wait for the process to complete.
5. **Reboot** the Box.

### Stage 3: Update the Box Firmware
1.  Once the Box has rebooted, **navigate** to `192.168.2.1` again.
2.  Select the **Box firmware file** (`.zip`) you downloaded.
3.  Click **Upgrade** and wait for the process to complete.
4.  **Reboot** the Box.

### Stage 4: Verify Update and Delete Data
1.  **Power on** the Box.
2.  Use the rotary encoder to navigate to **Settings > Firmware**. You should see the new version.
3.  Now navigate to **Settings > Delete Data & Restart** to delete the old data.
4.  **Reboot** the Box.
5.  All done!
