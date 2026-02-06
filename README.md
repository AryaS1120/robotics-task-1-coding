# robotics-task-1-coding
This is my task on coding domain.(primary)
For blinking of a LED using push button, first l have taken a breadboard and inserted pushbutton in it.(I didnt had pushbutton which can be inserted directly in breadboard, so l have 
attached two wires to it and then joined that wires to terminal of pushbutton and other end to breadboard.) Then l have taken 2 jumper wires(male to male), one of white color and one of 
black color,then I have attached black wire to 5V in Arudino UNO and I have attached white terminal to 6 number pin. Then l have attached 10k resistor to ground. Its imp to use resistor 
bcoz even without connecting pushbutton due to floating voltages Arudino considers it as input.Then we have connected a grey wire to GND in Arudino and other side on breadboard ground.
Then we will connect led on breadboard and attach green wire(-ve terminal) to ground on breadboard and red wire(+ve terminal) to pin 7 on Arudino.
The led bulb has 2 legs, shorter one is cathode(-) and longer one is anode(+).
In Arudino IDE code there are two imp functions void setup and void loop. We have considered white wire as 'a' so we will write in code integer 'a=6' and 'led=7'. Then in setup,
we declare which wires are input and output.So we write pinMode and give our pin number i.e. 6 and write its mode i.e.INPUT. Here we are going to use digitalRead bcoz we have to read
the pin. We will declare a 'var x' and assign digitalRead to 'x', then we will print it see the value. so we will use Serial.begin(9600) and Serial.println(x) to see output. we can see the
output on serial monitor, when we click on pushbutton it shows 1 continuously and when we again click on pushbutton it shows 0.After checking our basic code is working then we will write 
pinMode again in setup  for led as 7, output. For the switch to on and off on clicking we will use if-else condition like if x==0 so it should switch off so we will write 
digitalWrite(7,LOW) else (7,HIGH) and our coding part is done. Then we connect our USB and  compile it and upload it and LED will be blinking on our command!


#MECHANICAL DOMAIN LINK:-
https://gmail5868545.autodesk360.com/g/shares/SH90d2dQT28d5b602811bb761023be5c35aa


