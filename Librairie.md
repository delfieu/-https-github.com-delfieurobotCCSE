# M.A.R.K : la librairie ! 
## Les fonctions
Général  : <br />
* [MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid)
* [~MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid-1) 

Moteurs : <br />

* [begin()](https://github.com/generationrobots-lab/MARK/wiki/Librairie#begin)
* [setLeftMotor(int _speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setleftmotorint-_speed)
* [setRightMotor(int _speed)]()
* [stopLeftMotor()]()
* [stopRightMotor()]()

LCD RGB : 

* [setLcdRGB(unsigned char r, unsigned char g, unsigned char b)]()
* [lcdPrint(String text)]()
* [lcdPrint(float data)]()
* [setLcdCursor(uint8_t, uint8_t)]()
* [lcdHome()]()
* [lcdClear()]()
<!---
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
* []()
--->

---

#### MARK(void)
Constructeur. 
##### exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class
```

---

#### ~MARK(void)
Desctructeur

---

#### begin()
Initialisation de la classe (Serial, I2C, encodeurs etc)
##### exemple : 

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
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setRightMotor(-50);
  delay(1000);
  stopLeftMotor()
  stopRightMotor()
  delay(1000);
}

```

---

#### setRightMotor(int _speed)
configure la vitesse du moteur droit (-100 < _speed < 100 , 0 = stop).
##### exemple : 
```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setRightMotor(-50);
  delay(1000);
  stopLeftMotor()
  stopRightMotor()
  delay(1000);
}

```

---

#### stopLeftMotor()
Stop le moteur gauche.
##### exemple : 
```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setRightMotor(50);
  myrobot.setRightMotor(-50);
  delay(1000);
  stopLeftMotor()
  stopRightMotor()
  delay(1000);
}

```

---

#### stopRightMotor()
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### setLcdRGB(unsigned char r, unsigned char g, unsigned char b)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### lcdPrint(String text)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### lcdPrint(float data)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### setLcdCursor(uint8_t, uint8_t)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### lcdHome()
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### lcdClear()
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### gedInfrared()
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getVoltage(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getBatteryLevel(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getUsDist(String _pos)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### setLeftMotor(int _speed)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getBumper(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getInterruptFlag()
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### resetInterruptFlag()
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getJoystickY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getJoystickX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getJoystickClic(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### setServo(int)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getServo(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getAccelX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getAccelY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getAccelZ(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

####  getGyroX(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getGyroY(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getGyroZ(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getTemp(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### sendWifiCmd(char *cmd)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### waitWifiResult(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### displayWifiAnswer(void)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### getEncoder(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 

---

#### resetEncoder(String _side)
configure la vitesse du moteur gauche (-100 < _speed < 100 , 0 = stop).
##### exemple : 