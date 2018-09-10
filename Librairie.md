# M.A.R.K : la librairie ! 

## Les fonctions
Général  : <br />
* [MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid)
* [~MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid-1) 
* [begin(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#beginvoid)
    
Moteurs :

* [setLeftMotor(int _speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setleftmotorint-_speed)
* [setRightMotor(int _speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setrightmotorint-_speed)
* [stopLeftMotor(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#stopleftmotorvoid)
* [stopRightMotor(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#stoprightmotorvoid)

LCD RGB : 

* [setLcdRGB(unsigned char r, unsigned char g, unsigned char b)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setlcdrgbunsigned-char-r-unsigned-char-g-unsigned-char-b)
* [lcdPrint(String text)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#lcdprintstring-text)
* [lcdPrint(float data)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#lcdprintfloat-data)
* [setLcdCursor(uint8_t, uint8_t)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setlcdcursoruint8_t-uint8_t)
* [lcdHome(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#lcdhomevoid)
* [lcdClear(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#lcdclearvoid)

Barre de leds : 

* [setLedBarLevel(int level)]()
* [getLedBarLevel(void)]()

Capteur de réflectance infrarouge : 

* [gedInfrared(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#gedinfraredvoid)

Diviseur de tension : 

* [getVoltage(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getvoltagevoid)
* [getBatteryLevel(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getbatterylevelvoid)

Ultrason : 

* [getUsDist(String _pos)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getusdiststring-_pos)

Capteur de contact : 

* [getBumper(String _side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getbumperstring-_side)
* [getInterruptFlag(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getinterruptflagvoid)
* [resetInterruptFlag(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#resetinterruptflagvoid)

Joystick : 

* [getJoystickY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickyvoid)
* [getJoystickX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickxvoid)
* [getJoystickClic(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickclicvoid)

Servomoteur : 

* [setServo(int)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setservoint)
* [getServo(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getservovoid)

Accéléromètre : 

* [getAccelX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getaccelxvoid)
* [getAccelY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getaccelyvoid)
* [getAccelZ(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getaccelzvoid)
* [getGyroX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getgyroxvoid)
* [getGyroY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getgyroyvoid)
* [getGyroZ(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getgyrozvoid)
* [getTemp(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#gettempvoid)

Wifi : 

* [sendWifiCmd(char *cmd)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#sendwificmdchar-cmd)
* [waitWifiResult(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#waitwifiresultvoid)
* [displayWifiAnswer(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#displaywifianswervoid)

Encodeurs : 

* [getEncoder(String _side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getencoderstring-_side)
* [resetEncoder(String _side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#resetencoderstring-_side)

---

#### MARK(void)
Constructeur. 
##### Paramètres :
Aucun.
##### Valeur de retour :
Aucune.
##### Exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class
```

---

#### ~MARK(void)
Destructeur.
##### Paramètres :
Aucun.
##### Valeur de retour :
Aucune.


---

#### begin(void)
Initialisation de la classe (Serial, I2C, encodeurs etc)
##### Paramètres :
Aucun.
##### Valeur de retour :
bool : égale à 1 si la fonction se termine bien.
##### Exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  //nothing
}

```

---

#### setLeftMotor(int speed)
Configure la vitesse du moteur gauche.
##### Paramètres : 
- speed : vitesse du moteur ( entre -100 et 100 , 0 arrête le moteur).
##### Valeur de retour : 
Aucune.
##### Exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setLeftMotor(-50);
  delay(1000);
  myrobot.stopLeftMotor();
  myrobot.stopRightMotor();
  delay(1000);
}

```

---

#### setRightMotor(int speed)
Configure la vitesse du moteur droit.
##### Paramètres : 
- speed : vitesse du moteur ( entre -100 et 100 , 0 arrête le moteur).
##### Valeur de retour : 
Aucune.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setLeftMotor(-50);
  delay(1000);
  myrobot.stopLeftMotor();
  myrobot.stopRightMotor();
  delay(1000);
}

```

---

#### stopLeftMotor(void)
Stop le moteur gauche.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
Aucune.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setLeftMotor(-50);
  delay(1000);
  myrobot.stopLeftMotor();
  myrobot.stopRightMotor();
  delay(1000);
}

```

---

#### stopRightMotor(void)
Stop le moteur droit.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
Aucune.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setLeftMotor(-50);
  delay(1000);
  myrobot.stopLeftMotor();
  myrobot.stopRightMotor();
  delay(1000);
}

```

---

#### setLcdRGB(unsigned char r, unsigned char g, unsigned char b)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
- r : valeur de la composante rouge (entre 0 et 255).
##### Valeur de retour : 
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setLcdRGB(255,0,0); //red
  delay(1000);
  myrobot.setLcdRGB(0,255,0); // green
  delay(1000);
  myrobot.setLcdRGB(0,0,255); // blue
  delay(1000);
}
```
---

#### lcdPrint(String text)
Affiche le texte à la position du curseur.
##### Paramètres : 
- text : chaîne de caractères à afficher (type String).
##### Valeur de retour : 
Aucune.
##### exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setLcdCursor(0,0);
  myrobot.lcdPrint("Hello World !"); 
  delay(1000);

}
```

---

#### lcdPrint(float data)
Affiche le nombre à la position du curseur.
##### Paramètres : 
- data: nombre (type float).
##### Valeur de retour : 
Aucune.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

int i = 0;
void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setLcdCursor(0,0);
  myrobot.lcdPrint(i); 
  delay(1000);
  i++;
}
```

---

#### setLcdCursor(uint8_t, uint8_t)
Positionne le curseur de l'écran. 
##### Paramètres : 
- (colonne, ligne). L'écran contient 16 colonnes (de 0 à 15) et 2 lignes (de 0 à 1), (0,0) étant le coin en haut a gauche.
##### Valeur de retour : 
Aucune
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  for (int i=0; i<=1; ++i){
    for (int j=0; j<=15; ++j){
      myrobot.setLcdCursor(j,i);
      myrobot.lcdPrint(">>>"); 
      delay(200);
      myrobot.setLcdCursor(j,i);
      myrobot.lcdPrint(" ");
    }
  }
}
```

---

#### lcdHome(void)
Positionne le curseur en (0,0).
##### Paramètres : 
Aucun.
##### Valeur de retour : 
Aucune.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
      myrobot.setLcdCursor(0,1);
      myrobot.lcdPrint("2nd line"); 
      
      myrobot.lcdHome();
      myrobot.lcdPrint("Return to Home");
      delay(2000);
    
}
```

---

#### lcdClear(void)
Efface les données de l'écran.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
Aucune.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
    myrobot.lcdHome();
    myrobot.lcdPrint("Hello World !");
    delay(2000);
    myrobot.lcdClear();
    delay(2000);
}
```

---

#### gedInfrared(void)
Retourne la valeur du capteur de réflectance infrarouge.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
bool : égale à 0 si l'infrarouge est réfléchi.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
     if( myrobot.getInfrared()){
      myrobot.lcdPrint("1"); 
     }
     else{
      myrobot.lcdPrint("0"); 
     }
      myrobot.lcdHome(); 
    
}
```

---

#### getVoltage(void)
Retourne la valeur de la tension de la batterie.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : tension aux bornes de la batterie, en mV.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.lcdClear(); 
  myrobot.lcdHome(); 
  myrobot.lcdPrint(myrobot.getVoltage()); 
  delay(2000);
    
}
```

---

#### getBatteryLevel(void)
Retourne la tension de la batterie sur une échelle de 0 à 10.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
int : valeur comprise entre 0 et 10 (0 => 6000mV, 10 => 8400mV).
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
     myrobot.setLedBarLevel(myrobot.getBatteryLevel());
     delay(500);
}
```

---

#### getUsDist(String _pos)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### setLeftMotor(int _speed)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getBumper(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getInterruptFlag(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### resetInterruptFlag(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple :  
```c++
```

---

#### getJoystickY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple :  
```c++
```

---

#### getJoystickX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getJoystickClic(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### setServo(int)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getServo(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getAccelX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getAccelY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getAccelZ(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

####  getGyroX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple :  
```c++
```

---

#### getGyroY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getGyroZ(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getTemp(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### sendWifiCmd(char *cmd)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### waitWifiResult(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### displayWifiAnswer(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### getEncoder(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---

#### resetEncoder(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
```c++
```

---
