# T02: Control de Versions — Treballant amb Git

## 📝 Breu Descripció

Fins ara, la gestió del control de versions s'havia realitzat utilitzant directament la interfície web de GitHub[cite: 1]. Tot i que és una solució funcional, aquesta metodologia presenta limitacions evidents en entorns professionals[cite: 1]:
* **Lentitud en l'edició:** L'editor web és poc versàtil si es compara com un entorn local (com *Visual Studio Code*) o un editor específic de Markdown (com *Ghostwriter*)[cite: 1].
* **Gestió feixuga:** Crear carpetes o afegir fitxers des de la web requereix accions ineficients i lentes[cite: 1].

L'objectiu d'aquesta unitat és fer el salt a la metodologia de treball del món real, **combinant el control de versions local mitjançant el protocol `git` amb un gestor de repositoris remots (GitHub)**[cite: 1].

---

## 💻 El Protocol Git vs. GitHub

És fonamental entendre que `git` i GitHub no són el mateix[cite: 1]:
* **Git:** Creat per Linus Torvalds (el creador de Linux), va néixer abans que GitHub com un protocol de control de versions descentralitzat, trencant amb els sistemes centralitzats de l'època[cite: 1].
* **Remot:** GitHub és la plataforma que allotja aquests repositoris, existint alternatives potents en el mercat com *GitLab* o *Bitbucket*[cite: 1].

---

## 🔄 Flux de Treball Estàndard (Workflow)

El nostre dia a dia operatiu seguirà un circuit de sincronització local-remot molt definit[cite: 1]:

1. **Partida:** Es comença sempre amb un repositori ja existent a GitHub[cite: 1].
2. **Clonació:** El primer pas és descarregar una còpia sincronitzada en local (al disc dur del teu PC)[cite: 1].
3. **Desenvolupament Local:** Tots els canvis, modificacions i edicions es fan exclusivament en local[cite: 1].
4. **Registre de Canvis:** S'aplica el flux clàssic del protocol mitjançant les comandes `git add` i `git commit`[cite: 1].
5. **Sincronització Remota (Pujar):** En finalitzar la jornada de treball, es pugen els canvis cap a GitHub amb un `git push`[cite: 1].
6. **Actualització Local (Baixar):** Abans de reprendre la feina (especialment si canvies d'ordinador entre casa i l'escola), s'executa un `git pull` per assegurar que treballes amb l'última versió del codi[cite: 1].

---

## 📚 Materials i Links de Suport

* 🌐 [Introducció a GitHub](https://github.com/SMX2n/IntroGitHub) — Conceptes bàsics i primers passos amb la plataforma remota[cite: 1].
* 🛠️ [Guia de Control de Versions](https://github.com/SMX2n/ControlVersions) — Manual de referència per al protocol Git i els seus comandaments[cite: 1].