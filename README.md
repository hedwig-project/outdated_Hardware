# Hardware
Hardware for Hedwig

## Basic Module
Basic Module for datalog using Blynk. Complete HW but simple communication.

Presence (cont in range 0 to 100);Temperature in ºC; Humidity in %; Brightness (0 to 102.4).

### ESP8266 Programming (usually NodeMCU or Wemos D1 R2)
http://blog.filipeflop.com/wireless/programar-nodemcu-com-ide-arduino.html

Link for ESP8266 library:http://download.igrr.me/versions/2.3.0/package_esp8266com_index.json

## Blynk
Getting Started Guide -> http://www.blynk.cc/getting-started

Documentation -> http://docs.blynk.cc/

Sketch generator -> http://examples.blynk.cc/

Latest Blynk library -> https://github.com/blynkkk/blynk-library/releases/download/v0.4.7/Blynk_Release_v0.4.7.zip

Latest Blynk server -> https://github.com/blynkkk/blynk-server/releases/download/v0.24.0/server-0.24.0.jar


Download App from Google Play

## Get Historical Data
LDR: http://blynk-cloud.com/token/data/V2

Umidade: http://blynk-cloud.com/token/data/V3

Temperatura: http://blynk-cloud.com/token/data/V4

Presença: http://blynk-cloud.com/token/data/V5


token: Receive in your email.

# MQTT Arduino Library Test (PubSub Client)
API Documentation: http://pubsubclient.knolleary.net/api.html

## For local test
Simply download web interface files and open index.html in your favorite browser.

## For LAN test
Upload the file MQTTcomESP8266_v004 to your Wemos R1 D2.
Save all web interface files to your Python folder in your computer (download and install from https://www.python.org/)
Execute in cmd: "python -m SimpleHTTPServer 8002" (you can change the port to 8080, 8000 or whatever you may need)

## For Internet test
Edit your router´s configuration to forward port 8002 (or the one you selected). For TP LINK, see http://www.tp-link.com.br/faq-72.html
Get to know your global IP address (for example, from https://whatismyip.com.br/)
Now, you can open the web interface which uses MQTT from anywhere by http://yourip:8002/
