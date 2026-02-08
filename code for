#define BLYNK_TEMPLATE_ID "TMPL3DhohGZkt"
#define BLYNK_TEMPLATE_NAME "SMART HELMET FOR COAL MINNING"
#define BLYNK_AUTH_TOKEN "7L13anZODkltX8C8NK3wlzG4G-2d2baN"
#include<Servo.h>
Servo servo;
#define BLYNK PRINT Serial
#include <ESP8266WiFi.h>
#include <BlynkSimpleEsp8266. h>
//LiquidCrystal_I2C lcd(0x27, 16, 2)
#include "DHT.h"
#define DHTPIN D4
// GPIO2
#define DHTTYPE DHT11
// DHT11 sensor
DHT dht (DHTPIN, DHTTYPE) ;
const int sensor = A0;
float tempc; //variable to store temperature in degree Celsius
float tempf; //variable to store temperature in Fahreinheit
float vout, VIB, i = 0.834, tvoltage;
char auth [] = BLYNK_AUTH_TOKEN;
char ssid[] = "Pradeep"; // type your wifi name
char pass [] = "12345678"; // type your wifi password
int t, h, button = D8;
char auth[] = BLYNK_AUTH_TOKEN;
char ssid[] = "Pradeep"; // type your wifi name
char pass[] = "12345678"; // type your wifi password
int t, h, button = D8;|
BlynkTimer timer;
void sendSensor ()
{
int gas = analogRead (A0) ;
float h = dht.readHumidity();
float t = dht.readTemperature (); // Celsius
Blynk.virtualWrite (V2, gas);
Blynk.virtualWrite(V0, t);
Blynk.virtualWrite (V1, h);
int b_state = digitalRead(D8) ;
if (b_state == 1)

{

Blynk.virtualWrite (V5, "EMERGENCY");
Blynk. virtualWrite (V6, "SAVE ME");
} else
{
Blynk. virtualWrite (V5, " SMART ");
Blynk. virtualWrite (V6, " HELMET");
delay(5000);
if(t>100) {
Blynk. virtualWrite (V5, "HIGH");
Blynk. virtualWrite (V6, "TEMPERATURE");
Jelse{
Blynk.virtualWrite (V5, "NORMAL");
Blynk.virtualWrite (V6, "TEMPERATURE");
delay(5000) ;
if (gas>700) {
Blynk.virtualWrite (V5, "POISNOUS") ;
Blynk.virtualWrite (V6, " GAS");
Jelse{
Blynk.virtualWrite (V5, "INHALING");
Blynk. virtualWrite (V6, " GAS");
delay(5000) ;
}
void setup() {
Serial.begin (9600);
Blynk. virtualWrite (V5, "POISNOUS");
Blynk.virtualWrite (V6, " GAS");
}else{
Blynk.virtualWrite (V5, "INHALING");
Blynk.virtualWrite (V6, " GAS");
delay(5000);
}
}
void setup() {
Serial.begin (9600) ;
dht.begin();
Blynk.begin (auth, ssid, pass);
pinMode (D8, INPUT);
pinMode (D2, OUTPUT) ;
timer.setInterval(2500L, sendSensor);
}
void loop()
{
  Blynk.run();
timer.run();
}
