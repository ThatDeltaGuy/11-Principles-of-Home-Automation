# 11 Principles of Home Automation

## Introduction

This is a thought experiment turned rules. 
I set out thinking what the perfect smart home would look like if you had the ability to rewire the home or come up with any device that doesnt exist on the market currently, but still work within know laws of physics (transmission rates of mesh networks etc.)

I came up with these 11 rules, trying to remain as technology/named brand independant as possible. 
Below I've included a Glossary, the meanings are mostly self explanitory but I wanted to besure to be unambiguous. 
This list is by no means exhaustive and I'm still not happy with some of the wording but I'm still updating it here and there.

My goal is to help people see niches in the market and create new devices that currently dont exist, or help reviewers with a bit more of an objective rating of products.

### Glossary

| Phrase  | Meaning |
| ------------- | ------------- |
| Controller  | The main brain behind the smart home. Current examples include Home-Assistant, Hubitat etc.  |
| Hub  | A connection point between wired and wireless devices. Current examples include Zigbee, Z-Wave, Thread etc.  |
| Device  | Any controlling element, sensor, or interface within the house. A light switch, thermostat, plug socket etc.  |
| Smart Device  | Any device that can send information back to the controller or be controlled by the controller  |
| Dumb Device  | Any device that cannot send information back to the controller or be controlled by the controller  |
| Sub-system  | A self-contained simple controller/hub that can run things on its own and is focused on a specific task, but can link back to the main controller for over-riding control. Current examples include Tado, X-Sense, Ring Alarm etc.  |
| An automation  | An event driven set of instructions for controlling devices. They have also been called routines by several smart home manufacturers.  |

## Principle of Intuitiveness
_A smart home should be intuitive and shouldn't need new habits forming to use._

When all automations are set and honed in, people using the home should not be left confused as to how something works. 
They should not have to learn a new way to do something that doesn't come intuitively after explaining it to them. 
A good start is that home automation should not take away from the existing functionality of the home. 
Where there's a light switch, there's should always be a light switch, where there's a thermostat, there should always be a thermostat, unless it would make sense to move/remove it even in a non-smart home. 

## Principle of Inclusivity
_A smart home should be setup to make life easier for everyone who uses it._

It is important to remember that automations and smart home features will be used by all occupants of the home as well as guests, and therefore every smart home will, by necessity, be different. 
Some inhabitants may struggle with certain concepts that come easy to most, but as it's their home too, accommodations must be made. 
Voice should always be considered as a backup or secondary way of controlling things, as they require everyone to know specific commands. 

## Principle of Local Control
_Wherever possible, smart home devices should be controlled and managed locally, and have no dependency on the internet, or be locked to a specific hub._

If the internet connection to the home stops working, or a manufacturer goes out of business or just stops supporting a device, the device should still continue to work with full functionality. 
Devices that require setup/configuration before use should not be tied to a manufacturer's app and should be able to run through configuration via a 3rd party app, hub, or built in web server. 
A locally deployed Home automation server should be able to co-ordinate everything. It is important to note however that some device functionality may not be possible to replicate locally; weather alerts, music streaming etc.

## Principle of Reactivity
_A smart home should be able to predict the needs of its occupants_

Wherever possible, the use of sensors and other inputs should be used to automatically have things happen when the occupants require them, without any input from the occupants. 
Some manual input will always be required, but for the most part, a smart home should listen to changes within the home and react accordingly. 
For instance, motion sensors turning on lights, temperature sensors turning on the heating etc.

## Principle of Tactility
_Any regular manual interaction with the smart home should be carried out with physical buttons._

If regular manual interactions are required, such as turning on lights or plugs, wherever possible, it should be able to be carried out via physical buttons. 
For more complex interactions, a dedicated touch screen that requires no more than 3 presses to trigger the required action can be used. 
Smart homes and smart devices should not require an app for everyday use.

## Principle of Radio Quietness
_A smart home should be set up to emit as little radio noise as possible, where practical._

Due to the increasing amount of smart devices within the home, and the multiple sources of interference that can exist, wireless transmission of data should be kept to a minimum. 
When possible, smart devices with high bandwidth or high frequency transmissions should be wired via Ethernet or other cable. 
Wi-Fi should only be used for high bandwidth devices where wiring is impractical. 
For low bandwidth devices, whilst wired would be better, a low powered mesh network is usually much more practical.

## Principle of Low Maintainence
_A smart home should require as little maintenance as possible._

Home automations should not need tweaking or manual intervention on a regular or even semiregular basis. 
Smart devices should also require minimum interaction where maintenance is concerned. 
For instance using a mains connection rather than using a battery, using local network storage rather than an SD card, choosing a vacuum cleaner that auto empties into a dock rather than having to manually empty it every time.

## Principle of Security
_A smart home should be built ground up with security in mind._

Most smart devices are not built with security in mind, meaning that they can be easily compromised. 
Any sensitive devices should only be accessible internally or via a trusted and secure app (most manufacturers apps do not fall into the second category). 
Any Locks, cameras, etc, that would give access to your home, you should have absolute control over. 
Smart devices should only be connected to the internet if they absolutely require it. 
If the Device is wireless, a secure connection protocol should be employed, Bluetooth should be avoided for this very reason.

## Principle of Restoration
_Smart devices should be, within reason, repairable by at least 3rd party repair shops._

As more and more smart devices enter homes that are by definition more complicated than their dumb counterparts, it's going to become more important that they can be serviced and can have their service life prolonged. 
Preferably in home but, at least, by a 3rd party repair shop rather than relying on a manufacturer. 
For any device functionality that it is not possible to run locally, there should be a choice of service provider, rather than being locked to a single provider.

## Principle Of Retaining Functionality
_If a device loses connection to a hub or controller, it should still maintain any functionality that it's dumb counterpart would do._

If the network in the home goes down or if the controller, hub, or home server breaks or in some other way looses functionality, any devices should continue to work manually. 
Curtains should still be able to open normally, lights should still turn on with a manual switch etc. 

## Principle of Segregation
_Important systems should remain segregated, only talking to each other through a central hub_

If a function of the smart home, must function no matter the status of the rest of the smart home, it should be moved to a sub-system and operate as its own unit. 
For instance, a fire alarm system should be able to operate even if there's an issue with the main smart home controller. 
The main smart home controller should still be able to communicate with the individual devices, even if through a secondary hub. 
