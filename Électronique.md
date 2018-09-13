# M.A.R.K : l'électronique.
Cett
## Connexion des modules :

### Ultrason avant

| Ultrason | Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | NC|
| YELLOW | D8 |

### Ultrason arrière

| Ultrason| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | NC|
| YELLOW | D10 |

### LCD RGB

| LCD RGB| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | SDA|
| YELLOW | SCL |

### Joystick

| Joystick| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | A3|
| YELLOW | A2 |

### Barre de leds

| Barre de leds| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | D5|
| YELLOW | D4 |

### Accéléromètre 

| Accéléromètre | Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | SDA|
| YELLOW | SCL |

### Module wifi

| Module wifi| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | D14/TX3|
| YELLOW | D15/RX3 |

### Carte de contrôle des moteurs

| Carte de contrôle des moteurs| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | SDA |
| YELLOW | SCL |

### Diviseur de tension

| Diviseur de tension| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | NC |
| YELLOW | A0 |

### Capteur de réflectance infrarouge

| Capteur de réflectance infrarouge| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | NC |
| YELLOW | D6 |

## Autre

### Servomoteur

| Servomoteur| Grove Shield | 
|:-:|:-:|
| GND | GND |
| VCC | VCC |
| WHITE | PWM D12|


### Encodeur gauche

| Encodeur | Grove Shield | Arduino Mega | Carte de contrôle des moteurs |
|:-:|:-:|:-:|:-:|
| GND | GND | - | - |
| OUT B | D18 | - | - |
| OUT A | - | D29 | - |
| VCC | VCC | - | - |
| M1 | - | - | M1- |
| M2 | - | - | M1+ |

### Encodeur droit

| Encodeur | Grove Shield | Arduino Mega | Carte de contrôle des moteurs |
|:-:|:-:|:-:|:-:|
| GND | GND | - | - |
| OUT B | - | D27 | - |
| OUT A | D19 | - | - |
| VCC | VCC | - | - |
| M1 | - | - | M2+ |
| M2 | - | - | M2- |


### Bumper droit

| Bumper droit | Grove Shield | 
|:-:|:-:|
| GND | GND |
| OUT | D3 |

### Bumper gauche

| Bumper gauche | Grove Shield | 
|:-:|:-:|
| GND | GND |
| OUT | D2 |

## Que reste-t-il de libre ? 

* A1 
* A4 -> A15
* D7
* D9
* D11
* D13
* D16
* D17
* D22 -> D26
* D28
* D30 -> D53