# Bienvenue dans le wiki du projet M.A.R.K ! 
![blabla](https://dubsism.files.wordpress.com/2017/12/image-not-found.png?w=547)<br />
Ici vous trouverez le nécessaire pour programmer et customiser votre robot. <br />

## Pour bien débuter

### Prérequis : 

#### IDE Arduino
Page de téléchargement : <br />
https://www.arduino.cc/en/Main/Software

Tutoriels d'installation : <br />
https://www.arduino.cc/en/Guide/Windows<br />
https://www.arduino.cc/en/Guide/Linux <br />
Le paquet Arduino est également présent dans les dépôts Universe d'Ubuntu.

#### M.A.R.K librairie

1. [Télécharger le git](https://github.com/generationrobots-lab/MARK/archive/master.zip)
2. Décompresser l'archive et placez-là où bon vous semble.
3. Lancer l'IDE Arduino 
4. Dans Fichier => Préférences => dans l'onglet Paramètres, le champ "Emplacement du carnet de croquis" doit pointer vers le dossier "Software" de l'archive fraichement décompressée et rangée (exemple : D:\MARK-master\Software)
5. Dans l'IDE Arduino, vous devriez voir apparaitre dans Ficher => Carnet de croquis les exemples pour débuter avec votre M.A.R.K.

Il est également possible de fusionner le dossier Software avec le dossier que vous utilisez déjà (par defaut C:\Users\..\Documents\Arduino).

## Software

### La librairie M.A.R.K
La librairie que nous vous proposons permet de simplifier l'utilisation des capteurs vendus avec le robot. Merci de vous rendre sur [la page "Librairie"](https://github.com/generationrobots-lab/MARK/wiki/Librairie) pour plus d'informations sur les fonctions.
### Les librairies sources
Vous pouvez également programmer votre Arduino Mega de A à Z, comme vous le souhaitez et optimiser ainsi votre code. Voici quelques pistes par où commencer : 
* [Accelerometre](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Accelerometer_And_Gyroscope_LSM6DS3-master)
* [Encodeurs](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Encoder-master)
* [Motor driver](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_I2C_Motor_Driver_v1_3-master)
* [LCD RGB](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_LCD_RGB_Backlight-master)
* [LED bar](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_LED_Bar-master)
* [Ultrasonic ranger](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_Ultrasonic_Ranger-master)

Vous trouverez des exemples dans Fichier => Carnet de croquis, ou dans le git [ici](https://github.com/generationrobots-lab/MARK/tree/master/Software). 

## Hardware

### Électronique <br />
M.A.R.K est un robot qui se veut modulable, pour cela son électronique se base un maximum sur un maximum de capteur GROVE, qui facilite la connectique et permet la réalisation simple de prototypes. 

Pour avoir plus d'informations sur le câblage du robot et sur les composants électroniques, merci de visiter [la page dédiée du wiki](https://github.com/generationrobots-lab/MARK/wiki/%C3%89lectronique).
### Mécanique
Pour avoir plus d'informations sur la structure et sur les composants mécaniques, merci de visiter [la page dédiée du wiki](https://github.com/generationrobots-lab/MARK/wiki/M%C3%A9canique).
