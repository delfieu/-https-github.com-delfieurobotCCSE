# Bienvenue dans le wiki du projet M.A.R.K ! 
<!-- ![blabla](https://dubsism.files.wordpress.com/2017/12/image-not-found.png?w=547)<br /> -->
Vous trouverez ici tout le nécessaire pour programmer et customiser votre robot. <br />

## Pour bien débuter

### Prérequis : 

#### Installer l'IDE Arduino
Page de téléchargement : <br />
https://www.arduino.cc/en/Main/Software

Tutoriels d'installation : <br />
https://www.arduino.cc/en/Guide/Windows<br />
https://www.arduino.cc/en/Guide/Linux <br />
Le paquet Arduino est également présent dans les dépôts Universe d'Ubuntu.

#### Installer la librairie MARK

1. [Télécharger le git](https://github.com/generationrobots-lab/MARK/archive/master.zip)
2. Décompresser l'archive et la placer dans un répertoire de votre choix.
3. Lancer l'IDE Arduino 
4. Dans `Fichier => Préférences => Paramètres`, le champ "Emplacement du carnet de croquis" doit pointer vers le dossier "Software" de l'archive fraîchement décompressée et rangée (exemple : D:\MARK-master\Software)
5. Dans l'IDE Arduino, vous devriez voir apparaître dans `Ficher => exemples => MARK` les exemples pour débuter avec votre M.A.R.K.

Il est également possible de fusionner le dossier Software avec le dossier que vous utilisez déjà (par défaut C:\Users\..\Documents\Arduino).

## La librairie M.A.R.K

La librairie que nous vous proposons permet de simplifier l'utilisation des capteurs vendus avec le robot. Merci de vous rendre sur [la page "Librairie"](https://github.com/generationrobots-lab/MARK/wiki/Librairie) pour plus d'informations sur les fonctions.

## Les librairies sources
Vous pouvez également programmer votre Arduino Mega de A à Z, comme vous le souhaitez, et optimiser ainsi votre code. Voici quelques pistes pour commencer : 
* [Accéléromètre](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Accelerometer_And_Gyroscope_LSM6DS3-master)
* [Encodeurs](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Encoder-master)
* [Motor driver](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_I2C_Motor_Driver_v1_3-master)
* [LCD RGB](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_LCD_RGB_Backlight-master)
* [LED bar](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_LED_Bar-master)
* [Capteur à ultrasons](https://github.com/generationrobots-lab/MARK/tree/master/Software/libraries/Grove_Ultrasonic_Ranger-master)

Vous trouverez des exemples dans `Fichier => Carnet de croquis`, ou dans le git [ici](https://github.com/generationrobots-lab/MARK/tree/master/software). 

## Hardware

### Électronique <br />
M.A.R.K est un robot qui se veut modulable, pour cela son électronique se base sur un maximum de capteurs GROVE, ce qui permet la réalisation simple de prototypes, grâce notamment à leur connectique standardisée. 

Pour avoir plus d'informations sur le câblage du robot et sur les composants électroniques, merci de visiter [la page dédiée du wiki](https://github.com/generationrobots-lab/MARK/wiki/%C3%89lectronique).

### Mécanique
Pour avoir plus d'informations sur la structure et sur les composants mécaniques, merci de visiter [la page dédiée du wiki](https://github.com/generationrobots-lab/MARK/wiki/M%C3%A9canique).
