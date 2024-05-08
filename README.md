## INTERFACING DIGITAL INPUT SENSOR WITH ARDUINO PUSH BUTTON

## NAME :DIVYA R																			             
## ROLLNUMBER :212222040040
## DEPARTMENT :CSE
## DATE :26.02.2024


## AIM:
To interface a digital input (push button) and blink and LED upon activation.
## COMPONENTS REQUIRED:
1.	1 KΩ Resistor 
2.	Arduino Uno 
3.	Bread board 
4.	USB Interfacing cable 
5.	Jumper wires 
6.	LED of choice 
## THEORY :
Arduino UNO
 	  The Uno is a microcontroller board based on the ATmega328P. It has 14 digital input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz quartz crystal, a USB connection, a power jack, an ICSP header and a reset button. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with a AC-to-DC adapter or battery to get started.
	Technical specifications of Arduino UNO :
Microcontroller	ATmega168/328
Microcontroller	ATmega168/328
Operating Voltage	5V
Input Voltage (recommended)	7-12V
Input Voltage (limits)	6-20V
Digital I/O Pins	14 (of which 6 provide PWM output)
Analog Input Pins	6
DC Current per I/O Pin	40 mA
DC Current for 3.3V Pin	50 mA
Flash Memory	16 KB (ATmega168) or 32 KB (ATmega328) of which 2 KB used by boot loader
SRAM	1 KB (ATmega168) or 2 KB (ATmega328)
EEPROM	512 bytes (ATmega168) or 1 KB (ATmega328)
Clock Speed	16 MHz
## PIN DIAGRAM FOR ATMEGA 328
 
![image](https://user-images.githubusercontent.com/36288975/163530394-115baee4-7ed1-49fe-9cce-d7b625e11e85.png)

![image](https://user-images.githubusercontent.com/36288975/163530431-4d390e98-0942-42d8-95b8-f57d348e6ad8.png)


## PROCEDURE 
 Open tinker cad account 
1.	Select Arduino uno , bread board , digital input and digital output 
2.	Connect the circuit as given in the figure 
3.	Develop the program and compile it for any errors 
4.	 .Execute the program 
5.	Check the simulation 



## CIRCUIT DIAGRAM 


![image](https://user-images.githubusercontent.com/36288975/163530437-87a0afbd-b3c9-44ad-b907-5de63486fb9d.png)
![Screenshot 2024-02-16 160917](https://github.com/divyadivya10/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/119560271/989770be-e4ee-4585-8eea-ead1ac60f800)









## PROGRAM 
```
int Led=3;
int pushbutton=4;
void setup()
{
  pinMode(Led, OUTPUT);
  pinMode(pushbutton,INPUT);
}

void loop()
{
  int pb;
  pb=digitalRead(pushbutton);
  if(pb==HIGH)
  {
  digitalWrite(Led, HIGH);
  delay(500); // Wait for 1000 millisecond(s)
  digitalWrite(Led, LOW);
  delay(500);
  }
  else
  {
    digitalWrite(Led, LOW);
  delay(1000);
  }
   
}
```
 
 









 
 
 



## OUTPUT OF SIMULATION :

[My image](username.github.com/repository/img/image.jpg)
![Screenshot 2024-02-19 100719](https://github.com/divyadivya10/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/119560271/b1fe2080-025c-4722-8ff8-dae506d7ed28)

![Screenshot 2024-02-16 155346](https://github.com/divyadivya10/-INTERFACING-DIGITAL-INPUT-SENSOR-WITH-ARDUINO-PUSH-BUTTON-/assets/119560271/1fae3996-c118-44e8-a2b4-e75a4a6a6196)

## RESULT:

Thus, we have interfaced a digital input (push button) and blink of LED upon activation.



