Project description

In this project, we are trying to monitor the Temperature and Humidity of a closed area like a Meeting/Conference room, Cabins, cubicles. So we have connected the temperature measurement sensor to the LCD screen with the help of an Arduino device. 

For this project, you need to download & install two libraries LiquidCrystal & DHT library. You can download those libraries from GitHub or directly from Arduino IDE 

Github links - 

LiquidCrystal - $ https://github.com/arduino-libraries/LiquidCrystal $ 

DHT - $ https://github.com/adafruit/DHT-sensor-library $ 

From Arduino IDE - 

\tGo to Sketch >Include Library >Manage Libraries . The Library Manager should open. Search for "DHT" on the Search box and install the DHT library from Adafruit. Now after that search for "LiquidCrystal" on the search box and install the LiquidCrystal library build by Ardunio, Adafruit. 

The LiquidCrystal library will be used for LCD Screen to print the output on LCD. To wire your LCD screen to your board, connect the following pins: 

LCD RS pin to digital pin 12 

LCD Enable(E) pin to digital pin 11 

LCD D4 pin to digital pin 5 

LCD D5 pin to digital pin 4 

LCD D6 pin to digital pin 3 

LCD D7 pin to digital pin 2 

LCD R/W pin to GND 

LCD VSS pin to GND 

LCD VCC pin to 5V 

LCD LED+ to 3.3V 

LCD LED- to GND 

DHT library will be used to get temperature and humidity from the DHT22 sensor. DHT Library gives temperature output in Celsius by default if you want to convert into Fahrenheit then change one line - 

	float air_temp = dht.readTemperature(true); 
