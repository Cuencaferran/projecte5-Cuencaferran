# 🏢 T05 – Instal·lació del Domini (Active Directory)

## 📌 Breu descripció
Aquest document descriu el procediment per al **desplegament d’Active Directory Domain Services (AD DS)** sobre el servidor Windows Server 2025 creat a la tasca anterior.

L’objectiu és disposar d’una **Prova de Concepte (PoC)** que permeti validar la configuració abans del desplegament definitiu als sistemes de **TransLògic S.A.**.

---

## 🧩 Introducció
Com a continuació de la tasca **T04 – Instal·lació de Windows Server 2025**, es procedeix a:

- 🏗️ Instal·lar els rols necessaris
- 🌐 Crear un **domini nou dins d’un bosc nou**
- 🔐 Promocionar el servidor com a **Controlador de Domini (DC)**
- ⚙️ Automatitzar el procés mitjançant **PowerShell**

Aquest procediment permet:
- Practicar el desplegament real
- Ajustar paràmetres segons les necessitats del client
- Documentar el procés per a futures implantacions

---

## ⚙️ Procediment a documentar

### 1️⃣ Instal·lació dels rols necessaris

Es procedeix a instal·lar els rols:
- **Active Directory Domain Services (AD DS)**
- **DNS Server** (automàticament requerit)

📍 Ruta gràfica:

📸 *Captura recomanada:* selecció del rol **AD DS**.

---

### 2️⃣ Creació d’un domini nou en un bosc nou

Durant la promoció del servidor:
- 🌲 **Nou bosc**
- 🌐 Nom del domini:  
  **translogicXX.test**  
  *(on XX és el número de llista)*

📸 *Captura recomanada:* selecció “Add a new forest”.

---

### 3️⃣ Nivell funcional del domini i del bosc

- 🆙 **Nivell funcional del bosc:** Windows Server 2025  
- 🆙 **Nivell funcional del domini:** Windows Server 2025

Aquesta configuració permet:
- Accés a totes les funcionalitats modernes d’AD
- Major seguretat i compatibilitat futura

📸 *Captura recomanada:* pantalla de selecció del nivell funcional.

---

### 4️⃣ Promoció del servidor a Controlador de Domini

Durant l’assistent de promoció:
- ✔️ DNS instal·lat
- ✔️ Global Catalog activat
- 🔐 Contrasenya de **Directory Services Restore Mode (DSRM)** configurada

⚠️ **IMPORTANT:**  
És obligatori documentar la **pantalla de resum** abans de confirmar la instal·lació.

📸 *Captura obligatòria:* pantalla **Review Options / Summary**.

Un cop finalitzat el procés:
- 🔄 El servidor es reinicia automàticament
- 🏷️ L’equip passa a ser **DCxx.translogicXX.test**

---

## 🧪 Verificació final
Després del reinici:
- El servidor inicia sessió com a **Administrador del domini**
- Es pot accedir a:

