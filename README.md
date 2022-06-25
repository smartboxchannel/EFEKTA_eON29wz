# EFEKTA_eON29wz
Zigbee Indoor climate sensor EFEKTA_eON29wz with e-ink display

It's a compact wireless devices, atmospheric pressure, temperature, humidity, weather forecaster, illumination, charts with 2.9" e-paper display, resolution of 296 x 128 pixels. It works in automation systems Home Assistant, OpenHAB, ioBroker, MajorDoMo via Zigbee2mqtt and ZHA.
The device has an industrial look, at least I wanted to achieve this. 
The sensor has good energy efficiency. Powered by CC2530 chip (Zigbee), works with **Zigbee2mqtt, ZHA**.

### You can buy a ready-made device by writing to the mail hello@efektalab.com

### Delivery is carried out worldwide.

## You can make your own pcb here - https://www.pcbway.com/setinvite.aspx?inviteid=550959


#### Sale: 

#### Video:

#### zigbee2mqtt.io/supported-devices: https://www.zigbee2mqtt.io/supported-devices/#s=efekta

#### Telegram DiyDev - https://t.me/diy_devices

More info at http://efektalab.com/eON29wz

---

![Zigbee Indoor climate sensor EFEKTA_eON29wz with e-ink display]([https://github.com/smartboxchannel/EFEKTA_eON213z/blob/main/IMAGES/002.jpg](https://github.com/smartboxchannel/EFEKTA_eON29wz/blob/main/Images/photo_2022-06-24_20-59-10%20(2).jpg)) 
#### Technical specifications

● Model: eON29wz

● Display: E-ink display, size 2.9 inches.

● Battery: AAA X2 (not included)

● Wireless Protocol: Zigbee

● Dimensions: 99 × 43 × 12 mm

● Temperature range and accuracy: 0℃~ +50°C, ±0.3℃

● Humidity range and accuracy: 0 - 100% relative humidity (non-condensing), ± 3%

● Atmospheric Pressure range and accuracy: 30 kPa-110 kPa ± 0.12 kPa



#### Main Features

° ZigBee wireless connection, no wiring required

° Monitors temperature, humidity and atmospheric pressure in real time.

° Remote monitoring: When the indoor temperature reaches a certain threshold above or below, the EFKTA eON29wz  sensor can send an alert to your Smart Home system or send a command to other devices.

°  Home Automation: The EFKTA eON29wz temperature and humidity sensor can control other connected devices directly, such as a cordless outlet, to make sure that your fan or humidifier maintains a constant level of comfort for you and your family.

° Accurate measurement: Uses a high-quality sensor from industry-leading manufacturers Sensirion and Bosch.

° Built-in air pressure sensor: monitors the ambient air pressure in the rain, makes the calculation of the weather forecast.


### How to flash the device

1. Download the Smart RF Flash Programmer V1 https://www.ti.com/tool/FLASH-PROGRAMMER

2. Open the application select the HEX firmware file

3. Connect the device with wires to CCDebugger, first erase the chip, then flash it.

---

### How to install IAR

https://github.com/ZigDevWiki/zigdevwiki.github.io/blob/main/docs/Begin/IAR_install.md

https://github.com/sigma7i/zigbee-wiki/wiki/zigbee-firmware-install (RU)

---

### How to join:
#### If device in FN(factory new) state:
##### one way
1. Open z2m, make sure that joining is prohibited
2. Insert the battery into the device
3. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
4. Go to the LOGS tab
5. Press the reset button on the device (the join procedure will begin, еhe device starts flashing the LED repeatedly)
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times

##### another way
1. Open z2m, make sure that joining is prohibited
2. Insert the battery into the device
3. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
4. Go to the LOGS tab
5. Press and hold button (1) for 2-3 seconds, until device start flashing the LED repeatedly
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times


#### If device in a network:
##### one way 
1. Hold button (1) for 10 seconds, this will reset device to FN(factory new) status 
2. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
3. Go to the LOGS tab
5. Press and hold button (1) for 2-3 seconds, until device start flashing the LED repeatedly
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times

##### another way
1.Find the device in the list of z2m devices and delete it by applying force remove
2. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
3. Go to the LOGS tab
4. Press the reset button on the device (the join procedure will begin, еhe device starts flashing the LED repeatedly)
5. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times

![Efekta THP_LR \ THP](https://github.com/smartboxchannel/EFEKTA_eON213z/blob/main/IMAGES/003.jpg) 

### Troubleshooting

If a device does not connect to your coordinator, please try the following:

1. Power off all routers in your network.
2. Move the device near to your coordinator (about 1 meter).
or if you cannot disable routers (for example, internal switches), you may try the following:
2.1. Disconnect an external antenna from your coordinator.
2.2. Move a device to your coordinator closely (1-3 centimeters).
3. Power on, power on the device.
4. Restart your coordinator (for example, restart Zigbee2MQTT if you use it).

If the device has not fully passed the join

1. If the device is visible in the list of z2m devices, remove it by applying force remove
2. Restart your coordinator (for example, restart Zigbee2MQTT if you use it).
3. Click on the icon in z2m - allow joining (you have 180 seconds to add the device)
4. Go to the LOGS tab
5. Press and hold button (1) for 2-3 seconds, until device start flashing the LED repeatedly
6. Wait, in case of successfull join, device will flash led 5 times, if join failed, device will flash led 2 times



### Other checks

Please, ensure the following:

1. Your power source is OK (a battery has more than 3V). You can temporarily use an external power source for testings (for example, from a debugger).
2. The RF part of your E18 board works. You can upload another firmware to it and try to pair it with your coordinator. Or you may use another coordinator and build a separate Zigbee network for testing.
3. Your coordinator has free slots for direct connections.
4. You permit joining on your coordinator.
5. Your device did not join to other opened Zigbee network. When you press and hold the button, it should flash every 3-4 seconds. It means that the device in the joining state.
