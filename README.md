# ECG-App
Establishes communcation between the PC and an ECG development board from Corscience. The user has the the ability to change certain settings about what data the device will be sending and the ECG data will be displayed as a continuous graph in the app.

# Features
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
- Set options for R wave and pacer detection, buffersize, sampling frequency and more 
- Start and stop transmitting ECG data
- Information displayed: 
  - detected R waves (on/off)
  - detected pacers (on/off)
  - heart rate
  - received, broken, lost packages
  - RR interval
  - runtime
- Error Handling
- GUI
- Moving average filter integrated (on/off , window length = 30 at 1kHz and 15 at 500 Hz) (on/off)

# Implemented functions for:
- Encoding commands to be sent over USB connection
- Octet Stuffing (replacing a start or endflag within the message with the appropriate substitude, to prevent early termination of a response)
- Calculating checksum using CRC16-CCITT
- Seperating responses
- Decoding payload 
- Saving raw ECG data in .txt file
