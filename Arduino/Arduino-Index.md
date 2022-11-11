## to include lip 
	in main
```c++
//include <lipName.h>
#include <Servo.h>
```

## to create an object from lip
	in main 
```c++
Servo servo;
```

## to define pin name
	in main
```c++
//#define pinName pinNumber
#define led 13  // led in pin 13
```

## to define pin input or output
	in the setup funiction
```c++
//pinMode(pinName,input or output);
pinMode(A0,INPUT);
pinMode(2,OUTPUT);
```

## to print the output 
```c++
  //Initialize serial and wait for port to open
  Serial.begin(9600);
//to print  
 Serial.println("WiFi shield not present");//new line
 Serial.print("Attempting to connect to SSID: ");//same line
```

## to attach the lip to pin 
	in the setup funiction 
```c++
//servo.attach(pin number);
servo.attach(9);
```

## to move the servo 
	in the loop function
```c++
//servo.write(servoangel);
servo.write(0);
```

## add delay
	in the loop function
```c++
//delay(time in milsec);
delay(1000);//1sec
```

## name variable 
	in main 
```c++
//int varName =  Intger val ;
int pos=0;
//float varName = Float val ;
float voult = 0.0 ;
//boolean varName = Boll val ;
bool dataOn = true ; 
//string varName = String val ;
string myName = 'elsayed';
//arry varNamr = Array val;
array MyArr = [a,2,f];
//void varName = Void val ;
void myFunc(){};
```

## for loop
```c++
//for(what){do}
for(pos=0; pos<=180; pos++){
servo.write(pos);
delay(500);// 1\2 sec delay
} 
```

## Read analog pin 
```c++
//analogRead(potPin);
int reading = analogRead(A0);
```

## map to value to other value 
```c++
//map(FirstValue Start,FirstValue End,SecondValue Start,SecondValue End);
int angle = map(0,1023,0,180);
```

## IF condition 
```c++
// if(condition){do}
if(pos<=180){
servo.write(pos);
}
else{
servo.write(-pos);
}
```

## Switch Case
```c++
// switch (condition){
// case conditionValue :
//     Do;
//     break; 
// default:
//    Do;
//}
switch (data){
	case 1:
		data++;
		break; // to stop in this case if data = 1.
	case 2:
		data--;
		break; // to stop in this case if data = 2.
	default:
		data=3; // if no case match .
}
```

## While condition 
```c++
//while(condition){do}
while(pos<=180){
servo.write(pos);
}
```

## add string to string
```c++
//str1 += str2
"hi" += "elsayed";
```

## to open pin or close pin
```c++
//digitalWrite(pinName, low or high);
digitalWrite(2,HIGH);//to opne
digitalWrite(2,LOW);//to close
```

