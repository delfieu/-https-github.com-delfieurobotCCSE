# M.A.R.K : la librairie ! 
## Les fonctions

* [MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie/_edit#markvoid)
* [~MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie/_edit#markvoid-1)
* [begin()](https://github.com/generationrobots-lab/MARK/wiki/Librairie/_edit#begin)
* [setLeftMotor(int _speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie/_edit#setleftmotorint-_speed)

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
##### exemple : 

```c++
#include <MARK.h>

MARK myrobot; //initialize an instance of the class
```


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