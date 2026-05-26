# T06: Configuració del Domini (Active Directory)

## 📝 Breu Descripció

Una vegada el domini base està correctament creat i operatiu, el següent pas crític és el seu desplegament i estructuració mitjançant la creació dels diferents objectes que el componen: grups, usuaris i màquines[cite: 1]. En aquesta unitat es treballarà de manera pràctica la utilitat de segmentar i organitzar aquests objectes utilitzant **Unitats Organitzatives (OUs)**, facilitant així l'administració i la futura aplicació de polítiques de grup[cite: 1].

---

## 🛠️ Procediment Pràctic (Fases de la Configuració)

L'estudiant haurà de realitzar i documentar els següents passos de configuració en l'entorn de servidors[cite: 1]:

### 📁 1. Disseny de l'Estructura d'OUs
* Crear una jerarquia d'**Unitats Organitzatives (OUs)** que sigui coherent amb l'estructura de l'empresa[cite: 1].
* Justificar tècnicament la decisió de la distribució adoptada[cite: 1].

### 👥 2. Definició de Grups de Seguretat
Configurar l'estructura de grups segons els següents perfils operatius[cite: 1]:
* `gestio`[cite: 1]
* `magatzem`[cite: 1]
* `gerencia`[cite: 1]
* `personal` **(Grup global):** Tots els grups anteriors (`gestio`, `magatzem` i `gerencia`) han de ser configurats com a membres d'aquest grup principal[cite: 1].

### 👤 3. Automatització mitjançant Plantilles d'Usuari
Crear una **plantilla d'usuari** específica per a cadascun dels grups (`Gestio`, `Magatzem` i `Gerencia`)[cite: 1]. Cada plantilla ha de tenir preconfigurat:
* La pertinença automàtica al seu grup de seguretat corresponent[cite: 1].
* La ruta de creació de la **carpeta personal** automatitzada al servidor[cite: 1].
* *Validació:* Definir i donar d'alta un usuari de prova real per a cadascuna de les plantilles creades[cite: 1].

### 💻 4. Aprovisionament i Unió de Clients al Domini
* Crear l'objecte d'equip anomenat `PC1` dins de la OU `equips` de l'Active Directory[cite: 1].
* Desplegar una Màquina Virtual (VM) client amb **Windows 11** amb els següents requisits de l'entorn[cite: 1]:
  * Memòria RAM: **4 GB**[cite: 1].
  * Emmagatzematge: Disc suficient per al SO[cite: 1].
  * Configuració de Xarxa: Mode **Xarxa NAT**[cite: 1].
* Un cop instal·lat el sistema, procedir a **agregar l'equip client al domini**[cite: 1].

---

## 🧪 Fase de Validació i QA

> 🚀 **Criteri d'Èxit:** Per comprovar el correcte funcionament de tota la infraestructura, s'ha d'iniciar sessió satisfactòriament a l'equip client `PC1` utilitzant, de forma consecutiva, els **tres usuaris de prova** creats a partir de les plantilles[cite: 1].

---

## 📚 Materials i Links de Suport

* 📑 **UD6.AA3 Desplegament** — Material teòric i guies de configuració disponibles a la plataforma [Moodle de 0224 SOX] de l'assignatura[cite: 1].