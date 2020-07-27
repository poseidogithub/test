# test
test para ver cómo fuciona esto

https://github.com/JsBergbau/MiTemperature2

me ha funcionado así

git clone https://github.com/JsBergbau/MiTemperature2.git
sudo apt install python3 bluez python3-pip
pip3 install bluepy


en domotiz añado un dummy (	Dummy (Does nothing, use for virtual switches only) Create Virtual Sensors)  en hardware
en devices añado un sensor de tempp y humedad, copio el IDX


sudo nano sendToDomoticz.py 
edito la dirección del server domoticz 192.168.1.100:8080
edito el idx del sensor creado

sudo python3 LYWSD03MMC.py -d A4:C1:38:C0:F3:DA -2p -p2 75 -o2 -4 -p1 33 -o1 -6 -b 5 --callback sendToDomoticz.py


more info: https://easydomoticz.com/forum/viewtopic.php?f=26&t=9535&p=78308&hilit=MiTemperature2&sid=6bb37a13941a529cff45f760a94c7324#p78308
