## T03: Serveis de transferència de fitxers

![foto](img_t03blai/1.png)

Posem el primer adaptador en xarxa NAT

![foto](img_t03blai/2.png)

I al segon adaptador el posem en xarxa amfitrió


![foto](img_t03blai/3.png)

Entrem a configurar la xarxa amb el nano /etc/netplan/50-cloud-init.yaml. activem l’enp0s8 i posem al dhcp4: true

![foto](img_t03blai/4.png)

Sortim i fem un sudo netplan apply.

![foto](img_t03blai/5.png)

Fem un sudo apt update && sudo apt upgrade -y. 

![foto](img_t03blai/6.png)

I podem veure com llegeix els paquets de la màquina 

![foto](img_t03blai/7.png)

Un cop entrem a la màquina un cop posats els adaptadors correctament fem un ip a per veure les nostres ip’s de la màquina.

![foto](img_t03blai/8.png)

amb la comanda sudo apt install vfstpd per instalar el vfstpd.

![foto](img_t03blai/9.png)

Un cop instalat fem un 
systemctl status vsftpd 
i un systemctl enable vsftpd


![foto](img_t03blai/10.png)

Fem un cp /etc/vsftpd.conf /etc/vsftpd.conf.original

![foto](img_t03blai/11.png)

i fem un cp /etc/vsftpd.conf /etc/vsftpd.bak

![foto](img_t03blai/12.png)

Fem un cat /etc/vsftpd.conf | head -30 per revisa el contigut del fitxer de configuració. 

![foto](img_t03blai/13.png)

Amb la comanda sudo nano /etc/vfstpd.conf entrem al arxiu. 

![foto](img_t03blai/14.png)

Un cop entrem al arxiu busquem anonymous_enable=No i ho cambien per YES i reiniciem el servei. 

![foto](img_t03blai/15.png)
Per reinicia el servei fem un: 
systemctl restart vsftpd 
systemctl status vsftpd
systemctl enable vsftpd 
I ja haurem reiniciat el servei de l’arxiu. 

![foto](img_t03blai/16.png)

I quan a l’arxiu posem que no li estem dien que l’usuari anonymous no pugui entrar. 

![foto](img_t03blai/17.png)

Com podeu veure quan el posem no li deixa entrar. 


![foto](img_t03blai/18.png)

Farem un ls -la /srv/ per veure que estan a dins correctament. 

![foto](img_t03blai/19.png)

fem un mkdir per crear la carpeta /srv/ftp

![foto](img_t03blai/20.png)

I fem mkdir perque a dins de la carpeta /srv/ftp i hagi al pub el files al music i el pics


![foto](img_t03blai/21.png)

Installem al tree amb la comanda apt install tree

![foto](img_t03blai/22.png)

I un cop instal·lat fem la comanda tree /srv/ per veure al que te a dins la carpeta /srv/

![foto](img_t03blai/23.png)

Fem un touch document.txt i un touch song.mp3

![foto](img_t03blai/24.png)

I si tornem a fer el tree /srv/ podem veure com a dins de files esta el document.txt i dins del music està al song.mp3

![foto](img_t03blai/25.png)

i creem el sun.jpg dins de la carpeta /srv/ftp/pub/pics/sun.jpg

![foto](img_t03blai/26.png)

i si fem un altre tree /srv/ podem veure que a dins de pics esta al sun.jpg

![foto](img_t03blai/27.png)

Fem un ftp amb la nostre ip posem anonymous posem la conttrasenya i podem veure que a l’anonymous li deixa entrar. 

![foto](img_t03blai/28.png)

creem la prova1 amb useradd prova1 i amb passwd creem la contrasenya i al mateix amb la prova2

![foto](img_t03blai/29.png)

![foto](img_t03blai/30.png)

Entrem a l’arxiu sudo nano /etc/vsftpd busquem la linia marcada en vermell i las posem en YES

![foto](img_t03blai/31.png)

I mes abaix de l’arxiu busquem aquestas dues i las posem tambe en YES

![foto](img_t03blai/32.png)

sortim de l’arxiu i fem un restart de l’arxiu i un status per veure com està al servei.

## CLIENT 

![foto](img_t03blai/33.png)

Posem el primer adaptador en NAT 

![foto](img_t03blai/34.png)

I el segon al posem habilitat amb amfitrió.

![foto](img_t03blai/35.png)

I posan la nostre ip de la màquina del servido amb al nom del usuari creat al servidor i la seva contrasenya ens haurien de sortir totes las carpetes creades al servidor correctament. 
