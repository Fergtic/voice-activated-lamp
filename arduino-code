const int lightPin = 8;





String serialData;



void setup() {

  // put your setup code here, to run once:



pinMode(lightPin, OUTPUT);

digitalWrite(lightPin, HIGH);

Serial.begin(9600);

Serial.setTimeout(10);

}



void loop()

{

    delay(50);    

}



void serialEvent(){

  serialData = Serial.readString();

  

  if(serialData[0] == '0')

  {

    digitalWrite(lightPin, HIGH);

    Serial.println("Off");

  }

  else if(serialData[0] == '1')

  {

    digitalWrite(lightPin, LOW);

    Serial.println("On");

  }

}
