# ECG-App
Establishes communcation between the PC and an ECG developement board from Corscience. The user has the the ability to change certain settings about what data the device will be sending and the ECG data will be displayed as a continuous graph in the app.

# Working
- Transmitting and receiving commands to and from the ECG device (Corscience EMB1)
- Establishing connection between PC and EMB
- Handshake procedure (getting product information about the device)
  - Manufacturer
  - Device name
  - License key
  - Hard- and software version
  - Serial number
  - Protocol version
  - SCM version
- Start and stop transmitting ECG data
- Error Handling
- GUI
