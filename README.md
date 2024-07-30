<!-- Please do not change this logo with link -->

<a target="_blank" href="https://www.microchip.com/" id="top-of-page">
   <picture>
      <source media="(prefers-color-scheme: light)" srcset="images/mchp_logo_light.png" width="350">
      <source media="(prefers-color-scheme: dark)" srcset="images/mchp_logo_dark.png" width="350">
      <img alt="Microchip Technologies Inc." src="https://www.microchip.com/content/experience-fragments/mchp/en_us/site/header/master/_jcr_content/root/responsivegrid/header/logo.coreimg.100.300.png/1605828081463/microchip.png">
   </picture>
</a>

# pic18f57q43-timer-toggle-led-callbacks-mcc

The [TIMER Toggle LED example](https://onlinedocs.microchip.com/v2/keyword-lookup?keyword=MCC.MELODY.EXAMPLES.RUNNING.TIMER.PIC16F18F.TOGGLE.LED&version=latest&redirect=true
), of the MCC Melody Timer Example Component, is used in the **Polled implementation**.  The LED on the PIC18F57Q43 Curiosity Nano is toggled, as well as a Debug IO, which can be used to verify the 100 ms period. 


<!-- This is where the introduction to the example goes, including mentioning the peripherals used -->

## MCC Melody Example Components
Example Components are a tight integration of learning material directly into MCC. This allows users to conveniently place configuration instructions side-by-side to the components they are configuring - [MCC Melody Example Components Introduction](https://onlinedocs.microchip.com/v2/keyword-lookup?keyword=MCC.MELODY.EXAMPLES&version=latest&redirect=true). 


![MCC Melody Example Components](images/GUID-ADDC2E58-F16C-46BD-A42F-D8FF02459622-high_12cm.png)


Completele projects, such as this one, avilable in [MPLAB® Discover](https://mplab-discover.microchip.com), or GitHub, are specific to a board and microcontroller. However, this project could be re-created following the steps in the example component, on a range of supported microcontrollers. Furthermore, the functionality of this example could be added to an existing project. 

To explore what an example component is, as well as the difference between example and implementation, see - [MCC Melody Example Components - The Basics](https://onlinedocs.microchip.com/v2/keyword-lookup?keyword=MCC.MELODY.EXAMPLES.BASICS&version=latest&redirect=true).

Example Components are related to [MCC Melody Design Patterns for Control Flow](https://onlinedocs.microchip.com/g/GUID-7CE1AEE9-2487-4E7B-B26B-93A577BA154E), which shows different standard ways to organize main.c and other application-level files, e.g., Polling-, Interrupt and Callback- or State Machine-Design Patterns. You may be familiar with each of these patterns, but...
- What support does MCC Melody provide for each?
- What are the recommended ways of building on the MCC Melody generated code? 

<!-- Any information about an application note or tech brief can be linked here. Use unbreakable links!
     In addition a link to the device family landing page and relevant peripheral pages as well:
     - [AN3381 - Brushless DC Fan Speed Control Using Temperature Input and Tachometer Feedback](https://microchip.com/00003381/)
     - [PIC18F-Q10 Family Product Page](https://www.microchip.com/design-centers/8-bit/pic-mcus/device-selection/pic18f-q10-product-family) -->

## Software Used

<!-- All software used in this example must be listed here. Use unbreakable links!
     - MPLAB® X IDE 5.30 or newer [(microchip.com/mplab/mplab-x-ide)](http://www.microchip.com/mplab/mplab-x-ide)
     - MPLAB® XC8 2.10 or a newer compiler [(microchip.com/mplab/compilers)](http://www.microchip.com/mplab/compilers)
     - MPLAB® Code Configurator (MCC) 3.95.0 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
     - MPLAB® Code Configurator (MCC) Device Libraries PIC10 / PIC12 / PIC16 / PIC18 MCUs [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
     - Microchip PIC18F-Q Series Device Support (1.4.109) or newer [(packs.download.microchip.com/)](https://packs.download.microchip.com/) -->

- MPLAB® X IDE 6.20.0 or newer [(MPLAB® X IDE 6.20)](https://www.microchip.com/en-us/development-tools-tools-and-software/mplab-x-ide)
- MPLAB® XC8 2.46.0 or newer compiler [(MPLAB® XC8 2.46)](https://www.microchip.com/en-us/tools-resources/develop/mplab-xc-compilers/xc8)

## Hardware Used

- PIC18F57Q43 Curiosity Nano [(DM164150)](https://www.microchip.com/en-us/development-tool/DM164150)
- Curiosity Nano Explorer [(EV58G97A)](https://www.microchip.com/en-us/development-tool/EV58G97A)

<!-- All hardware used in this example must be listed here. Use unbreakable links!
     - PIC18F47Q10 Curiosity Nano [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029)
     - Curiosity Nano Base for Click boards™ [(AC164162)](https://www.microchip.com/Developmenttools/ProductDetails/AC164162)
     - POT Click board™ [(MIKROE-3402)](https://www.mikroe.com/pot-click) -->

## Setup

All instructions required to re-create this example are listed below, under Configuration Instructions.   

![TIMER Toggle LED, Polled Implementation](images/TIMER_Toggle_LED_Polled_15cm.png)

Once you have loaded the project in MPLAB X IDE, you will also be able to find more information from Tooltips and links next to the instructions 
[![Tooltip and link](images/info-circle-fill.png "Change the values of these settings until the needed Requested Period is between the indicated min., max values.")](https://onlinedocs.microchip.com/v2/keyword-lookup?keyword=MCC.MELODY.CONFIGHELP.TIMER.PERIOD&version=latest&redirect=true) .


![Tooltips and contenxt help](images/HardwareSettings_RequestedPeriod.png)


<!-- Explain how to connect hardware and set up software. Depending on complexity, step-by-step instructions and/or tables and/or images can be used -->

## Operation

The image below shows the [TIMER Toggle LED example](https://onlinedocs.microchip.com/v2/keyword-lookup?keyword=MCC.MELODY.EXAMPLES.RUNNING.TIMER.PIC16F18F.TOGGLE.LED&version=latest&redirect=true
) running. The period of 100ms is verifyied using Debug GPIO on the MPLAB Data Visualizer. A PIC18F57Q43 Curiosity Nano is used.

Note: One could achieve this same functionality by adding the Timer Example component to a new or existing MCC Melody project, for one of the supported microcontrollers.  

![Running the Timer Toogle LED example](images/RunningTimerToggleLED_15cm.png)


Two vertical cursors are added to verify the timer frequency. See configuration instructions below.
 
![DataVisualizer config Timer Toggle LED](images/DataVisualizerConfigTimerToggle_LED_15cm.png)

A logic analyser can be used instead of Debug GPIO on the MPLAB Data Visualizer.

<!-- Explain how to operate the example. Depending on complexity, step-by-step instructions and/or tables and/or images can be used -->

## Summary

<!-- Summarize what the example has shown -->
For more example components, open the standalone content mangager in MCC ![CM_icon](images/CM_icon.png) . 

![Standalone_CM](images/MCC_ContentManager_Examples_18cm.png) 

