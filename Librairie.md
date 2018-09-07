# M.A.R.K : la librairie ! 
## Les fonctions
Général  : <br />
* [MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid)
* [~MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie/#markvoid-1) 
<br />

Moteurs : <br />

* [begin()](https://github.com/generationrobots-lab/MARK/wiki/Librairie/#begin)
* [setLeftMotor(int _speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie/#setleftmotorint-_speed)
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
  myrobot.setLeftMotor(50);
  delay(1000);
  myrobot.setLeftMotor(-50);
  delay(1000);
}

```