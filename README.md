<h1>ADDI AI Coding </h1>
<hr/>
Block coding application utilizing ADDI blocks
<br/><br/>
<h1> 📱 Project Introduction </h1>
<hr/>
Connect Addi blocks via Bluetooth. <br/>
Then, perform block coding and execute it to see the ADDI blocks operate in real-time.
<br/><br/>
<h1>:calendar: When? </h1>
<hr/>
240201~ , KIST_Creamo
<br/><br/>
<h1>🙂 Members </h1>
<hr/>

|Members|
|------|
|Seungyeon JI|
|Heeyun HEO|
|Jiwoo BYUN|
|A Lim HAN|

<h1>:gear: Environment Setting</h1>
<hr/>

[![예제](http://img.youtube.com/vi/usE9IKaogDU/0.jpg)](https://youtu.be/usE9IKaogDU?t=0s) 

<ul>
  <li><b>IDE: Android Studio 2022.3.1.21</b></li>
  <li><b>Flutter SDK: 3.16.8</b></li>
</ul>
<br/><br/>
<h1>▶ How to RUN? </h1>
<hr/>

    flutter run lib/main.dart


<br/>
<h1>🏆 Results </h1>
<hr/>

<h2> MAIN PAGE</h2>

![1](https://github.com/multi-sensor/CREAMO_Team_A/assets/83489449/d09c1b2c-32e4-495d-96c2-a585e66614e2)
<br/>
<h2> START PAGE </h2>

![2](https://github.com/multi-sensor/CREAMO_Team_A/assets/83489449/d7e5be24-9f6e-4227-aec1-9d99aad36ded)
<br/>
<h2>PUZZLE PAGE</h2>

![3](https://github.com/multi-sensor/CREAMO_Team_A/assets/83489449/7e49b106-df8f-45f0-82f6-2b975b5b2970)

TBD

<br/><br/>
<h1> ➕ Details </h1>
<hr/>

`main.dart`

* The file that runs the application. 


`splash_page.dart`

* This is the initial screen where Addi AI coding is executed.


`start_page.dart`

* The page is for choosing between "Getting Started" and "How to Use."


`content_page.dart`

* You can check the problem table of contents and select a problem from here.


`puzzle_page.dart`
1. <b>Drag and Drop</b>: Users can drag puzzle blocks from a horizontal list and drop them onto the drop target area.

2. <b>Snap-to-Grid</b>: When a block is dropped near another block, it snaps into place with a grid-like alignment, making it easier to arrange the blocks correctly.

3. <b>Reset Functionality</b>: Users can reset the puzzle to its initial state, clearing all dropped blocks.

4. <b>Connection Detection</b>: Once the puzzle is solved by arranging the blocks in the correct order, the app detects the connections between the blocks and displays a list of connected images.

5. <b>Bluetooth Integration</b>: The app provides an option to connect to Bluetooth devices via the BluetoothHelper class, accessible through the app bar.


`bluetooth_helper.dart`
1. <b>Start Bluetooth Scan</b>: Initiates Bluetooth scanning in the Flutter app to discover available devices for connection.

2. <b>Permission Check</b>: Checks for location permission to utilize Bluetooth functionalities, requesting it from the user if not granted.

3. <b>Display Scanned Devices</b>: Presents scanned Bluetooth devices in a dialog, allowing users to select their desired device for connection.

4. <b>Display Connected Device</b>: If a device is already connected, displays its information in a dialog and provides an option to disconnect.

5. <b>Connection and Disconnection</b>: Attempts to establish a connection with the selected Bluetooth device and provides an option to disconnect from the connected device.

6. <b>Connection Status Notification</b>: Notifies the user of the success or failure of connection and disconnection operations via toast messages.


`bluetooth_communication.dart`
1. <b>Connection Establishment</b>: Establishes a connection with a Bluetooth device.

2. <b>Service and Characteristic Discovery</b>: Discovers services and characteristics of the connected Bluetooth device.

3. <b>Data Reception</b>: Subscribes to notifications for receiving data from the connected device.

4. <b>Data Transmission</b>: Sends data to the connected Bluetooth device.
