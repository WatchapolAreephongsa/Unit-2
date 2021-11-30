```C++
// C++ code
//
void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
  Serial.begin(125000);
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  bool bit0 = true;
  bool bit1 = true;
  bool bit2 = true;
  int dec = 0;
	for(int k = 0; k<2; k+=1){
   	 bit2 =!bit2;    
  	  for(int j = 0; j<2; j+=1){
        bit1 =!bit1;
        for(int i=0; i<2; i+=1){
            bit0 =!bit0;
            Serial.print(dec);
            Serial.print("-");
            Serial.print(bit2);
            Serial.print(",");
            Serial.print(bit1);
            Serial.print(",");
            Serial.println(bit0);
            dec ++;
    }
   }
 }
}

```

# Output
0-0,0,0
1-0,0,1
2-0,1,0
3-0,1,1
4-1,0,0
5-1,0,1
6-1,1,0
7-1,1,1
