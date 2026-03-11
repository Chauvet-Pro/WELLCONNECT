# Tester's Guide

Welcome to the WELLCONNECT testing team! This guide provides instructions on how to set up your hardware for testing the latest versions of the WELLCONNECT app.

> [!IMPORTANT]  
> To use the latest test version of the app, you **must** have the latest **WebUI** and **Box Firmware** installed on your hardware.

---

## 🛠 Preparation

Before you begin, ensure you have the necessary files:

1.  **Download WebUI:** Get the latest version from the [firmware](./firmware) directory.
2.  **Download Box Firmware:** Get the latest testing firmware from the [firmware](./firmware) directory.

### Network Setup
*   **Box IP Address:** `192.168.2.1`
*   **PC IP Address:** Set your computer to a static IP in the same range (e.g., `192.168.2.100`).
*   **Connection:** Connect your PC to the Box using a CAT-5 Ethernet cable.

---

## 📥 Installation Steps

The update process must be done in two stages.

### Stage 1: Update the WebUI
1.  **Power on** the box.
2.  Open a web browser and navigate to `192.168.2.1`.
3.  In the WebUI, select the **WebUI firmware file** (`.zip`) you downloaded.
4.  Click **Upgrade** and wait for the process to complete.
5.  **Reboot** the box.

### Stage 2: Update the Box Firmware
1.  Once the box has rebooted, **navigate** to `192.168.2.1` again.
2.  Select the **Box firmware file** (`.zip`) you downloaded.
3.  Click **Upgrade** and wait for the process to complete.
4.  **Reboot** the box.
5.  **Done!** You are now ready to test.

> [!NOTE]  
> The WebUI is typically only available for the first 30 minutes after the box is powered on.

---

## 🐛 Reporting Issues

Your feedback is essential for improving WELLCONNECT. If you find any bugs or have suggestions, please let us know!

**How to report:**
1.  Go to the [WELLCONNECT Issues](https://github.com/Chauvet-Pro/WELLCONNECT/issues) page.
2.  Click **New Issue**.
3.  Include details about the versions you are using and steps to reproduce the issue. Include screenshots and videos if possible

Thank you for your help!

