# T03: Serveis de Transferència de Fitxers

## 📝 Breu Descripció

Després d'haver configurat serveis crítics com DHCP, DNS i l'administració remota d'equips durant l'etapa a *EverPia*, arriba el moment d'ampliar competències en el camí en solitari[cite: 1]. Tot i que les plataformes cloud (com Dropbox o Google Drive) són habituals, per esdevenir experts és imprescindible dominar els protocols fonamentals de transferència de dades que operen a la xarxa[cite: 1]. Per aquest motiu, l'equip s'integra en una formació d'especialització tècnica[cite: 1].

---

## 🎯 Objectius de la Formació

En finalitzar aquesta unitat, s'ha de ser capaç de respondre i resoldre amb fets i configuracions reals els següents vectors tecnològics[cite: 1]:
* **Funcionament del protocol FTP:** Arquitectura i mecànica de connexió[cite: 1].
* **Modes de connexió FTP:** Diferències crítiques entre el mode actiu i el mode passiu[cite: 1].
* **Seguretat en entorns tradicionals:** Implementació d'un servidor FTP segur[cite: 1].
* **Alternatives robustes:** Ús del protocol sFTP (sobre SSH) com a substitut de l'FTP tradicional[cite: 1].
* **Aïllament d'entorns:** Engabiat (*chroot*) d'usuaris en connexions SFTP per evitar fuites de seguretat[cite: 1].
* **Diversificació tècnica:** Identificació d'altres mètodes alternatius per a la transferència de fitxers[cite: 1].

---

## 📅 Pla de Treball: Fases del Projecte

La formació s'estructura en dues fases clarament diferenciades per garantir l'assoliment de competències[cite: 1]:

### 📘 1. Fonaments Teòrics i Seguretat
* Estudi profund dels protocols FTP i sFTP[cite: 1].
* Anàlisi de la seguretat en el trànsit de dades, gestió de ports, comportament dels modes actiu/passiu i l'estratègia d'engabiat d'usuaris[cite: 1].

### 💻 2. Laboratori Pràctic (The "Real World")
Implementació tècnica real mitjançant l'ús de màquines virtuals dividida en dos escenaris[cite: 1]:
* **Activitat A (Servidor FTP):** Configuració d'un servidor estàndard, alta d'usuaris, aplicació de restriccions d'engabiat (*chroot*) i assignació de permisos de lectura/escriptura[cite: 1]. S'analitzarà com les dades viatgen "en clar" (sense xifrar) per la xarxa[cite: 1].
* **Activitat B (Servidor sFTP):** Implementació de la transferència de fitxers segura utilitzant el túnel SSH, aprenent a engabiar els usuaris per protegir l'estructura del sistema de fitxers del servidor[cite: 1].

> ⚠️ **Nota de la Consultoria:** Com a administradors de sistemes, la seguretat no és una opció, és una obligació[cite: 1]. Entendre l'arquitectura i vulnerabilitats d'aquests protocols és vital per al futur professional[cite: 1].

---

## 📊 Sistema d'Avaluació

La superació d'aquesta formació es determinarà mitjançant dos formats d'avaluació compartimentats[cite: 1]: