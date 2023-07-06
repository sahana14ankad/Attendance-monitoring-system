# Attendance-monitoring-system
ABSTRACT:

Attendance Monitoring System deals with the maintenance of user’s attendance details . Here we have used RFID sensor . Each user will be provided with RFID tags which contains 12-digit unique code .Only if the user is present on that particular date and within time, the attendance will be considered . Once the RFID tag is scanned by the user the entry time, date, month will be recorded. We have used ThingSpeak cloud platform which is used to collect the data and store it in the cloud with advanced data analysis . Every time a user scans the card a tweet is sent.

INTRODUCTION:

Software called the Attendance Monitoring System was created to track daily attendance in schools, universities, institutes, and businesses. It makes it easier to get a specific user’s attendance data every day . This approach aids in assessing attendance eligibility standards. The intention behind creating an attendance monitoring system is to automate the manual process of taking attendance. The software’s ability to automatically generate reports at the session’s end or in between sessions is another reason for its development.

MOTIVATION:

We decided to make an attendance monitoring system to provide an efficient and accurate way to track and manage student attendance. The system can help teachers and administrators quickly identify which students are absent, late, or present in class, and can provide valuable information about student attendance patterns over time. Additionally, the system can generate reports that can be used to identify students who need additional support or intervention, and can provide administrators with valuable data for making decisions about school policies and procedures.

OBJECTIVES:

1. The purpose of the attendance monitoring software is to reduce the time
   that is consumed when attendance is taken manually.
2. Weekly and monthly attendance reports for the employee are produced.
3. When we scan RFID tag count of visitors and their name will be displayed on LCD.
4. At the same time, entry date , time and other details will be recorded in ThingSpeak cloud and tweet will be sent.

COMPONENTS REQUIRED:

1. EM18 RFID Reader Module
2. RFID Cards
3. NodeMCU-ESP8266
4. 16x2 Alphanumeric LCD
5. I2C module for LCD
6. Breadboard
7. Connecting Wires


1. NodeMCU-ESP8266:
   
NodeMCU firmware is a powerful platform for IoT applications. It contains all the functionality of the ESP8266, allowing the user to connect to her Wi-Fi
network, interact with the Internet, create and store data, and build powerful
applications. Based on a lightweight version of the Lua scripting language, it
is designed for developers familiar with the Arduino platform. The firmware
has an integrated function library that allows users to quickly and easily
create applications for their projects. The NodeMCU Development Board is
a great way to start programming the ESP8266. It’s cheap and feature-
packed, making it perfect for anyone looking to develop an IoT product. The
NodeMCU firmware is open source and can be easily modified to suit the
needs of any project. It’s also compatible with the Arduino IDE and other
popular development platforms, making it an ideal choice for developers of
all skill levels.


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/185a9917-4184-41ee-b529-8b745839828c)


2. EM18 Reader Module:

Radio waves are used by Radio frequency Identification (RFID), a wireless
identification technique, to detect the presence of RFID tags. RFID technology is used to identify the presence of persons, objects, etc., just like a bar
code reader. With bar code technology, we must hold the bar code in front of
the reader to optically scan it, however with RFID technology, we only need
to bring the RFID tags within reading distance. Bar codes can also become
distorted or illegible, which rarely happens with most RFID. RFID is utilised
in many different applications, such as an attendance system that provides
each person with a unique RFID tag to aid in identifying them and their
attendance. Many businesses utilise RFID to grant access to their authorised
staff.

Specifications:
• EM-18 operating voltage : +4.5V to +5.5V
• Current : 50mA.
• Can operate at low power and has integrated antenna.
• Temperature : 0ºC to +80ºC.
• Frequency : 125KHz.
• Communicating parameters : 9600bps.
• 12 digit code reading distance: 10cm, depending on TAG.


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/65ba197c-b0b9-4243-af5d-6fb73f9a8f1c)



3. 16x2 LCD Display with I2C Protocol :

Specifications :

• Display color: Blue back lit.
• Character size: 2.95 mm wide x 4.35 mm high.
• Character pixels: 5 W x 7 H.
• Voltage requirements: 5 V DC +/- 0.5V.
• Current requirements: 2 mA @ 5 V DC.
• Display capacity: 16 character x 2 row.




FUNCTIONAL BLOCK DIAGRAM:

Firstly , power supply is given to NodeMCU and RFID tag is scanned, then the number of visitors and visitor’s name will be displayed on LCD. Count of visitors and their details such as entry date , time , month will be sent to ThingSpeak. For every RFID based entry a tweet is sent to twitter account.


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/14b88bee-0298-4e67-8dfd-a3bf0c6fbdcd)



FLOW CHART:


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/c9f875b2-2a5d-4113-9c1b-763ff675cea9)


CIRCUIT CONNECTIONS AND STEPS TO CARRYOUT EXPERIMENTS:

• Connections as per shown in the figure.
• As we scan the RFID tag to the EM18 reader module it reads the 12
  digits code from the tag.
• After scanning the card the attendance is displayed in LCD and the
  entering time and date is stored.


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/dee7200c-e5de-4e6e-8f83-e19a3b207b8a)


RESULTS:

Each RFID card has 12- digit unique code. So when we scan the card we get the output in serial window as shown below. Copy this code and register it with the user's name in the code.


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/1122d644-f537-4b1e-868a-052ff34d98a5)


LCD Results:

![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/97e91471-b91a-4c6a-9d57-822817a8582b)


ThingSpeak results:

![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/a51d3712-57dd-4097-a764-8063cec65cae)


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/4b839fa2-5a14-4bda-98e2-322f2113d8c9)


Twitter Result:


![image](https://github.com/sahana14ankad/Attendance-monitoring-system/assets/136897959/e1f3cd71-479e-440b-8418-b079ef1098de)


CONCLUSION:

The IoT-based attendance monitoring system is very successful and reliable. It can be turned into an efficient and error-free attendance management system for schools, colleges, and other organizations. In our project, we have used RFID sensor. Each user will be provided with RFID tags which contains 12-digit unique code. Only if the user is present on that particular date and within time, the attendance will be considered. Once the RFID tag is scanned by the user the entry time, date, month will be recorded. We have used ThingSpeak cloud platform which is used to collect the data and store it in the cloud with advanced data analysis. Every time a user scans the card a tweet is sent. This system is easy to use and very convenient, making it a great choice for any organization. Thus, we have completed our project successfully.

FUTURE SCOPE:

The Internet of Things (IoT) is a growing technology that is being used more and more around the world. It allows us to have a more in-depth understanding of other cloud-based applications, as well as to develop enhanced solutions using technologies such as touch less sensing devices. The system can be improved by using face recognition technology to help calculate attendance percentages.



