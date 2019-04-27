#include <DHT.h>  // library sensor DHT 

#define DHTPIN A0  //pin A0 untuk sensor ( input data )
#define DHTTYPE DHT11 //jenis sensor yang digunakan = DHT11
DHT dht(DHTPIN, DHTTYPE); //deklarasi pin dan jenis sensor 

int lampu_bahaya= 9; //pin 9 untuk lampu indikator bahaya
int lampu_aman=10; //pin 10 untuk lampu indikator aman
int sirine=11; //pin 11 untuk Buzzer

void setup() {
  dht.begin(); //program komunikasi atau setup untuk sensor DHT 
  pinMode(lampu_bahaya, OUTPUT); //mengatur lampu_bahaya sebagai OUTPUT
  pinMode(lampu_aman,OUTPUT); //mengatur lampu_aman sebagai OUTPUT
  pinMode(sirine,OUTPUT);// mengatur sirine sebagai OUTPUT
  Serial.begin(9600);
}

void loop() {
 // float kelembaban = dht.readHumidity(); //menyimpan nilai kelembapan pada variabel kelembaban
  float suhu = dht.readTemperature(); //menyimpan nilai suhu pada variabel suhu
  delay(200); //mengatur jeda waktu pembacaan sensor selama 200 milidetik
//  Serial.print("Kelembapan :"); //menampilkan tulisan ("Kelembapan : ")
//  Serial.print(kelembaban); //menampilkan nilai kelembaban pada Serial Monitor
//  Serial.print("%"); //menambahkan tanda (" % ")
  Serial.print(" "); //menambahkan spasi
  Serial.print(" "); //menambahkan spasi
  Serial.print("Suhu :"); //menampilkan tulisan ("Suhu : ")
  Serial.print(suhu); //menampilkan nilai suhu pada Serial Monitor
  Serial.print("*C"); //menampilkan tanda (" *C") = Derajat Celcius
  Serial.print(" "); //menambahkan spasi
  Serial.print(" "); //menambahkan spasi
  Serial.println(" "); //menambahkan spasi
  
    //logika kondisi if untuk indikator bahaya dan aman
 
/*  if ( kelembaban < 80.00){      //jika kelembaban lebih besar dari 80.00
     digitalWrite(lampu_bahaya, LOW);   //lampu_bahaya mati
     delay (10);
     digitalWrite(sirine, LOW);   //lampu_bahaya mati
     //delay (10);
     digitalWrite(lampu_aman,HIGH); //lampu_aman menyala
     delay(10);
         }

 else if( suhu < 30.00){         //jika suhu lebih besar dari 30.00 
     digitalWrite(lampu_bahaya, LOW);   //lampu_bahaya mati
     delay (10);
     digitalWrite(sirine, LOW);   //lampu_bahaya mati
     //delay (10);
     digitalWrite(lampu_aman,HIGH); //lampu_aman menyala
     delay(10);
         }
          
 else{                           //jika tidak   
     digitalWrite(lampu_bahaya, HIGH);  //lampu_bahaya menyala kelap - kelip
     delay (10);
     digitalWrite(lampu_aman,LOW);
     delay (10);
     digitalWrite(lampu_bahaya,LOW);
     delay (10);
     digitalWrite(sirine,HIGH);
     delay(10);
     digitalWrite(sirine,LOW);
     delay(10); 
        }  */
}
