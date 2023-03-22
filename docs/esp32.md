# ESP32 + BioAmp EXG Pill

 
[Espressif's ESP32](https://www.espressif.com/en/products/socs/esp32) is a feature-rich MCU with integrated Wi-Fi and
Bluetooth connectivity for a wide-range
of applications. It's 12bit ADC input is bit noisy but, can easily be coupled with the BioAmp EXG Pill to record ECG, EMG, EOG, and EEG. To make things work you need to create a voltage divider using 2.2k and 1k just like shown in the connection diagram below and flash the [Fixed Sampling](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/blob/main/software/FixedSampling/FixedSampling.ino) on to your ESP32 development board. 

![](ESP32-Basic-Circuit.png)

Using the exact setup and [BioAmp EXG Pill example arduino sketches](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/tree/main/software) you can easily do [Electromyography](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/electromyography-emg-walkthrough), [Electrocardiography](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/supportive-technology), [Electrooculography](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/electrooculography-eog-walkthrough), and [Electroencephalography](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/electroencephalography-eeg-walkthrough).

## **TECHNICAL SPECIFICATION**

|Features|             |   
|----------------------|:-------------------|       
|Wireless connectivity |150.0 Mbps data rate|
|Bluetooth | BLE (Bluetooth Low Energy) and Bluetooth Classic|
|Processor | 32-bit LX6 microprocessor|
|ROM | 448 KB|
|SRAM | 520 KB|

## Electromayograph
To make an Electromayograph for recording EMG signals using Espressif's ESP32 and BioAmp EXG Pill follow the circuit in the image below, flash the [EMG filter arduino sketch](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/blob/main/software/EMGFilter/EMGFilter.ino) onto your ESP32 development board and open up the serial plotter of your Arduino IDE.

![](ESP32-Electromyography.png)

Checkout [the Electromyography (EMG) Walkthrough project update](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/electromyography-emg-walkthrough) for information about EMG filtering, envelop detection, servo control, and LED-bar control, as well as an exciting project demo that relies on EMG data recorded with BioAmp EXG Pill.

## Electrocardiograph

To make an Electrocardiograph for recording ECG signals using Espressif's ESP32 and BioAmp EXG Pill follow the circuit in the images below, flash the [ECG filter arduino sketch](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/blob/main/software/ECGFilter/ECGFilter.ino) onto your ESP32 and open up the serial plotter of your Arduino IDE.

![](ESP32-Electrocardiography-Lead1.png)
![](ESP32-Electrocardiography-Hand.png)


Checkout [the Supportive Technology project update](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/supportive-technology) for information about ECG filtering and heart-beat detection, and more on ECG recording, with BioAmp EXG Pill.

## Electrooculograph

To make an Electrooculograph for recording EOG signals using Espressif's ESP32 and BioAmp EXG Pill follow the circuit in the images below, flash the [EOG filter arduino sketch](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/blob/main/software/EOGFilter/EOGFilter.ino) onto your ESP32 and open up the serial plotter of your Arduino IDE.

![](ESP32-Electrooculography-Vertical.png)
![](ESP32-Electrooculography-Horizontal.png)

Checkout [the Electrooculography (EOG) Walkthrough project update](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/electrooculography-eog-walkthrough) for information about EOG filtering and eye-blink detection, and more on EOG recording, using BioAmp EXG Pill.

## Electroencephalograph

To make an Electroencephalograph for recording EOG signals using Espressif's ESP32 and BioAmp EXG Pill follow the circuit in the image below, flash the [EEG filter arduino sketch](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/blob/main/software/EEGFilter/EEGFilter.ino) onto your ESP32 and open up the serial plotter of your Arduino IDE.

![](ESP32-Electroencephalography.png)

Checkout [the Electroencephalography (EEG) Walkthrough project update ](https://www.crowdsupply.com/upside-down-labs/bioamp-exg-pill/updates/electroencephalography-eeg-walkthrough) for information about EEG filtering, and more on EEG recording, with BioAmp EXG Pill.


# Blink eye to click photos over bluetooth and more!

A lot of awesome projects can be made with this setup, like [EOG based photo clicker over BLE](https://github.com/upsidedownlabs/BioAmp-EXG-Pill/blob/main/software/EOGPhotoCaptureBLE/EOGPhotoCaptureBLE.ino) created by [Padmalaya Rawal](https://www.linkedin.com/in/padmalayarawal/) of [PR Robotics](https://www.youtube.com/PRROBOTICS). A new [T Rex Game](https://t-rex-game.com/) controller can also be created by detecting Eye blinks and sending spacebar signal over BLE to your Laptop or PC. Possibilities are endless and we are very excited to watch what you will be making with yor own BioAmp EXG Pill. In the coming project update(s) we will be enabling our ESP32 + EXG setup to connect mobile/laptop to show a user interface for visualization of the BioPotential signals and more.

# EMG monitoring BioAmp EXG Pill (review)

Recently a pretty awesome video has been published by [EDISON SCIENCE CORNER on YouTube](https://www.youtube.com/watch?v=qrb8LeRfkP4) on BioAmp EXG Pill in which he talked about EMG monitoring using BioAmp EXG pill and Arduino. He did a pretty good job in clearly showing how you have assemble the BioAmp EXG Pill for the first time and then how you can use it to record EMG signals.

YouTube: https://www.youtube.com/watch?v=qrb8LeRfkP4

##### That was all for this Project update, Look out for more awesome project updates :)
