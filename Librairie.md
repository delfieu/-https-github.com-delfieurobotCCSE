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
* [gedInfrared(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#gedinfraredvoid)
* [getVoltage(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getvoltagevoid)
* [getBatteryLevel(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getbatterylevelvoid)
* [getUsDist(String _pos)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getusdiststring-_pos)
* [setLeftMotor(int _speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setleftmotorint-_speed-1)
* [getBumper(String _side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getbumperstring-_side)
* [getInterruptFlag(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getinterruptflagvoid)
* [resetInterruptFlag(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#resetinterruptflagvoid)
* [getJoystickY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickyvoid)
* [getJoystickX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickxvoid)
* [getJoystickClic(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickclicvoid)
* [setServo(int)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setservoint)
* [getServo(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getservovoid)
* [getAccelX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getaccelxvoid)
* [getAccelY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getaccelyvoid)
* [getAccelZ(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getaccelzvoid)
* [getGyroX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getgyroxvoid)
* [getGyroY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getgyroyvoid)
* [getGyroZ(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getgyrozvoid)
* [getTemp(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#gettempvoid)
* [sendWifiCmd(char *cmd)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#sendwificmdchar-cmd)
* [waitWifiResult(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#waitwifiresultvoid)
* [displayWifiAnswer(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#displaywifianswervoid)
* [getEncoder(String _side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getencoderstring-_side)
* [resetEncoder(String _side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#resetencoderstring-_side)

---

#### MARK(void)
Constructeur. 
##### Exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class
```

---

#### ~MARK(void)
Desctructeur

---

#### begin(void)
Initialisation de la classe (Serial, I2C, encodeurs etc)
##### Paramètres : 
##### Valeur de retour : 
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

#### setLeftMotor(int _speed)
Configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
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

#### setRightMotor(int _speed)
Configure la vitesse du moteur droit (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
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

#### stopLeftMotor(void)
Stop le moteur gauche.
##### Paramètres : 
##### Valeur de retour : 
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
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
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
##### Valeur de retour : 
##### Exemple : 

---

#### lcdPrint(String text)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### lcdPrint(float data)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### setLcdCursor(uint8_t, uint8_t)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### lcdHome(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### lcdClear(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### gedInfrared(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getVoltage(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getBatteryLevel(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getUsDist(String _pos)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### setLeftMotor(int _speed)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getBumper(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getInterruptFlag(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### resetInterruptFlag(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple :  

---

#### getJoystickY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple :  

---

#### getJoystickX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getJoystickClic(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### setServo(int)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getServo(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getAccelX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getAccelY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 
---

#### getAccelZ(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

####  getGyroX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple :  

---

#### getGyroY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getGyroZ(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getTemp(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### sendWifiCmd(char *cmd)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### waitWifiResult(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### displayWifiAnswer(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### getEncoder(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 

---

#### resetEncoder(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### Paramètres : 
##### Valeur de retour : 
##### Exemple : 