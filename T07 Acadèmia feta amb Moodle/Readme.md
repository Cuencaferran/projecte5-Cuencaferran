# T07: Acadèmia Digital amb Moodle (Cas: Escola Júlia)

## 📝 Breu Descripció

Aquesta pràctica individual consisteix en el desplegament, personalització, configuració i administració d'un entorn de gestió de l'aprenentatge (*LMS*) basat en **Moodle**[cite: 1]. El projecte simula un encàrrec real per a un client educatiu: l'**Escola Júlia** (un centre d'ensenyament secundari), que requereix un portal digital centralitzat per optimitzar la comunicació i els fluxos d'aprenentatge entre el seu equip docent i l'alumnat[cite: 1].

> ⚠️ **Metodologia d'Avaluació Executiva:** La pràctica es divideix en **5 parts tancades**[cite: 1]. En finalitzar cadascuna de les fases, s'ha d'avisar el docent per fer una **validació en directe i defensa tècnica** del bloc (demostrant on s'ha configurat, el perquè de la decisió i el seu correcte funcionament)[cite: 1].

---

## 📂 Fases del Projecte i Requisits Tècnics

### 🌐 Part 1: Instal·lació, Personalització i Paràmetres Base
* **Allotjament i Base de Dades:** Descompressió del paquet Moodle al servidor web local[cite: 1]. Configuració d'un motor de base de dades **MySQL Improved** anomenat `moodle` (usuari: `root` / contrasenya: `root`)[cite: 1].
* **Compte d'Administrador:** Alta del perfil d'administració principal de la plataforma (`admin` / `Administrador_1`) completant correu, població i país[cite: 1].
* **Idioma i Identitat:** Establir el **català** com a idioma predefinit del lloc[cite: 1]. Configuració del nom complet a `Escola d'Ensenyament Secundari Júlia` i el nom curt a `Escola Júlia`, incloent-hi una descripció de valors del centre[cite: 1].
* **Lògica d'Accés i Disseny Visual:** Configurar la Home perquè no mostri contingut als usuaris anònims; un cop autenticats, visualitzaran la llista de categories i la barra de cerca de cursos[cite: 1]. Instal·lació d'un **tema visual extern** adaptat, configuració de logo corporatiu i un *favicon* personalitzat[cite: 1].

### 👥 Part 2: Estructura Educativa, Usuaris i Permisos
* **Categories de Cursos:** Alta d'estructures per a `1er ESO`, `2on ESO`, `3er ESO` i `4rt ESO`[cite: 1].
* **Cuentas de Docents:** Creació d'usuaris per a Pedro Ruiz, Benito Wolff, Angel Lobo, Claudia Blazquez i Vicente Puñal[cite: 1]. Assignació del rol de **Creador de Cursos** a Pedro Ruiz, modificant els permisos del rol per permetre-li gestionar categories globalment[cite: 1].
* **Aprovisionament de Cursos (Rol: Pedro Ruiz):**
  * `Matemàtiques 1` (`MAT_1ESO`): Inici 12/09/2025, visible, format de 5 temes (un per pàgina), qualificacions visibles, límit de pujada de 2 MB, sense grups i el rol de professor canviat a `Senyor Ruiz`[cite: 1].
  * `Taulell d'anuncis 1` (`TAU_1ESO`): Inici 12/09/2025, format social, sense notícies ni qualificacions visibles, límit de 2 MB, situat a dalt de tot de la llista de la categoria[cite: 1].
  * `Informàtica 1` (`INF_1ESO`): Format de 12 setmanes en una sola pàgina, temes ocults visibles, **Grups separats obligatoris** (un alumne només veu els del seu propi grup), rol de professor com `Senyor Ruiz` i professor no-editor com `Senyoreta Blazquez`[cite: 1].
* **Matriculació i Autoregistre:** Configuració d'automatriculació per a alumnes amb les claus `mates1` i `info1`[cite: 1]. Accés de convidats a Taulell d'anuncis amb la clau `guest`[cite: 1]. Activació de l'**Autoregistre basat en correu electrònic** (amb confirmació manual de l'administrador a causa de la manca de servidor de correu local)[cite: 1].

### 📚 Part 3: Disseny i Recursos del Curs (Matemàtiques 1)
* **Estructuració de Temes:** Definició dels 5 blocs del curs: *Nombres, Equacions de primer grau, Equacions de segon grau, Polinomis i Trigonometria*, incloent un resum formatat per a cadascun[cite: 1].
* **Elements Comuns i Contingut Interactiu:**
  * **Etiqueta superior:** Nom del curs acompanyat d'una imatge matemàtica optimitzada[cite: 1].
  * **Fòrum de Matemàtiques 1:** Format tipus blog amb subscripció automàtica obligatòria[cite: 1].
  * **Glossari de Matemàtiques 1:** Format enciclopèdia (màxim 5 entrades/pàgina) amb definicions per a *Nombres Enters, Teorema de Pitàgores i Regla de Ruffini* (incloent-hi imatges)[cite: 1].
  * **Xat del Professor:** Sessions repetitives configurades setmanalment els dissabtes a les 10:00 AM[cite: 1].
  * **Enquesta i URL:** Integració d'enquesta tipus COLLES (preferit) i enllaç web a la XTEC configurat per obrir-se en una finestra emergent[cite: 1].
  * **Pàgina de Criteris d'Avalació:** Creació d'una taula de ponderacions de nota: Nombres (10%), Equacions 1r (20%), Equacions 2n (25%), Polinomis (15%) i Trigonometria (30%)[cite: 1].
* **Ordre de Visualització Final:** `Etiqueta` ➔ `Enllaç` ➔ `Pàgina` ➔ `Fòrum` ➔ `Xat` ➔ `Glossari` ➔ `Enquesta`[cite: 1].

### 📝 Part 4: Activitats Avançades i Mecanismes d'Avaluació
* **Secció Nombres:** Segmentació mitjançant 3 etiquetes visuals amb icones reduïdes: *Apunts, Exercicis pràctics i Exercicis d'avaluació*[cite: 1].
* **Consulta (Exercici pràctic 1):** Pregunta d'operació combinada amb opcions de resposta (5, 9, 18), publicació de resultats anònims post-votació i llistat vertical[cite: 1].
* **Lliçó Interactiva (Els nombres racionals):** Format diapositives, màxim 2 respostes, barra de progrés activa, puntuació acumulada, menú lateral actiu (al >75%), qualificació sobre 10 (es conserva la millor nota). Inclou 4 pàgines de contingut intercalades amb 4 preguntes de vertader/fals (punts: 2, 2, 3, 3)[cite: 1].
* **Qüestionari Automatitzat (Exercici d'avaluació 1):** Disponible el 25 de febrer de 9:00 a 10:00 AM, temps límit de 20 minuts amb tramesa automàtica d'intents oberts[cite: 1]. Un sol intent permès, preguntes i respostes barrejades per evitar còpies[cite: 1]. Mode interactiu amb penalització del 25% per intent secundari. Retroaccions globals definides al 100% (*"Perfecte!"*) i al 45% (*"Ui! Casi"*)[cite: 1].
* **Tasques:** 
  * *Exercici pràctic 2:* Tipus text en línia (re-lliurable, nota sobre 10)[cite: 1].
  * *Exercici d'avaluació 2:* Tipus enviament de fitxer (data límit: 25 de febrer a les 10:00 AM, bloqueig posterior, nota sobre 10)[cite: 1].

### 🔌 Part 5: Blocs, Plugins de Gamificació i Respatller
* **Enriquiment de Blocs Laterals:** Inserció de *Calendario* i *Eventos próximos* (visibles a tot el curs)[cite: 1]. Inserció d'*Usuarios en línea, Mis cursos, Comentarios, Entrada aleatoria del glosario* i *Canal RSS remoto* (El Periódico / La Vanguardia) visibles només a la Home del curs[cite: 1].
* **Bloc de Text i Gadgets:** Creació de llistat d'enllaços externs (Xtec, Educatlab, Vitutor) i integració mitjançant codi de dos *gadgets*: un rellotge JavaScript i un giny web d'interès d'Internet[cite: 1].
* **Gamificació (Badges / Insígnies):** Habilitar el seguiment de compleció de l'activitat en format "SÍ"[cite: 1]. Dissenyar 3 insígnies a Canva (*Activitat 1, 2 i 3*) i vincular-les a les condicions de visualització i finalització de 3 activitats del curs[cite: 1].
* **Còpia de Seguretat i Auditoria:** Generació d'una còpia de seguretat completa del curs `Matemàtiques 1`[cite: 1]. Validació del fitxer realitzant una restauració completa en un nou curs anomenat `Matemàtiques 1 backup` (`MAT_BCKP`)[cite: 1].

---

## 🏁 Checklist de Control per a la Defensa en Directe

Abans de cridar el professorat per a la validació de cada bloc, assegura't que el teu entorn compta amb els següents elements operatius en pantalla[cite: 1]:
- [ ] **Part 1:** Moodle en català, base de dades connectada, tema visual extern aplicat i favicon personalitzat visible[cite: 1].
- [ ] **Part 2:** Les 4 categories de l'ESO creades, els 5 professors donats d'alta i el sistema de grups separats funcionant correctament a Informàtica 1[cite: 1].
- [ ] **Part 3:** Els 5 temes de Matemàtiques estructurats amb el fòrum, xat setmanal, glossari amb imatges i la taula de ponderacions en l'ordre correcte[cite: 1].
- [ ] **Part 4:** Les 3 seccions de Nombres delimitades, la lliçó de fraccions interactiva amb barra de progrés i el qüestionari amb restricció de temps i data simulat[cite: 1].
- [ ] **Part 5:** Tots els blocs funcionals (RSS i enllaços), els ginys JavaScript actius, les insígnies vinculades a la compleció d'activitats i el curs clonat a `MAT_BCKP`[cite: 1].