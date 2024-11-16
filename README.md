# Indian-Automation-Challenge
![image](https://github.com/user-attachments/assets/a270379c-3793-44b4-bf87-d31b0bcb7357)

Home is where you find your mind at peace. A relaxing peaceful evening at home is one of life's greatest pleasures. What if a thief broke into your house and has a weapon and you're hiding under the bed to avoid being found, how would you alert security without giving away your location? To automate this and implement real-time surveillance of the home security, we came up with a raspberry pi project that can send abnormal images and warning messages through telegram and also receive remote instruction from the users. 

Component Required for Automated Security System
1. Raspberry Pi 4B+
2. Servo 
3. Piezo Buzzer
4. IR sensor
5. Pi Camera 5MP
6. Buck Converter
![image](https://github.com/user-attachments/assets/038ca377-1a44-4ad4-9a88-25e657c15974)


Automated Security System Circuit Diagram
![image](https://github.com/user-attachments/assets/aa6cdaac-d273-466c-bdbd-cde50efbf266)
As the circuit diagram shows, the Raspberry Pi is connected with the PIR Sensor, Buzzer Servo, and the Pi camera. Servo:- Signal is Connected to GPIO 17 and powered using an external power supply. Buzzer:- it is connected to GPIO 23 & GND. IR Sensor: - Out connected at GPIO 16 and powered using an external power supply. Pi Cam:- Direct connection to Raspberry Pi Board.


Automated Security System with Telegram Bot
When we were brainstorming on solving the alert issue, we pondered upon what is something that most people have with them all the time. And the most obvious answer was a smartphone. We decided to use telegram to implement our system as telegram has freely available application programming interfaces (APIs) to make bots that help collect data or automate things. We will use some more software and python libraries like Pycharm, Gsheets, Thonny IDE, Putty, WinSCP, Telegram. Python libraries : Opencv - cv2, Dlib, numpy, face_recognition, Rpi.GPIO, telepot, picamera, gspread, codecs, sys, oauth2client.service_account

Bot commands:-

/start: Initiates bot, sends a welcome message and a list of commands. /photo & /getinfo: If someone stands in front of the door, the IR sensor picks up this input and triggers the OpenCV code that runs the facial recognition algorithm and updates the output to google sheets. When the /photo command is activated it sends a picture of the camera output. Whereas when the /getinfo command is activated it displays a list of people that were detected in the past hour. /motion: Checks for presence of motion and returns a photo if true, or a message stating that no one is there if false. /buzzer: This command is used to sound an alarm in case of emergencies, where there is a fire/ burglary etc. The command triggers the buzzer function in the code and sets the GPIO pin to high which rings the buzzer. /opengate & /closegate: These commands set the angle of the servo motors accordingly to open and close the gate.

Hardware Specification for Automated Security System

Raspberry Pi 4B+: The Raspberry Pi 4 B is equipped with Latest High-Performance Quad-Core 64-bit Broadcom 2711, Cortex A72 processor clocked at 1.5GHz speed. Taking this processing power and computational speed into consideration we settled with the Raspberry Pi 4B+ for our project.

IR sensor: Infrared sensors are nowadays commonly employed in motion detectors, which are utilized in security systems to detect visitors. The sensor elements detect heat radiation (infrared radiation) that changes over time and space owing to people's movement within a predetermined angle range.

Servo: Despite its size, it generates quite the amount of power and is known to be incredibly energy-efficient, and hence we decided to use it to open/close gates.

Piezo buzzer: Because the piezoelectric buzzer is controlled by electronic circuits, it can produce a variety of pleasant sounds and analog sound, intermittent sound. Pure timbre, not easily covered by noise. With it being lightweight, simple construction, and low-cost it was instantly our choice.

PiCamera: The Pi camera module is a portable lightweight camera that supports Raspberry Pi. It is one of the best choices in surveillance projects.

Buck Converter: It helps to convert a high voltage to a low voltage.

Conclusion
With the world changing and becoming more corrupt day by day, having just a security guard to protect your family and your house isn't enough. So, this automated security system will help to alert you on your phone and you can make a way to make safe your home and office. I hope you liked this project and learned something new. If you have any questions regarding the article, you can leave them in the comment or you can use our Electronics Forum


Refer to the website: https://circuitdigest.com/microcontroller-projects/automated-security-system-with-telegram-bot-and-facial-recognition

Video:
https://youtu.be/4QxZYN25Ieg
<iframe width="562" height="316" src="https://www.youtube.com/embed/4QxZYN25Ieg" title="Automated Security System with Telegram Bot &amp; Facial Recognition" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Contributors:
Het Patel
K S Vikash
Siddharth Ramanathan
Swaathy Kumar
Surjyabho Deb
