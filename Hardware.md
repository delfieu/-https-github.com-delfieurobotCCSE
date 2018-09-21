# Hardware :

## Liste des composants électroniques : 
| Composant | Quantité | Description |
|:-:|:-:|---|
| [Arduino Mega<br/><img src="https://store-cdn.arduino.cc/usa/catalog/product/cache/1/image/520x330/604a3538c15e081937dbfbd20aa60aad/a/0/a000067_featured_1_.jpg" width="200">](https://store.arduino.cc/usa/arduino-mega-2560-rev3) | 1 | L'arduino Mega est le "cerveau" de notre robot, c'est le micro-contrôleur présent sur cette carte que nous allons programmer afin de contrôler le robot. |
| [Grove Mega Shield<br/><img src="https://github.com/SeeedDocument/Grove-Mega_Shield/raw/master/img/500px-Megashieldn1_03.jpg" width="200">](http://wiki.seeedstudio.com/Grove-Mega_Shield/) | 1 | Ce shield permet d'avoir des connectiques Grove (4 pins) disponibles et directement connectées à l'Arduino Mega. Il sert également de hub I2C. |
| [Capteur à Ultrasons<br/><img src="https://github.com/SeeedDocument/Grove_Ultrasonic_Ranger/raw/master/img/Ultrasonic.jpg" width="200">](http://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/) | 2 | Les capteurs à ultrasons permettent de mesurer une distance. |
| [Ecran LCD RGB<br/><img src="https://raw.githubusercontent.com/SeeedDocument/Grove_LCD_RGB_Backlight/master/images/intro.jpg" width="200">](http://wiki.seeedstudio.com/Grove-LCD_RGB_Backlight/) | 1 | Principale interface entre l'utilisateur et le robot, cet écran vous permettra d'afficher des informations ou de changer de couleur (selon l'état du robot, par exemple). |
| [Joystick<br/><img src="https://raw.githubusercontent.com/SeeedDocument/Grove-Thumb_Joystick/master/img/Bgjoy1.jpg" width="200">](http://wiki.seeedstudio.com/Grove-Thumb_Joystick/) | 1 | Équipé de deux potentiomètres (axes X et Y) et d'un bouton, il permet à l'utilisateur d'interagir avec le robot. |
| [Barre de LED<br/><img src="https://raw.githubusercontent.com/SeeedDocument/Grove-LED_Bar/master/img/Grove-LED_Bar-1.jpg" width="200">](http://wiki.seeedstudio.com/Grove-LED_Bar/) | 1 | Seconde interface visuelle du robot, la barre de LED permettra d'afficher sur une échelle de 0 à 10 la charge de la batterie ou la vitesse des moteurs, par exemple. |
| [Accéléromètre 6 axes<br/><img src="https://raw.githubusercontent.com/SeeedDocument/Grove-6-Axis_AccelerometerAndGyroscope/master/img/Grove-6-Axis_AccelerometerAndGyroscope_product_view_1200_s.jpg" width="200">](http://wiki.seeedstudio.com/Grove-6-Axis_AccelerometerAndGyroscope/) | 1 | Ce composant est en fait la combinaison d'un accéléromètre (3 axes) et d'un gyroscope (3 axes) qui vous permettra de connaître la position angulaire de votre robot et l'accélération qu'il subit.|
| [Module wifi<br/><img src="https://github.com/SeeedDocument/Grove-Uart_Wifi/raw/master/img/V2/Main.JPG" width="200">](http://wiki.seeedstudio.com/Grove-UART_Wifi_V2/) | 1 | Le module wifi est un émetteur/receveur série intégrant les couche TCP/IP.|
| [Carte de contrôle des moteurs<br/><img src="https://raw.githubusercontent.com/SeeedDocument/Grove-I2C_Motor_Driver_V1.3/master/img/I2CMotorDriver_New.jpg" width="200">](http://wiki.seeedstudio.com/Grove-I2C_Motor_Driver_V1.3/) | 1 | Cette carte permet le contrôle de moteurs à courant continu avec un double pont en H (jusqu’à 1A). Les commandes lui sont envoyées en I2C. |
| [Diviseur de tension<br/><img src="https://github.com/SeeedDocument/Grove-Voltage_Divider/raw/master/img/Voltage_Divider_01.jpg" width="200">](http://wiki.seeedstudio.com/Grove-Voltage_Divider/) |  1 | Permet de connaître la tension aux bornes de la batterie. |
| [Capteur de réflectance infrarouge<br/><img src="https://github.com/SeeedDocument/Grove-Infrared_Reflective_Sensor/raw/master/img/thumbnail.jpg" width="200">](http://wiki.seeedstudio.com/Grove-Infrared_Reflective_Sensor/) | 1 | Ce capteur permet de repérer une ligne noire ou des espaces vides. |
| [Batterie<br/><img src="https://static.generation-robots.com/10665-large_default/batterie-li-ion-74v-2200mah-2s2p-avec-pcm.jpg" width="200">](https://www.generationrobots.com/fr/403175-batterie-li-ion-74v-2200mah-2s2p-avec-pcm.html?utm_source=Doofinder&utm_medium=Doofinder&utm_campaign=Doofinder) | 1 | Cette batterie Li-ion de 2,2 Ah permet une grande autonomie. Elle intègre une protection contre la décharge et la surcharge et peut être chargée alors que le robot est allumé. |
| [Servomoteur<br/><img src="https://www.parallax.com/sites/default/files/styles/full-size-product/public/900-00005.png?itok=uNwvj185" width="200">](https://www.parallax.com/sites/default/files/downloads/900-00005-Standard-Servo-Product-Documentation-v2.2.pdf) | 1 | Le servomoteur est utilisé pour faire pivoter le capteur à ultrasons avant afin de pouvoir balayer l'espace à la recherche d'objets ou éviter les obstacles. |
| [Moteur<br/><img src="https://images-na.ssl-images-amazon.com/images/I/41ltFs26adL._SY355_.jpg" width="200">](https://www.pololu.com/product/2385/specs) | 2 | Ces moteurs compacts avec un rapport de réduction de 298:1 servent à entraîner les roues. |
| [Encodeur<br/><img src="https://a.pololu-files.com/picture/0J6833.1200.jpg?37cdba39b716a232eb49d5fb765e15c0" width="200">](https://www.pololu.com/product/3081) | 2 | Ces encodeurs magnétiques utilisent un disque magnétique et génèrent 12 pulsations par tour de moteur. |


## Liste des pièces mécaniques : 
| Pièce | Quantité | Description |
|:-:|:-:|---|
| [Roue motrice<br/><img src="https://a.pololu-files.com/picture/0J2673.600x480.jpg?31dc6108b680fbbdaeca43110befd0a6" width="200">](https://www.pololu.com/product/1423) | 2 | Les roues ont un revêtement en silicone pour une bonne adhérence sur la plupart des surfaces. Elles mesurent 60mm de diamètre et 8mm de large. |
<!---
| [Châssis<br/><img src="LINK" width="200">](LINK) |   |   |
| [blabla <br/><img src="LINK" width="200">](LINK) |   |   |
| [blabla <br/><img src="LINK" width="200">](LINK) |   |   |
| [blabla <br/><img src="LINK" width="200">](LINK) |   |   | --->

