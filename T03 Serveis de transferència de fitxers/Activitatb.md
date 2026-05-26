# ACTIVITAT B

![foto](img_t03B/1.png)

Primer fem un sudo apt install openssh-server -y posem la nostra contrasenya i veiem com ens comença a llegir tot. 

![foto](img_t03B/2.png)

Entrem a la màquina client i posem sftp usuari@192.168.56.101 cadascú amb la seva ip corresponent, posem la contrasenya i ja podem començar a treballar. 

![foto](img_t03blai/3.png)

posem un interrogan i podem veure el available command. 

![foto](img_t03B/4.png)

Aqui podem veure com l’usuari pot explorar tot el sistema d’arxius.

![foto](img_t03B/5.png)

Entrem al arxiu de ssh config 

![foto](img_t03B/6.png)

I abaix de tot de l’arxiu afegim aquest paràgraf. 

![foto](img_t03B/7.png)

surtim de l’arxiu i fem un restart ssh i status ssh 

![foto](img_t03B/8.png)

Fem un sudo addgroup admins i dins de admins afegim amb useradd admin1 i li posem una contrasenya

![foto](img_t03B/9.png)

Fem un sudo mkdir /var/data i amb ls -l /var podem veure al que hi ha a la carpeta.

![foto](img_t03B/10.png)

Fem sudo mkdir /var/data/files

![foto](img_t03B/11.png)

fem un sudo chown :admins /var/data/files i un sudo chown 2770 /var/data/files fem un ls -l /var/data per veure que s’ha fet correctament. 

![foto](img_t03B/12.png)

fem un restart i un status ssh

![foto](img_t03B/13.png)

Entrem amb powershell del client i posem sftp admin1@192.168.56.101 
posem la contrasenya i veiem com funciona correctament.



