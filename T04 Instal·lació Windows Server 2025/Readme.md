# 🖥️ T04 – Instal·lació de Windows Server 2025

## 📌 Breu descripció
Aquest document descriu el procediment d’instal·lació d’un **Windows Server 2025** en una màquina virtual de prova per a l’empresa **TransLògic S.A.**  
L’objectiu és **aprendre el procés**, aplicar **bones pràctiques** i generar una **guia reutilitzable** per a futures implantacions en entorns reals.

---

## 🧩 Introducció al cas
Després del nostre assessorament, **TransLògic S.A.** ens encarrega el desplegament dels seus servidors basats en **Windows Server 2025**.

Abans de la implantació definitiva, es realitza una **instal·lació pilot** mitjançant una màquina virtual que servirà com a:
- 🧪 Entorn de proves  
- 📘 Documentació base  
- 🔁 Referència per a futurs desplegaments  

---

## ⚙️ Configuració de la màquina virtual

### 🖥️ Recursos de maquinari
| Component | Configuració |
|---------|--------------|
| 💾 Memòria RAM | 8 GB |
| 🧠 Processadors | 2 CPU |
| 💽 Disc principal | 32 GB (Sistema Operatiu) |
| 💽 Disc secundari | 10 GB |
| 🌐 Xarxa 1 | NAT |
| 🌐 Xarxa 2 | Host-Only |

---

## 📊 Comparació amb els requisits de Microsoft

### 📝 Requisits mínims de Windows Server 2025 (GUI)
| Component | Requisit mínim Microsoft | VM configurada | ✔️ |
|--------|-------------------------|---------------|----|
| 🧠 CPU | 1.4 GHz, 64 bits | 2 CPU | ✅ |
| 💾 RAM | 2 GB | 8 GB | ✅ |
| 💽 Disc | 32 GB | 32 GB + 10 GB | ✅ |
| 🌐 Xarxa | Adaptador Ethernet | 2 adaptadors | ✅ |

🔎 **Conclusió:**  
La configuració de la màquina virtual **supera àmpliament** els requisits mínims establerts per Microsoft, assegurant un funcionament estable i òptim del sistema.

---

## 💿 Procediment d’instal·lació

### 1️⃣ Creació de la màquina virtual
- Es crea una nova VM amb la configuració definida anteriorment.
- Es munta la **ISO de Windows Server 2025**.

📸 *Captura recomanada:* configuració de CPU, RAM i discos.

---

### 2️⃣ Inici de la instal·lació
- Arrencada des de la ISO.
- Selecció de:
  - 🌍 **Idioma:** English (US)
  - 🕒 **Format regional:** Español (España)
  - ⌨️ **Teclat:** Español

📸 *Captura recomanada:* pantalla de selecció d’idioma.

---

### 3️⃣ Selecció de la versió
- S’escull **Windows Server 2025 – GUI (Desktop Experience)**.

📸 *Captura recomanada:* selecció de versió.

---

### 4️⃣ Particionat de discs
- Instal·lació del SO al **disc principal de 32 GB**.
- El disc secundari queda disponible per a dades futures.

📸 *Captura recomanada:* selecció de disc.

---

### 5️⃣ Finalització de la instal·lació
- Configuració de la contrasenya de l’usuari **Administrator**.
- Accés a l’escriptori del servidor.

📸 *Captura recomanada:* primer inici de sessió.

---

## 🏷️ Configuració inicial del sistema

### 🔤 Canvi del nom de l’equip
- Nom assignat: **DCxx** (on *xx* és el número de llista)

📍 Ruta:

