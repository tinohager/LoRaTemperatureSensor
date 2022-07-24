# LDTS - LoRa Distributed Temperature Sensor
A distributed Temperature Sensor connected via LoRa with a Master Module with a WLAN connection.

The aim of this project is to record the temperatures of the individual units in a small apartment complex in order to obtain an overall picture of the heating and cooling performance. The sensor data of the slave modules are then sent via LoRa to the master module. This then forwards the data via WLAN to a cloud service. This means that each slave module does not have to have its own WLAN configuration.

![Housing printed](doc/housing-printed.png)

## LoRa

### RSSI
The Received Signal Strength Indication (RSSI) is the received signal power in milliwatts and is measured in dBm.
This value can be used as a measurement of how well a receiver can "hear" a signal from a sender.
The closer to 0 the better the signal is, RSSI `minimum is -120dBm`.

- `-30dBm` signal is strong
- `-120dBm` signal is weak


## Used Hardware

- [1x Heltec - WIFI LoRa 32 - V2.1](https://amzn.to/3NMaJKi)
- [1x AZDelivery GY-BME280 Temperature Sensor](https://amzn.to/3Aph1wp)
- [1x Prototype Board](https://amzn.to/3OXw8Bc)

## Used Software Packages

- [espressif - arduino-esp32](https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json)
  (httpclient is more up to date than like heltec)
- [sandeepmistry - arduino-LoRa](https://github.com/sandeepmistry/arduino-LoRa)
- [adafruit - Adafruit_BME280](https://github.com/adafruit/Adafruit_BME280_Library)
- [adafruit - Adafruit_SSD1306](https://github.com/adafruit/Adafruit_SSD1306)

## Housing

![Housing](doc/housing.png)
![Cover](doc/housing-cover.png)

## Sensor data targets

- https://www.datagekko.com
- https://iotplotter.com
- https://iotguru.live
- https://thingspeak.com
- https://thingsboard.io
