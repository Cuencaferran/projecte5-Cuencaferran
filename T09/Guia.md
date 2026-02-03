# T09 Vulnerabilitats. Guia de la pràctica

![foto](img_t09carlos/1.png)

Prime posem la Ova a documents i la importem i a paràmetres posem generar una nova MAC.

![foto](img_t09carlos/2.png)

Posem la màquina de metasploitable el primer adaptador en xarxa Nat.

![foto](img_t09carlos/3.png)

Posem la màquina Openvas el primer adaptador en xarxa NAT

![foto](img_t09carlos/4.png)

I el segon adaptador de openvas en amfitrió.

![foto](img_t09carlos/5.png)

La primer opció li donem a YES.

![foto](img_t09carlos/6.png)

Seguidament li doem a YES.

![foto](img_t09carlos/7.png)

En aquest pas posem com a nome usuari i com a contrasenya usuari també.

![foto](img_t09carlos/8.png)

Ja ens dona l’ok de que l’usuari s’ha creat.

![foto](img_t09carlos/9.png)

Aqui li donem a SKIP.

![foto](img_t09carlos/10.png)

![foto](img_t09carlos/11.png)

En aquesta part triem la primera opció de totas i li donem a ok.

![foto](img_t09carlos/12.png)

Aqui posem la segona opció de Network i li donem OK.

![foto](img_t09carlos/13.png)

Aqui fem la primera opció de interfaces.

![foto](img_t09carlos/14.png)

Posem la configuracio interface eth0.

![foto](img_t09carlos/15.png)

Aquí podem veure com he habilitat las ipv4 eth0 i la eth1.

![foto](img_t09carlos/16.png)

Ara amb la nostre ip entrem en el greenbone i ens demanara un usuari i una contrasenya posem usuari usuari que es com hem configurat abans la màquina.

![foto](img_t09carlos/17.png)

Entrem a assets i dins de assets a hosts.

![foto](img_t09carlos/18.png)

IP adresse posem la nostre que en el meu cas es 10.0.2.4 i posem linux com a comentari.

![foto](img_t09carlos/19.png)

creem al nou SSH li posem usuari de nom posem la primera opció en YES i de username posem msfadmin i com a contrasenya també msfadmin.

![foto](img_t09carlos/20.png)

Ara creem una nova tasca on com a nom li posem vulnerable posem openvasdefault ja que va més ràpid que CEV i li donem a save.

![foto](img_t09carlos/21.png)

I la iniciem i ens esperem fins que acabi la instal·lació.

![foto](img_t09carlos/22.png)


