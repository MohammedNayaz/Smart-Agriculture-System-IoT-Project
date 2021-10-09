# Smart-Agriculture-System-IoT-Project
Internship Project at TEQUED LABS (Bangalore)


About TEQUED LABS
https://github.com/MohammedNayaz/Smart-Agriculture-System-IoT-Project/blob/main/About%20TEQUED%20LABS.txt


TASK PERFORMED:
PROBLEM STATEMENT 
Develop a smart agriculture dashboard to measure parameters like moisture, ph. level, sunlight and other such parameters and create a dashboard to display all parameters and also buttons for controlling water pumps.
Read More:
https://github.com/MohammedNayaz/Smart-Agriculture-System-IoT-Project/blob/main/PROBLEM%20STATEMENT.txt
 
Tools Used:
Software Tools

Arduino IDE

![image](https://user-images.githubusercontent.com/64147100/136645505-c1daa4d2-c656-472e-862b-1587c7b8acf3.png)

Blynk

![image](https://user-images.githubusercontent.com/64147100/136645575-6fdcf154-af09-4645-9da5-d91531356f04.png)

Read more:
https://github.com/MohammedNayaz/Smart-Agriculture-System-IoT-Project/blob/main/Software%20Tools

Hardware Requierd :

NodeMCU

![image](https://user-images.githubusercontent.com/64147100/136645611-b9739cfb-bc80-40c5-880e-acf2f1f5fd0a.png)

![image](https://user-images.githubusercontent.com/64147100/136645632-e9d711da-497f-43bc-9d06-5efd3113e891.png)

Soil Moisture Sensor

![image](https://user-images.githubusercontent.com/64147100/136645651-db356815-5090-4be9-a28b-2b6d8fc80252.png)

DHT11 Temperature-Humidity Sensor

![image](https://user-images.githubusercontent.com/64147100/136645665-cd5fc530-8826-4816-9b1b-8bce43f3286b.png)

Relay Module

![image](https://user-images.githubusercontent.com/64147100/136645684-eb319319-c356-42ef-b7ef-3533e5bf8844.png)

Solenoid Water Valve

![image](https://user-images.githubusercontent.com/64147100/136645694-bf7a9268-893c-4237-9eec-e8a0c27d0860.png)

Breadboard

![image](https://user-images.githubusercontent.com/64147100/136645716-65bb31a5-7e44-4b35-84ab-ba613353cd41.png)

Jumpers

![image](https://user-images.githubusercontent.com/64147100/136645732-01cdf8dd-94c9-4f49-b7b1-7eca25ae4133.png)

Battery of 9/12V

![image](https://user-images.githubusercontent.com/64147100/136645755-297489e7-405a-4d78-a931-0fc2e63cf590.png)

Read More: https://github.com/MohammedNayaz/Smart-Agriculture-System-IoT-Project/blob/main/Hardware%20Tools.txt


3.6 Methodology
3.6.1 Interfacing code for sensors and NodeMCU
code:
https://github.com/MohammedNayaz/Smart-Agriculture-System-IoT-Project/blob/main/smartAgri.ino
__________________________________________________________________________
 
Gauge setup in Blync app

Steps	Task Performed	Demonstration
1	•	Open the Blynk app 
•	click on New Project	 
2	•	Name the project as Smart Agriculture
•	Select the Board as ESP8266
•	Select the Theme
•	Click on Create	 
3	•	Auth Token will be sent to the registered Email ID
•	Click ok to land on work area	  
4	•	Select the Gauge (3), Button (1), Timer (1) from the Widget Box
•	Arrange the items as per your choice 	  
5	•	Click on Gauge to open Gauge Settings
•	Name the Gauge
•	Select the Input type
•	Select Font size
•	Select Reading Rate	   
6	•	Click on Timer & Button
•	Name them
•	Set the Input 
•	Set the Timer start & stop time	  
7	•	After uploading the code to the NodeMCU, Click on Play button
•	The reading of Soil moisture sensor, DHT11 sensor are updated
•	The solenoid valve will operate based on timer and also manually.	  

Circuit Connection Diagram


 
Final Connection Setup

Connection Procedure:
1.	Take a breadboard, NodeMCU, DHT11 temperature & Humidity sensor, Soil Moisture sensor, solenoid valve, 9volt battery and jumper wires.
2.	Connect the Node MCU to the breadboard at b16 – i16 x b30 – i30.
a.	Connect 3V3 to +(15) of breadboard.
b.	Connect GND to –(13) of breadboard.
3.	Connecting the DHT11 sensor to i3, i4, i5.
a.	Connect + of DHT11 to +(7) of breadboard.
b.	Connect out of DHT11 to D4 of NodeMCU.
c.	Connect – of DHT11 to –(7) of breadboard.
4.	Connecting Relay Module to NodeMCU
a.	Connect VCC of Relay Module to Vin of NodeMCU.
b.	Connect GND of Relay Module to GND of NodeMCU
c.	Connect IN of Relay Module to D0 of NodeMCU
d.	Connect the other end(screw) to the positive of the battery and to the solenoid valve in such a way that, the negative of the solenoid value must return to the negative of the battery.
5.	Connecting Soil Moisture Sensor to NodeMCU.
a.	Connect the VCC of Soil Moisture Sensor to the +(13) of breadboard.
b.	Connect the GND of Soil Moisture Sensor to the –(11) of breadboard.
c.	Connect the D0 of Soil Moisture Sensor to the D3 of NodeMCU.
d.	Connect the A0 of Soil Moisture Sensor to the D3 of NodeMCU.
6.	Now dip the Soil Moisture Sensor in to the agriculture land/plant pot and provide the water connection to the solenoid valve.
7.	Note down the Readings on the Blynk app.
 
CHAPTER 4
EXECUTIVE SUMMARY
IoT based SMART AGRICULTURE SYSTEM for Live Monitoring of Soil Moisture, Temperature and Humidity has been proposed using NodeMCU with some Sensors and Cloud Computing. The System has high efficiency and accuracy in fetching the live data of temperature and soil moisture. The IoT based smart farming System being proposed via this report will assist farmers in increasing the agriculture yield and take efficient care of food production as the System will always provide helping hand to farmers for getting accurate live feed of environmental temperature, humidity and soil moisture with more than 99% accurate results.
Tequed Labs understand this need to move beyond the brick-and-mortar inlet to future-proof business and out the right solutions and technologies to give you an edge over other competitors. They work to come up with a solution that best suits business model, size and customers. They expertise lies in having in-depth knowledge, vast experience and exposure in automating business processes, offering effective solutions to transform them into business objectives. They have an adept team with best of breed technologies to change the growth story of anyone’s business.
The work performed during my internship tenure was to build a smart agriculture dashboard to monitor soil moisture, temperature, humidity and such related things for the automation of agriculture where the land owner can easily keep track of the soil condition of his land and get notify if the water is to be supplied to the land when the moisture gets low in the soil. The Blynk app provide the best UI to monitor the agriculture land via gauges, timer and switches where the timer can be set to water the field automatically and can also be controlled manually. 


