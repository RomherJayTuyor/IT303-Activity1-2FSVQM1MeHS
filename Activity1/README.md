**IT303L - Activity 1**

NAME: Romher Jay M. Tuyor
GRADE AND SECTION: BSIT 2-B
STUDENT ID: 2410282-1
DEVICE CODE: 2FSVQM1MeHS

**Tinkercard Circuit Link**
https://www.tinkercad.com/things/2FSVQM1MeHS


**Arduino Code**
void setup() {
  pinMode(2, INPUT);
  pinMode(13, OUTPUT);


  digitalWrite(13, LOW);

  Serial.begin(9600);
}

void loop() {
  int buttonState = digitalRead(2);

  if (buttonState == HIGH) {
    digitalWrite(13, HIGH);
    Serial.println("Button: HIGH | LED: ON");
  } 
  else {
    digitalWrite(13, LOW);
    Serial.println("Button: LOW | LED: OFF");
  }

  delay(200);
}


**Screenshoots**
<img width="1147" height="839" alt="Screenshot 2026-10-03 002427" src="https://github.com/user-attachments/assets/1f9a53bf-c11f-4974-9572-70be681253c1" />
<img width="1165" height="912" alt="Screenshot 2026-10-03 002604" src="https://github.com/user-attachments/assets/1e1bb457-7e67-428a-9977-2f3f4c25ae2a" />

**Integration Map**
<img width="1536" height="2048" alt="5a347b7a-031e-4052-916f-71e778716e73" src="https://github.com/user-attachments/assets/efcaee18-a0ab-4c45-91df-d19b138df076" />

**Components**
Name,Quantity,Component
"D1",1,"Red LED"
"R1",1,"220 Ω Resistor"
"U1",1," Arduino Uno R3"
"S1",1," Pushbutton"
"1",1," Breadboard Small"
"R2",1,"10 kΩ Resistor"

**Explaination**
This System uses a push button as the input, Arduino as the controller, and an LED as the output. When the button is pressed,
pin 2 reads HIGH, so the Arduino turns the LED ON through pin 13. When the button is released, pin 2 reads LOW, so the LED turns-
OFF. The Serial Monitor reports both the button reading and the LED decision. This demonstrates the complete input, decision,output,
and reporting loop.












































