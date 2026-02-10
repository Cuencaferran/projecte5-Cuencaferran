## T07: Acadèmia feta amb Moodle

Breu descripció
És una pràctica individual i tancada. L’objectiu és demostrar que ets capaç d’instal·lar, personalitzar, configurar i gestionar Moodle com ho faries en un encàrrec real d’una organització.

Treballaràs per a un client en concret: una escola d’ensenyament secundari anomenada Escola Júlia, que necessita un portal d’aprenentatge online per facilitar la comunicació i l’aprenentatge entre professorat i alumnat. Per fer-ho, s’ha decidit utilitzar Moodle.
Molt important: aquesta pràctica està dividida en 5 parts.
Quan acabis cada part: avisa el professor/a perquè validi que ho tens tot correcte.
L’avaluació es farà “en directe”: hauràs d’ensenyar cada part i defensar-la (explicar on ho has configurat, per què i demostrar que funciona).




Objectius específics de la tasca / Finalitat de la tasca



Part 1: Instal·lar un sistema de gestió d’aprenentatge a distància, personalitzar-lo i configurar-lo segons les necessitats d’una organització

Una escola d'ensenyament secundari, anomenada Escola Júlia, ens ha demanat el desenvolupament d'un portal web d'aprenentatge amb l'objectiu d'oferir, tan als professors com als alumnes, una plataforma online que faciliti la comunicació i l'aprenentatge. Per tal de crear aquest portal, s'ha decidit utilitzar l'aplicació web Moodle.
Segueix les indicacions que es mostren a continuació per tal d'adaptar el Moodle a les necessitats del client.

1. El primer que haurem de fer es descomprimir el Moodle al nostre servidor web. Un cop disposem de l'aplicació allotjada al servidor, accedirem a través del navegador per començar la instal·lació.
Com podràs observar, serà necessari crear una base de dades. Indica que utilitzarem una base de dades de MySQL Improved (MySQL Mejorado), que anomenarem moodle. Recorda que l'usuari de la base de dades és root (amb contrasenya root).
Al finalitzar la instal·lació hauràs de crear una compta d'usuari per l'administrador (que seràs tu mateix). El nom d'aquest usuari serà admin, amb la contrasenya Administrador_1. A part del nom d'usuari i la contrasenya, també s'ha d'indicar l'email, la població i el país.

2. Aconsegueix que l'idioma predefinit del Moodle sigui el català.

3. Configura els paràmetres de la primera pàgina del lloc indicant com a nom complert Escola d'Ensenyament Secundari Júlia i com a nom curt Escola Júlia. Afegeix també una descripció detallada dels valors i el compromís d'aquesta escola (copia aquesta informació de la web d'alguna altra escola).
A la primera pàgina del lloc no es mostrarà res fins que l'usuari no hagi entrat. Un cap hagi entrat, es mostrarà la llista de categories de cursos i la caixa de text per buscar cursos.

4. Modifica l'aparença del Moodle afegint, i aplicant, un nou tema (que sigui diferent als que incorpora per defecte).
Aconsegueix, també, modificar el favicon de l'aplicació per un personalitzat. I, si el tema que has aplicat ho permet, aconsegueix que es mostri el logo d'aquesta escola.


Part 2: Crear comptes d’usuari definint els privilegis d’accés sobre els recursos d’un sistema de gestió d’aprenentatge a distància

El nostre lloc web ja està totalment configurat i llest per ser utilitzar. El que ara necessitem és crear les comptes d'usuari dels professors i assignar-los als cursos que hauran de gestionar.

1. Afegeix 4 noves categories de cursos: 1er ESO, 2on ESO, 3er ESO i 4rt ESO.

2. Crea els comptes d'usuari pels professors del centre. El nom dels professors són: Pedro Ruiz Gomez, Benito Wolff Ruiz, Angel Lobo Mateo, Claudia Blazquez Tomas i Vicente Puñal Pineda.
La configuració que hauran de tenir aquestes comptes d'usuari es mostra a l'arxiu adjunt número 1 d'aquesta activitat.

3. Assigna a Pedro Ruiz Gomez el rol de creador de cursos.

4. Modifica el rol de creador de cursos per tal d'assignar-li el permís per gestionar les categories de cursos.
Accedeix a Administració del lloc > Usuaris > Definició de rols > Creador de cursos > Editar.

IMPORTANT: imagina't que ets el professor Pedro Ruiz Gomez, accedeix amb la seva compta d'usuari i segueix les indicacions que es mostren a continuació.

5. Afegeix un nou curs a la categoria 1er ESO que s'anomeni Matemàtiques 1 i tingui com a nom curt el codi MAT_1ESO. Les característiques del curs es detallen a continuació:
Indica que el curs va començar el 12 de setembre de 2025. El curs ha de ser visible
El resum del curs el trobaràs a l'arxiu adjunt número 2 d'aquesta activitat. Dóna format al resum per tal de que s'integri perfectament amb el tema que utilitza el lloc web
El curs estarà distribuït en 5 temes i es mostrarà un per pàgina. El temes ocults no es mostraran
L'idioma del curs serà el català
Al curs es mostraran fins a 5 noticies. També han de ser visible les qualificacions i els informes d'activitat
Els fitxers que enviaran els alumnes no superaran els 2 MB de capacitat
No es treballarà en grups
El rol de professor es mostrarà amb el nom Senyor Ruiz

6. Afegeix un altre curs a la categoria 1er ESO que s'anomeni Taulell d'anuncis 1 i tingui com a nom curt el codi TAU_1ESO. Les característiques del curs es detallen a continuació:
Indica que el curs va començar el 12 de setembre de 2025. El curs ha de ser visible
El resum del curs ha de ser Taulell d'anuncis de 1er de la ESO. Dóna format al resum per tal de que s'integri perfectament amb el tema que utilitza el lloc web
El curs tindrà un format social
L'idioma del curs serà el català
No es mostraran ni noticies, ni qualificacions, ni informes d'activitat
Els fitxers que enviaran els alumnes no superaran els 2 MB de capacitat
No es treballarà en grups

7. Afegeix un altre curs a la categoria 1er ESO que s'anomeni Informàtica 1 i tingui com a nom curt el codi INF_1ESO. Les característiques del curs es detallen a continuació:
Indica que el curs va començar el 12 de setembre de 2025. El curs ha de ser visible
El resum del curs el trobaràs a l'arxiu adjunt número 3 d'aquesta activitat. Dóna format al resum per tal de que s'integri perfectament amb el tema que utilitza el lloc web
El curs estarà distribuït en 12 setmanes. Totes les seccions es mostraran en una mateixa pàgina. El temes ocults també seran visibles
L'idioma del curs serà el català
Al curs es mostraran fins a 5 noticies. També han de ser visible les qualificacions i els informes d'activitat
Els fitxers que enviaran els alumnes no superaran els 2 MB de capacitat
Es treballarà en grups. Un alumne/a només podran veure als alumnes que pertanyen al mateix grup. Aquesta configuració s'haurà de complir, obligatòriament, a totes les activitats del curs
El rol de Professor es mostrarà amb el nom Senyor Ruiz. El rol de Professor no-editor es mostrarà amb el nom Senyoreta Blazquez

8. Modifica l'ordre en el que es llisten els cursos de la categoria 1er ESO per tal d'aconseguir que el curs Taulell d'anuncis 1 aparegui a dalt de tot.

9. Afegeix al professor Pedro Ruiz Gomez als cursos Matemàtiques 1 i Informàtica 1, en tots dos casos amb el rol de professor. Afegeix a la professora Claudia Blazquez Tomas al curs Informàtica 1 amb el rol de professor no-editor.
Accedeix al curs Informàtica 1 com a Claudia Blazquez Tomas i comprova les limitacions que té un usuari amb el rol de professor no-editor.

10. Fes les modificacions necessàries per que els usuaris (alumnes) es puguin automatricular als cursos creats als exercicis 5 i 7. Les contrasenyes han de ser, respectivament, mates1 i info1.
Habilita l'accés a visitants, mitjançant la contrasenya guest, al curs creat a l'exercici 6.

11. Anem a activar l'autenticació bassada en el correu electrònic. Accedeix com a administrador a Configuracions > Administració del lloc > Connectors > Autenticació > Gestió de l'autenticació. Ves a la secció Paràmetres comuns i al camp Autoregistre seleccionar l'opció activar Autenticació bassada en el correu electrònic.

12. Registra't com a nou alumne/a del centre i prova d'automatricular-te.
IMPORTANT: el nostre servidor local no té habilitat el servei de correu electrònic. Aleshores, per confirmar el registre d'aquest usuari, hauràs d'iniciar sessió com a administrador i confirmar-lo manualment.


Part 3: Manipular el sistema de gestió d’aprenentatge a distància, afegint continguts i configurant els components de l’aplicació

Ara que els professors ja estan assignats als seus cursos, és hora de començar a afegeir contingut, es a dir, activitats i recursos.
Imagina't que ets el professor Pedro Ruiz Gomez, accedeix amb la seva compta d'usuari al curs Matemàtiques 1, de 1er de la ESO, i segueix les indicacions que es mostren a continuació.

1. Accedeix al curs Matemàtiques 1 i afegeix el títol a cadascun dels 5 temes. Els temes són: Nombres, Equacions de primer grau, Equacions de segon grau, Polinomis i Trigonometria.
Introdueix un resum a cadascun dels temes. Dóna format al resum per tal de que s'integri perfectament amb el tema que utilitza el lloc web.

2. A la part superior del curs apareix una secció que no correspon a cap dels temes (possiblement contingui un fòrum). Afegeix a dalt de tot d'aquesta secció una nova etiqueta que mostri el nom del curs juntament amb una imatge relacionada amb les matemàtiques (tria tu mateix la imatge, tenint en compte que les dimensions han de ser reduïdes).
Dóna format al contingut de l'etiqueta per tal de que s'integri perfectament amb el tema que utilitza el lloc.

3. Afegeix un fòrum (o configura el que apareix per defecte) just per sota de l'etiqueta creada a l'exercici anterior. Aquest fòrum s'anomenarà Fòrum de Matemàtiques 1 i mostrarà com a text d'introducció Si tens dubtes amb l'assignatura, pregunta al fòrum. Indica que el text d'introducció es mostrarà a la pàgina principal del curs i dóna-li format per tal de que s'integri perfectament amb el tema que utilitza el lloc.
Ha de ser un fòrum estàndard (mostrat com si fos un blog) i la subscripció, per part dels participants del curs, es farà de forma automàtica.

4. Afegeix un glossari just per sota del fòrum creat a l'exercici anterior. Aquest glossari s'anomenarà Glossari de Matemàtiques 1 i mostrarà com a text d'introducció Glossari de terminologia matemàtica. Indica que el text d'introducció es mostrarà a la pàgina principal del curs i dóna-li format per tal de que s'integri perfectament amb el tema que utilitza el lloc.
El glossari s'ha de visualitzar en forma de enciclopèdia amb un màxim de 5 entrades per pàgina.
Un cop creat el glossari, afegeix 3 noves entrades (amb un contingut breu): Nombres Enters, Teorema de Pitàgores i Regla de Ruffini. Afegeix, com a mínim, en una de les entrades una imatge.

5. Afegeix un xat just per sota del glossari creat al punt anterior. Aquest xat s'anomenarà El xat del professor i mostrarà com a text d'introducció Xateja amb el teu professor. Indica que el text d'introducció es mostrarà a la pàgina principal del curs i dóna-li format per tal de que s'integri perfectament amb el tema que utilitza el lloc.
Configura el xat indicant que la propera sessió s'iniciarà el pròxim dissabte a les 10 del matí. Les sessions es repetiran a la mateixa hora setmanalment.
Un cop creat el xat, comprova el seu funcionament accedint com a professor i com a participant.

6. Afegeix una enquesta just per sota del xat creat al punt anterior. L'enquesta ha de ser del tipus COLLES (preferit) i s'anomenarà Enquesta de satisfacció.
Un cop creada l'enquesta, comprova el seu funcionament accedint com a participant.

7. Afegeix un enllaç (URL) a la secció de matemàtiques de la web de la XTEC (http://www.xtec.cat/web/recursos/matematiques) just per sota de l'enquesta creada a l'exercici anterior. L'enllaç s'anomenarà XTEC - Matemàtiques, no es mostrarà la descripció a la pàgina principal del curs i s'obrirà en una finestra emergent.

8. Afegeix un accés a una pàgina (que hauràs de crear tu mateix) just per sota de l'enllaç creat a l'exercici anterior. Aquesta pàgina s'anomenarà Criteris d'avaluació de Matemàtiques 1 i mostrarà com a text d'introducció Criteris d'avaluació. Indica que el text d'introducció es mostrarà a la pàgina principal del curs.
Al contingut de la pàgina s'ha de mostrar una taula amb 2 columnes. La primera amb el nom dels temes i la segona amb el pes (en percentatge) que tindrà el tema a la nota final de l'assignatura. La ponderació corresponent és: Nombres (10%), Equacions de primer grau (20%), Equacions de segon grau (25%), Polinomis (15%) i Trigonometria (30%).
Dóna format al contingut de la pàgina per tal de que s'integri perfectament amb el tema que utilitza el lloc.

9. Modifica l'ordre en que es mostren els elements que s'han creat als exercicis anteriors. L'ordre ha de ser el següent: etiqueta, enllaç, pàgina, fòrum, xat, glossari i enquesta.
Part 4: Manipular el sistema de gestió d’aprenentatge a distància, afegint continguts i configurant els components de l’aplicació

Ara que els professors ja estan assignats als seus cursos, és hora de començar a afegeir contingut, es a dir, activitats i recursos.
Imagina't que ets el professor Pedro Ruiz Gomez, accedeix amb la seva compta d'usuari al curs Matemàtiques 1, de 1er de la ESO, i segueix les indicacions que es mostren a continuació.

1. Divideix la secció corresponent al tema Nombres en 3 parts, mitjançant la creació de 3 etiquetes. El nom d'aquestes etiquetes serà Apunts, Exercicis pràctics i Exercicis d'avaluació. Afegeix, a cadascuna de les etiquetes, una imatge (tria tu mateix la imatge, tenint en compte que les dimensions han de ser reduïdes).
Dóna format al contingut de les etiquetes per tal de que s'integri perfectament amb el tema que utilitza el lloc.

2. Afegeix una consulta just per sota de l'etiqueta Exercicis pràctics. Aquesta consulta s'anomenarà Exercici pràctic 1 i la seva descripció serà Quin és el resultat d'aquesta operació: 10 : 2 + 5 · 3 + 4 - 5 · 2 - 8 + 4 · 2 - 20 : 4?. Dóna-li format a la descripció per tal de que s'integri perfectament amb el tema que utilitza el lloc.
Les respostes de la consulta, que es mostraran en vertical, han de ser 5, 9 i 18. No s'ha de permetre canviar la resposta ni tampoc es limitarà el nombre de respostes permeses. Cada cop que un usuari respongui es mostrarà els resultats de la consulta de forma anònima.

3. Afegeix una lliçó just per sota de l'etiqueta Apunts. Aquesta lliçó s'anomenarà Els nombres racionals, mostrarà la barra de progrés, la puntuació acumulada i el menú de l'esquerra (un cop superat el 75% de la lliçó). Es mostrarà en forma de diapositives amb un màxim de 2 respostes a cadascuna.
L'estudiant únicament disposarà d'un intent a cadascuna de les preguntes però, això sí, podrà revisar el contingut de la lliçó en qualsevol moment. Es tracta d'una lliçó de pràctica que es qualificarà sobre 10. L'estudiant podrà repetir la lliçó, conservant la millor qualificació que s'obtingui.
Afegeix a la lliçó 4 pàgines de contingut, intercalades amb 4 pàgines de preguntes de tipus Verdader/Fals (les preguntes encertades tindran un valor de 2 punts, 2 punts, 3 punts i 3 punts, respectivament). Tria tu mateix tan el contingut de les pàgines de ramificació com de les preguntes, tenint en compte que la lliçó correspon als nombres racionals (en aquest enllaç trobaràs informació sobre aquest tema).
Dóna format al contingut de la lliçó per tal de que s'integri perfectament amb el tema que utilitza el lloc.

4. Afegeix un qüestionari just per sota de l'etiqueta Exercicis d'avaluació. Aquest qüestionari s'anomenarà Exercici d'avaluació 1 i estarà disponible el dia 25 de febrer de 9 a 10 del matí. L'estudiant disposarà, com a màxim, de 20 minuts per respondre el qüestionari. Passat aquest temps, els intents oberts s'enviaran automàticament.
L'estudiant només disposarà d'un intent per realitzar el qüestionari. Cada pregunta es mostrarà en una pàgina. Les preguntes sortiran barrejades i, a cada pregunta, les respostes també sortiran barrejades (d'aquesta manera serà més difícil que els alumnes copiïn). Cada cop que l'estudiant respongui a una pregunta se l'informarà si ha encertat, o no. En cas de no encertar-la tindrà una altra oportunitat però amb menor puntuació.
Pel que fa a les opcions de revisió, es mostrarà si es correcta la resposta durant l'intent i totes les opcions de revisió, un cop tancat el qüestionari. Estableix una retroacció global que mostri el missatge Perfecte! si s'obté un encert del 100% i una altra amb el missatge Ui! Casi si s'obté un encert del 45%.
Afegeix al qüestionari 5 preguntes de diferents tipus tenint en compte que el qüestionari correspon als nombres racionals (en aquest enllaç trobaràs informació sobre aquest tema). Cada pregunta tindrà una puntuació màxima de 2 punts, amb una penalització del 25% a cada intent extra.
Dóna format al contingut de les preguntes del qüestionari per tal de que s'integrin perfectament amb el tema que utilitza el lloc.

5. Afegeix una tasca de tipus text en línia just per sota de la consulta creada a l'exercici 11. Aquesta tasca s'anomenarà Exercici pràctic 2 i la seva descripció serà Què són els nombres primers?. Dóna-li format a la descripció per tal de que s'integri perfectament amb el tema que utilitza el lloc.
L'activitat es puntuarà sobre 10 i l'estudiant podrà tornar a realitzar-la encara que ja estigui qualificada.

6. Afegeix una tasca de tipus penjar un fitxer just per sota del qüestionari creat a l'exercici 13. Aquesta tasca s'anomenarà Exercici d'avaluació 2 i la seva descripció serà Elabora un resum d'aquest tema. Dóna-li format a la descripció per tal de que s'integri perfectament amb el tema que utilitza el lloc.
La data límit d'entrega de l'activitat serà el dia 25 de febrer a les 10 del matí, un cop superada aquesta data ja no es podrà entregar. L'activitat es puntuarà sobre 10 i l'estudiant podrà tornar a enviar-la tantes vegades com vulgui.
Part 5: Afegir, i configurar, nous components i plugins en un sistema de gestió d’aprenentatge a distància

En aquesta ocasió, el que volem fer és millorar l'aspecte del curs Matemàtiques 1. Per aconseguir-ho afegirem i configurarem alguns dels blocs (i altres tipus de plugins) que incorpora el Moodle. Accedeix al Moodle amb el compte d'usuari del professor Pedro Ruiz Gomez i segueix les indicacions que es mostren a continuació.

IMPORTANT: Ho hauràs de fer com a administrador.

1. Afegeix els següents blocs: Calendario, Eventos próximos, Usuarios en línea, Mis cursos, Comentarios, Entrada aleatoria del glosario (utilitzant el glossari creat a l'activitat 3), Canal RSS remoto (enllaçat amb l'RSS de les noticies en portada de El periodico i La vanguardia) i Text. Configura aquest últim bloc perquè mostri un llistat amb 3 enllaços externs: xtec (http://www.xtec.cat), Recursos TIC (http://educalab.es/recursos) i Vitutor (http://www.vitutor.com).
Situa els blocs allà on creguis convenient i comprova el seu funcionament. Indica que els blocs Calendario i Eventos próximos seran visibles a totes les pàgines del curs. La resta de blocs només han de ser visibles a la pàgina principal del curs.
2. Afegeix, mitjançant blocs Text, diferents tipus de gadgets:
Busca, amb ajuda d'Internet, un rellotge creat amb javascript i afegeix-lo al curs
Afegeix un gadget per a pàgines web, aquell que trobis més interessant
3. Les insígnies (badges) són una bona forma per celebrar un èxit i mostrar el progrés. Les insígnies es poden atorgar basant-se en una varietat de criteris escollits i es poden mostrar en un perfil d'usuari. Crea 3 insígnies amb l'eina de creació de logos de Canva que es diguin Activitat 1, Activitat 2 i Activitat 3 i personalitza-les com a tu t'agradi. Has de crear 3 activitats amb les quals una vegada l'estudiant les visualitzi es guanyi una insígnia. Per poder personalitzar les insígnies caldrà habilitar el seguiment de compleció de l'activitat a SI. Un cop activat podràs configurar per a cada activitat les condicions per guanyar la insígnia. 
4. Ara que ja hem acabat de configurar el nostre curs, crea una còpia de seguretat de tot el contingut del curs Matemàtiques 1.
Per tal de comprovar el funcionament de la còpia de seguretat, restaura-la en un nou curs que s'anomenarà Matemàtiques 1 backup (amb el nom curt MAT_BCKP).






