# M.A.R.K : la librairie ! 

## Les fonctions
Général  : <br />
* [MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid)
* [~MARK(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#markvoid-1) 
* [begin(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#beginvoid)
    
Moteurs :

* [setLeftMotor(int speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setleftmotorint-speed)
* [setRightMotor(int speed)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setrightmotorint-speed)
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

* [setLedBarLevel(int level)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setledbarlevelint-level)
* [getLedBarLevel(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getledbarlevelvoid)

Capteur de réflectance infrarouge : 

* [gedInfrared(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#gedinfraredvoid)

Diviseur de tension : 

* [getVoltage(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getvoltagevoid)
* [getBatteryLevel(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getbatterylevelvoid)

Capteurs à ultrasons : 

* [getUsDist(String pos)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getusdiststring-pos)

Capteur de contact : 

* [getBumper(String side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getbumperstring-side)
* [getInterruptFlag(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getinterruptflagvoid)
* [resetInterruptFlag(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#resetinterruptflagvoid)

Joystick : 

* [getJoystickY(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickyvoid)
* [getJoystickX(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickxvoid)
* [getJoystickClic(void)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getjoystickclicvoid)

Servomoteur : 

* [setServo(int pos)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#setservoint-pos)
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

* [getEncoder(String side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#getencoderstring-side)
* [resetEncoder(String side)](https://github.com/generationrobots-lab/MARK/wiki/Librairie#resetencoderstring-side)

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
##### Exemple : 

```c++
#include <MARK.h>
MARK myrobot; 
myrobot.~MARK(); //Destructor
```

---

#### begin(void)
Initialisation de la classe (Serial, I2C, encodeurs, etc).
##### Paramètres :
Aucun.
##### Valeur de retour :
bool : égale à 1 si la fonction s'exécute correctement.
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
- (int) speed : vitesse du moteur. Les nombres négatifs font tourner le moteur vers l'arrière (de -1 à -100), les nombres positifs font tourner le moteur vers l'avant (de 1 à 100) et 0 fait arrêter le moteur.
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
- (int) speed : vitesse du moteur. Les nombres négatifs font tourner le moteur vers l'arrière (de -1 à -100), les nombres positifs font tourner le moteur vers l'avant (de 1 à 100) et 0 fait arrêter le moteur.
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
Stoppe le moteur gauche.
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
Stoppe le moteur droit.
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
Configure la couleur de l'écran. 
##### Paramètres : 
- (unsigned char) r : valeur de la composante rouge (entre 0 et 255).
- (unsigned char) g : valeur de la composante verte (entre 0 et 255).
- (unsigned char) b : valeur de la composante bleue (entre 0 et 255).
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
- (String) text : chaîne de caractères à afficher.
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
- (float) data: nombre à afficher.
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
- (colonne, ligne). L'écran contient 16 colonnes (de 0 à 15) et 2 lignes (de 0 à 1), (0,0) étant le coin supérieur gauche.
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

#### setLedBarLevel(int level)
Allume la barre de led. 
##### Paramètres : 
* (int) level : le niveau de la barre de led (0 => éteint, 10 => tout est allumé).
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
  for(int i=0; i<=10;i++){
     myrobot.setLedBarLevel(i);
     delay(500);
  }    
}

```

---

#### getLedBarLevel(void)
Retourne la dernière valeur appelée avec la fonction setLedBarLevel.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
int : valeur entre 0 et 10.

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

#### getUsDist(String pos)
Retourne la distance devant un ultrason.
##### Paramètres : 
* (String) pos : permet d'identifier sur quel ultrason la mesure doit être faite. 
##### Valeur de retour : 
int : valeur en centimètre. 
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.lcdClear();
  myrobot.setLcdCursor(0,0);
  myrobot.lcdPrint(myrobot.getUsDist("front")); 
  myrobot.setLcdCursor(0,1);
  myrobot.lcdPrint(myrobot.getUsDist("back")); 
  delay(1000);
}
```

---

#### getBumper(String side)
Retourne la valeur d'un microswitch.
##### Paramètres : 
* (String) side : permet d'identifier sur quel bumper la mesure doit être faite. 
##### Valeur de retour : 
bool : égale à 1 si le contact est présent (switch fermé).
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
}

void loop() {
  myrobot.setLcdCursor(0,0);
  myrobot.lcdPrint(myrobot.getBumper("right")); 
  myrobot.setLcdCursor(0,1);
  myrobot.lcdPrint(myrobot.getBumper("left")); 
  delay(100);
}
```

---

#### getInterruptFlag(void)
Retourne l'état de l'interruption.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
bool : égale à 1 si un bumper a changé d'état.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
   myrobot.setRightMotor(50);
  myrobot.setLeftMotor(50);
}

void loop() {
if(myrobot.getInterruptFlag()){
  myrobot.stopLeftMotor();
  myrobot.stopRightMotor();
  }
}
```

---

#### resetInterruptFlag(void)
Réinitialise l'état de l'interruption.
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
  myrobot.setRightMotor(50);
  myrobot.setLeftMotor(50);
}

void loop() {
if(myrobot.getInterruptFlag()){
  myrobot.stopLeftMotor();
  myrobot.stopRightMotor();
  delay (5000);
  myrobot.resetInterruptFlag();
  myrobot.setRightMotor(50);
  myrobot.setLeftMotor(50);
  }
}
```

---

#### getJoystickX(void)
Retourne la valeur sur l'axe X du joystick.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
int : valeur sur l'axe Y (entre ~240 et ~780, 1023 si le bouton est pressé)
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.lcdClear();
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getJoystickX());
  delay(200);
}
```

---

#### getJoystickY(void)
Retourne la valeur sur l'axe Y du joystick.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
int : valeur sur l'axe Y (entre ~240 et ~780).
##### Exemple :  
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.lcdClear();
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getJoystickY());
  delay(200);
}
```

---

#### getJoystickClic(void)
Retourne l'état du bouton du joystick.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
bool : égale à 1 si le bouton est pressé.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  if(myrobot.getJoystickClic()){
    myrobot.setLcdRGB(255,0,0);
  }
  else{
    myrobot.setLcdRGB(0,255,255);
  }
}
```

---

#### setServo(int pos)
Positionne le servomoteur à un angle donné.
##### Paramètres : 
* (int) pos : angle du servomoteur (entre 0° et 180°).
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
  myrobot.setServo(0);
  delay(1000);
  myrobot.setServo(80);
  delay(1000);
  myrobot.setServo(160);
  delay(1000);
  myrobot.setServo(80);
  delay(1000);
}
```

---

#### getServo(void)
Retourne la dernière valeur utilisée pour la fonction setServo().
##### Paramètres : 
Aucun.
##### Valeur de retour : 
int : la dernière valeur utilisée pour la fonction setServo().

---

#### getAccelX(void)
Retourne la valeur de l’accéléromètre sur l'axe X.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : entre -1 et 1.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getAccelX());
  myrobot.lcdPrint("   ");
}
```

---

#### getAccelY(void)
Retourne la valeur de l’accéléromètre sur l'axe Y.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : entre -1 et 1
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getAccelY());
  myrobot.lcdPrint("   ");
}
```

---

#### getAccelZ(void)
Retourne la valeur de l’accéléromètre sur l'axe Z.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : entre -1 et 1.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getAccelZ());
  myrobot.lcdPrint("   ");
}
```

---

####  getGyroX(void)
Retourne la valeur du gyroscope sur l'axe X.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : entre -1 et 1.
##### Exemple :  
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getGyroX());
  myrobot.lcdPrint("   ");
}
```

---

#### getGyroY(void)
Retourne la valeur du gyroscope sur l'axe Y.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : entre -1 et 1.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getGyroY());
  myrobot.lcdPrint("   ");
}
```

---

#### getGyroZ(void)
Retourne la valeur du gyroscope sur l'axe Z.
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : entre -1 et 1.
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getGyroZ());
  myrobot.lcdPrint("   ");
}
```

---

#### getTemp(void)
Retourne la température. 
##### Paramètres : 
Aucun.
##### Valeur de retour : 
float : retourne la température. 
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getTemp());
  myrobot.lcdPrint("   ");
}
```

---

#### sendWifiCmd(char *cmd)
Envoie une commande au module wifi.
##### Paramètres : 
 * (char) cmd : commande à envoyer.
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
  myrobot.sendWifiCmd("AT+CWLAP");
  myrobot.waitWifiResult();
  myrobot.displayWifiAnswer();
}
```

---

#### waitWifiResult(void)
Fonction bloquante qui attend la réponse du module wifi.
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
  myrobot.sendWifiCmd("AT+CWLAP");
  myrobot.waitWifiResult();
  myrobot.displayWifiAnswer();
}
```

---

#### displayWifiAnswer(void)
Envoie sur le port série 1 (Serial 1) la réponse du module wifi.
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
  myrobot.sendWifiCmd("AT+CWLAP");
  myrobot.waitWifiResult();
  myrobot.displayWifiAnswer();
}
```

---

#### getEncoder(String side)
Retourne la valeur de l'encodeur choisi. 
##### Paramètres : 
(String) side : côté de l'encodeur ("right" ou "left").
##### Valeur de retour : 
long : nombre d'impulsions mesurées. 
##### Exemple : 
```c++
#include <MARK.h>

MARK myrobot; 

void setup() {
  myrobot.begin();
} 

void loop() {
  myrobot.lcdClear();
  myrobot.setLcdCursor(0, 0);
  myrobot.lcdPrint(myrobot.getEncoder("right"));
    myrobot.setLcdCursor(0, 1);
  myrobot.lcdPrint(myrobot.getEncoder("left"));
  delay(200);
}
```

---

#### resetEncoder(String side)
Réinitialise la valeur de l'encodeur choisi à 0.
##### Paramètres : 
(String) side : côté de l'encodeur ("right" ou "left").
##### Valeur de retour : 
Aucune.

