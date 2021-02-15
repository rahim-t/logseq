---
title: Bluetooth Low Energy
---

## Bluetooth
### https://en.wikipedia.org/wiki/Bluetooth#Pairing_and_bonding)https://en.wikipedia.org/wiki/Bluetooth
#### operates at frequencies between 2.402 and 2.480 GHz

#### based on low-cost transceiver microchips

#### power 4dBm ([2.5.mW](http://2.5.mw/)) means a range of approx. 10m

#### master/slave architecture

#### Bluetooth profiles GAP, GATT and ATT: [](https://en.wikipedia.org/wiki/Bluetooth#Pairing)https://en.wikipedia.org/wiki/List_of_Bluetooth_profiles

#### Bluetooth 2.1 incl. secure simple pairing (SSP)

#### Bluetooth 4.0 incl. Bluetooth Low Energy (BLE): https://en.wikipedia.org/wiki/Bluetooth_Low_Energy
##### can be powered by coin cells;

##### a.k.a "Bluetooth Smart Ready" for hosts resp. "Bluetooth Smart"
###### single-mode chips (only BLE protocol) cheaper than dual-mode chips (incl. classic bluetooth protocol)

## Bluetooth Low Energy Profiles for **Proximity sensing**
### https://en.wikipedia.org/wiki/Bluetooth_Low_Energy#Proximity_sensing 

### So-called "electronic-leash" applications are well suited to the long battery life possible for 'always-on' devices. Relevant application profiles include:
#### FMP — the "find me" profile — allows one device to issue an alert on a second misplaced device.

#### PXP — the proximity profile — allows a proximity monitor to detect whether a proximity reporter is within a close range. Physical proximity can be estimated using the radio receiver's RSSI value, although this does not have absolute calibration of distances. Typically, an alarm may be sounded when the distance between the devices exceeds a set threshold.

### **DONE**: check what authentication restrictions have to be (or can be) implemented in order to use FMP profile. See FMP Specification:

### [FMP_SPEC_V10.pdf](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fdb96aaf-e492-4735-ae9a-fc6e5a8d2caf/FMP_SPEC_V10.pdf)

### There are no specific restrictions for using FMP but the restrictions of the GAP (Generic Access Profile), which describes pairing and bonding.

## Bluetooth Protocols
### https://en.wikipedia.org/wiki/Bluetooth#Bluetooth_protocol_stack)https://en.wikipedia.org/wiki/Bluetooth#Bluetooth_protocol_stack

## (https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b4f9cc10-fed6-442f-8a71-e3d388573fd2/Untitled.png)
### https://s3.us-west-2.amazonaws.com/secure.notion-static.com/b4f9cc10-fed6-442f-8a71-e3d388573fd2/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45O3KS52Y5%2F20200819%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20200819T115044Z&X-Amz-Expires=86400&X-Amz-Signature=76d9b07ad21d00759edd4fc0b01d4f249dc615906f5e68765f1f68c4357f0e29&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22

### 

### Link Manager: system that manages establishing the connection between devices; responsible for the establishment, authentication and configuration of the link

### L2CAP (Logical Link Control and Adaptation Protocol): used to multiplex multiple logical connections between two devices

### Service Discovery Protocol (SDP): allows a device to discover services offered by other devices, and their associated parameters

### Radio Frequency Communications (RFCOMM) is a cable replacement protocol used for generating a virtual serial data stream.

## Broadcasting and Oberserving

## Core Specification Part C (GAP) Chapter 9 (OPERATIONAL MODES AND PROCEDURES – LE PHYSICAL TRANSPORT) p.2040 ff [](https://learn.adafruit.com/introduction-to-bluetooth-low-energy/gap)https://learn.adafruit.com/introduction-to-bluetooth-low-energy/gap

## Device Pairing

## See [](https://en.wikipedia.org/wiki/Bluetooth#Pairing)https://en.wikipedia.org/wiki/Bluetooth#Pairing
### Any Bluetooth device in discoverable mode transmits the following information on demand:[["Device name"]][["Device class"]][["List of services"]]
#### Technical information (for example: device features, manufacturer, Bluetooth specification used, clock offset)

### Any device may perform an inquiry to find other devices to connect to, and any device can be configured to respond to such inquiries.

### Use of a device's services may require pairing.

### Some devices can be connected/paired to only one device at a time, and connecting to them prevents them from appearing in inquiries

### Implementation: During pairing, the two devices establish a relationship by creating a shared secret known as a link key

### **"Legacy-Pairing":** Input of **PIN codes** on both devices (can be hard-coded)

### "Secure Simple Pairing" (SSP): uses a form of public key cryptography; 4 options[["Just works: no user interaction; except for maybe a prompt to the user to confirm the pairing process"]][["Numeric comparison: only if both devices have a display, and at least one can accept a binary yes/no user input"]][["Passkey Entry: one device needs a display and a the other needs a numeric keypad entry or two devices with numeric keypad entry"]]
#### Out of band (OOB): This method uses an external means of communication (e.g. NFC) to exchange some information used in the pairing process. Pairing is completed using the Bluetooth radio, but requires information from the OOB mechanism. See [](https://www.bluetooth.com/blog/bluetooth-pairing-part-5-legacy-pairing-out-of-band/)https://www.bluetooth.com/blog/bluetooth-pairing-part-5-legacy-pairing-out-of-band/ **DONE**: Check wether PIN or OOB is useful! - No, neither initiating nor responding device can ensure alone that OOB is done. Besides that, input of 128-bit TK is not supported by iOS/Android. See also [](https://medium.com/@kbabcockuf/bridging-the-gap-bluetooth-le-security-aab27232a767)https://medium.com/@kbabcockuf/bridging-the-gap-bluetooth-le-security-aab27232a767 __Passkey Entry can be extended by specifying the OOB Capability, which enhances initial security by generating a complete 128-bit TK input to the STK generation algorithm. However, neither Android nor iOS supports the OOB Capability for 128-bit TK input, so it is not an option here.__ and [](https://stackoverflow.com/questions/48859717/how-to-do-bluetooth-pairing-at-factory-time)https://stackoverflow.com/questions/48859717/how-to-do-bluetooth-pairing-at-factory-time __In fact LESC out of band with pre-shared key is quite complicated to archive because of the calculation of the oob payload is supposed to be a random number signed with private key, and this mechanism is implemented in the softdevice but not accessible. Thus we could either re-invent the wheel, or just decide that this computation is useless as evedrop of out-of-band is just impossible with pre-shared key. Also, LESC oob pairing is more calculation intensive for no benefits.__

## Pairing flow

## See [](https://www.bluetooth.com/blog/bluetooth-pairing-part-1-pairing-feature-exchange/)https://www.bluetooth.com/blog/bluetooth-pairing-part-1-pairing-feature-exchange/ and other parts

## ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ead16b3a-7b19-44bf-8e8e-7291cf04bba0/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ead16b3a-7b19-44bf-8e8e-7291cf04bba0/Untitled.png)

## **Phase 1:**
### Exchange of Pairing features (initiator and responder tell if they have keyboard, display resp. if they need Legacy Pairing (Bluetooth <2.1) or if they want (in case of Legacy Pairing) resp. need (in case of Secure Connection) OOB key-generation

## **Phase 2:**

## [](https://www.bluetooth.com/blog/bluetooth-pairing-part-2-key-generation-methods/)https://www.bluetooth.com/blog/bluetooth-pairing-part-2-key-generation-methods/
### unless the OOB key-generation method is chosen, the key will be generated by use of IO Capabilities

### exceptions: if both devices have MITM-flag not set, then "just works" is used

### note: one device cannot ensure OOB, but it can ensure IO-Capabilities method

### example for passkey-entry:  [](https://www.bluetooth.com/blog/bluetooth-pairing-passkey-entry/)https://www.bluetooth.com/blog/bluetooth-pairing-passkey-entry/

## **TODO** Check if this is possible: Goal: Beacon wants LE Legacy-Pairing (no SC-flag), no OOB-flag[["**Bluetooth beacon fakes having a display**" " " "(doesn't matter if DisplayOnly or DisplayYesNo)"] ["PIN is known to user (but not displayed on beacon, since there is no display)"]][["random PIN-number generator always gives back same PIN or"] ["**TK/k input for c1 function is set to a default PIN**" " " "when calculation Sconfirm (beacon is Slave) and Mconfirm; analogously for s1 function to calculate STK"]]
### Find me profile discovery is possible as soon as paired if and only if the pairing/key-generation was done with method passkey-entry (**and not in case of unauthenticated "just works") - the GAP-method just works should be ignored** Halfway **DONE** - see core specification p. 2065 (device in security mode 1; security level 3 or 4 prerequisites link-key with authentication)

### The master triggers alerting through find me profile; better: IAS immediate alert service (maybe an existing app)

## Other Files

## Bluetooth Specification: [](https://www.bluetooth.com/specifications/archived-specifications/)https://www.bluetooth.com/specifications/archived-specifications/

## Bluetooth Security Overview: Pairing, Authentication, Authorisation, Encryption,..[](https://www.toengel.net/studium/mm_and_sec/bluetooth.pdf)https://www.toengel.net/studium/mm_and_sec/bluetooth.pdf [](https://duo.com/decipher/understanding-bluetooth-security)https://duo.com/decipher/understanding-bluetooth-security[](https://www.digikey.com/eewiki/display/Wireless/A+Basic+Introduction+to+BLE+Security#ABasicIntroductiontoBLESecurity-PairingOverview:)https://www.digikey.com/eewiki/display/Wireless/A+Basic+Introduction+to+BLE+Security#ABasicIntroductiontoBLESecurity-PairingOverview: [](https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-121r1.pdf)https://nvlpubs.nist.gov/nistpubs/legacy/sp/nistspecialpublication800-121r1.pdf

## **TODO** check if iOS allows to configure Bluetooth-SMP Protocolls (e.g. in order to set OOB-key in app)

## Bluetooth Core Documentation:[](https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/CoreBluetooth_concepts/CoreBluetoothOverview/CoreBluetoothOverview.html#//apple_ref/doc/uid/TP40013257-CH2-SW17)https://developer.apple.com/library/archive/documentation/NetworkingInternetWeb/Conceptual/CoreBluetooth_concepts/CoreBluetoothOverview/CoreBluetoothOverview.html#//apple_ref/doc/uid/TP40013257-CH2-SW17 Wikipedia Articles: [](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy#Proximity_sensing)https://en.wikipedia.org/wiki/Bluetooth_Low_Energy#Proximity_sensing resp.[](https://en.wikipedia.org/wiki/Bluetooth_low_energy_beacon#Beacon_protocols)https://en.wikipedia.org/wiki/Bluetooth_low_energy_beacon#Beacon_protocols resp. Bluetooth/BLE-Introduction:[](https://electronics.howstuffworks.com/bluetooth.htm)https://electronics.howstuffworks.com/bluetooth3.htm [](https://www.eetimes.com/bluetooth-4-0-an-introduction-to-bluetooth-low-energy-part-i/)https://www.eetimes.com/bluetooth-4-0-an-introduction-to-bluetooth-low-energy-part-i/ Eddystone: [](https://developers.google.com/beacons/eddystone#full_support_for_eddystone)https://developers.google.com/beacons/eddystone#full_support_for_eddystoneAndroid beacon Library: [](https://altbeacon.github.io/android-beacon-library/)https://altbeacon.github.io/android-beacon-library/ Ibeacon:[](https://stackoverflow.com/questions/18906988/what-is-the-ibeacon-bluetooth-profile)https://stackoverflow.com/questions/18906988/what-is-the-ibeacon-bluetooth-profile
