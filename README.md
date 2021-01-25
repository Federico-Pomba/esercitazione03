# esercitazione03


#define LED_1 5
#define LED_2 6
#define LED_3 9
#define LED_4 3
#define DELAY 1000
int temperatura=0;
void setup()
{
  pinMode(LED_1, OUTPUT);
  pinMode(LED_2, OUTPUT);
  pinMode(LED_3, OUTPUT);
  pinMode(LED_4, OUTPUT);
  pinMode(P1, INPUT);
  pinMode(P1, INPUT);
}

void loop()
{
  while(temperatura<=255 && temperatura>=0){
    do{
      int stato_pulsante =  digitalRead(P1);
      if(stato_pulsante==1)
        temperatura++;
      
   }while(temperatura>=63);
  analogWrite(LED1, 63);
 }       
