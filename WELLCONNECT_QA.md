# WELL CONNECT QA 

Please note that from now on, the WELL CONNECT will only be referred to as the BOX in this document.

## Test Set 1: Power 
#### Overview / Objective
this will test all ways of powering the box

### 1.0 How to power on and off the box
1. Power on the box
   - Press and hold the `power` button on the front left side of box until power button starts blinking.
   - After about 30–40 seconds, the display should turn on.
2. Power off the box
    - Press and hold the `power` button on the front left side of box until power button starts blinking.
    - After about 30–40 seconds, the display should turn off.

### 1.1 USB-C to USB-C 
1. Using a USB-C to USB-C connect the box to a USB-C power adapter. 
   - Does the power indicator on the next to the USB-C port light up 
     - Red is charging 
     - Green is charged
2. Power on the box
3. wait until the box has fully started  
4. Power off the box for the next test needed. 

### 1.2 USB-A to USB-C  
1. Using a USB-A to USB-C connect the box to a USB-A power adapter.
   - Does the power indicator on the next to the USB-C port light up
       - Red is charging
       - Green is charged
2. Power on the box
3. wait until the box has fully started
4. Power off the box for the next test needed.

### 1.3 USB-C Power bank 
1. Using a USB-C to USB-C connect the box to the USB-C port on the power bank. 
   - Does the power indicator on the next to the USB-C port light up
      - Red is charging
      - Green is charged
2. Power on the box
3. wait until the box has fully started
4. Power off the box for the next test needed.

### 1.4 USB-A Power bank
1. Using a USB-A to USB-C connect the box to the USB-A port on the power bank.
   - Does the power indicator on the next to the USB-C port light up
      - Red is charging
      - Green is charged
2. Power on the box
3. wait until the box has fully started
4. Power off the box for the next test needed. 

## Test Set 2: Encoder Test
#### Overview / Objective
Test if the encoder rotation and push button Enter are working. 

### 2.1 Encoder Test
1.	Power on the box. 
2.	Once you see the main screen, wait 30 seconds.
3.	Rotate the encoder to `Settings` then navigate to `Firmware Version` press `<Enter>` by pushing in on the encoder.
You should now see the firmware version on the screen. 

## Test Set 3: Back Button Test
#### Overview / Objective
Test if the encoder rotation and push button are working. 

### 3.1 Back Button Test
1.	Once you see the main screen, wait 30 seconds.
2.	Rotate the encoder to `Settings`
3.	Press `<Enter>`
4.	Press the `<Back>` button next to the encoder to return to the previous screen.
5.	Press the `<Back>` button next to the encoder again, which returns you to the main screen. 

## Test Set 4: Link and Unlink Fixtures
#### Overview / Objective
Test the ability to link and unlink fixtures to the Box.

### 4.1: Linking
1.	Make sure your test fixture is ready to be linked.
2.	Using the rotary encoder, navigate to `“Linking”` and press `<Enter>`.
3.	Navigate to `“Link”` and press `<Enter>` This process can take 30 to 60 seconds to complete.
4.	Check your fixtures to see if linking was successful.

### 4.2: Unlinking
1.	Make sure your test fixture is ready to be linked.
2.	Using the rotary encoder, navigate to `“linking”` and press `<Enter>`.
3.	Navigate to `“Unlink”` and press `<Enter>`. This process can take 30 to 60 seconds to complete.
4.	Check your fixtures to see if unlinking was successful. 

## Test Set 5: USB A Female Port
#### Overview / Objective
Test the connectivity of the USB female port to the Box.

### 5.1
1.	Use a formatted USB thumb drive.
2.	Insert thumb drive into the USB A female
3.	Using the rotary encoder, navigate to `“Settings”` and press `<Enter>`.
4.	Navigate to “USB Test” You will get a “Result:
      * “PASS”
      * “FAIL” 

## Test Set 6: DMX Output
#### Overview / Objective
Test the connectivity of the USB female port to the Box. You will need two fixtures 
for testing, one with WDMX and one with a five-pin DMX port. 

### 6.1: WDMX - Timo Two and DMX 5 pin out
1.	Link one fixture “A” to the Box using WDMX
2.	Connect to another fixture “B” using a five-pin XLR to the box's five-pin DMX port.
3.	Using the rotary encoder, navigate to `“Settings”` and press `<Enter>`.
4.	Navigate to `“Output Test”` and press `<Enter>`.

Once the countdown timer starts, all 512 DMX channels will change from 255 to 0 every 2 
seconds for two minutes. Both lights should now be flashing.  You can also test the output with a Swisson DMX tester in “Receive DMX”. 

## Test Set 7: DMX to WDMX
#### Overview / Objective
Test the DMX to WDMX mode. You will need one WELL fixture, a DMX controller, and RDM2GO.

### 7.1: Test DMX IN via 5-pin
1.	Link one fixture to the Box
2.	Set the personality to 12ch and address to 1
3.	Patch the console or use an RDM2GO.
4.	Set channels ch1=100% or 255 , ch4 = 100% or 255.
5.	Connect the controller/RDM2GO to the box using a 5-pin DMX cable.
6.	Using the rotary encoder, navigate to “Mode” and press “Enter”
7.	 Navigate to “DMX to WDMX” and press “Enter” 

The light should now be red at full brightness. 

## Test Set 8: Web UI
#### Overview / Objective
Test the ability to access the web UI and up date firmware from a PC.

>Note: The Box's IP address is 192.168.2.1, and the web UI is only available for the first 30 minutes 
after it is powered on. 

####  8.1 Access Web UI
1. Set PC’s IP address to 192.168.2.100
2. Connect PC to the Box using a CAT-5 cable. 
3. Connect power to the Box. 
4. Power on the box by holding the power button until it flashes slowly. 
5. Once you see the main screen appears and the encoder is working, go to the next step. 
6. On the PC, open a web browser like Chrome and navigate to 192.168.2.1 
7. If you should now see the web UI. 

### 8.2 Update UI 
This will update the web UI. **Note: this is only needed if there is an update.**
1.	Connect to the web interface like in test 6. 
2.	Click “choose file,” which will open a file browser 
3.	Navigate to the web UI “.zip” file 
4.	Click “UPGRADE.”  
5.	Wait until completed 
6.	Power cycle the box. 

### 8.3 Update fiemware via web UI
This will upgrade the firmware of the box. **Note: this is only needed if there is an update.**
1.	Connect to the web interface like in test 6. 
2.	Click “choose file,” which will open a file browser 
3.	Navigate to the Well Connect firmware “.zip” file 
4.	Click “UPGRADE.”  
5.	Wait until completed 
6.	Power cycle the box. 

## Test Set 9: Bluetooth packet test
#### Overview / Objective
This will test the Bluetooth connectivity/packet loss.  
1. Open the “Connect_app” app
2. From the “Home” screen toggle the off button to on 
3. Click “settings” 
4. Click Developer Settings
5.	Click “Start 5s Packet Test” after 10 to 20 seconds, the results will pop up. If you 
are within one to two meters of the Box, you should get 0% loss

## Test Set 9: ArtNet to WDMX
#### Overview / Objective
Test if the ArtNet in to WDMX out is working. 
1. Link one or more fixtures to the Box using WDMX
2. Set the IP Address, Unaverse, and subnet if needed. 
#### Setting the IP Address 
1. Navigate to the `"Settings"` menu and press `<Enter>`
2. Navigate to the `"Ethernet options"` menu and press `<Enter>`
3. Navigate to the `"IP Address"` menu and press `<Enter>`
4. Navigate to the `"Edit"` menu and press `<Enter>`
5. Navigate to the IP segment you want to change and press `<Enter>`
