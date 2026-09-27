# Pràctiques ASIR

> **Documentació tècnica i pràctica d'Administració de Sistemes
> Informàtics en Xarxa**

Benvinguts a la meua documentació de pràctiques. Aquest lloc recull els
treballs, configuracions i procediments realitzats durant el cicle
d'**Administració de Sistemes Informàtics en Xarxa (ASIR)**.

------------------------------------------------------------------------

## 📚 Sobre aquest projecte

Aquest lloc web ha estat creat amb **MkDocs** i el tema **Risonia**, i
està publicat mitjançant **GitHub Pages**.

L'objectiu és centralitzar la documentació de les pràctiques en un únic
lloc, mantenint una estructura clara i fàcil de consultar.

### Tecnologies utilitzades

  Tecnologia           Ús
  -------------------- -------------------------------------
  **MkDocs**           Generació del lloc de documentació
  **Risonia**          Tema visual del lloc
  **Markdown**         Redacció de la documentació
  **Git**              Control de versions
  **GitHub**           Allotjament del repositori
  **GitHub Pages**     Publicació del lloc web
  **GitHub Actions**   Integració i desplegament automàtic

------------------------------------------------------------------------

## 🗂️ Contingut

La documentació s'organitza en diferents apartats per facilitar la
consulta de les pràctiques.

### 🖥️ Administració de sistemes

Documentació relacionada amb l'administració i configuració de sistemes
informàtics.

### 🌐 Xarxes

Pràctiques i configuracions relacionades amb xarxes i serveis de
comunicació.

### 🗄️ Bases de dades

Documentació dels treballs relacionats amb sistemes gestors de bases de
dades.

### 🔐 Seguretat

Procediments i pràctiques relacionats amb la seguretat dels sistemes.

### ⚙️ Implantació d'aplicacions web

Treballs relacionats amb eines i processos de desplegament d'aplicacions
web.

------------------------------------------------------------------------

## 🚀 MkDocs + GitHub Pages

El projecte utilitza MkDocs per convertir els documents Markdown en un
lloc web estàtic.

El procés de treball és:

``` text
Documentació Markdown
        │
        ▼
     MkDocs
        │
        ▼
      site/
        │
        ▼
 GitHub Actions
        │
        ▼
 GitHub Pages
        │
        ▼
     Web pública
```

La pàgina publicada està disponible en:

**[Pràctiques ASIR --- GitHub
Pages](https://climent97.github.io/Practica-3-MkDocs-Risonia-i-GitHub-Pages/)**

------------------------------------------------------------------------

## 🔄 Integració contínua

El projecte incorpora **GitHub Actions** per automatitzar la construcció
i el desplegament de la documentació.

Quan es realitza un canvi en la branca `main`:

``` bash
git add .
git commit -m "Actualització de la documentació"
git push
```

GitHub Actions s'encarrega de:

1.  Descarregar el repositori.
2.  Preparar l'entorn de Python.
3.  Instal·lar MkDocs i Risonia.
4.  Generar el lloc amb `mkdocs build`.
5.  Preparar els fitxers generats.
6.  Desplegar-los en GitHub Pages.

D'aquesta manera, els canvis es poden publicar sense executar manualment
un desplegament amb MkDocs.

------------------------------------------------------------------------

## 🧪 Exemple de treball

El flux habitual per actualitzar la documentació és:

``` bash
# Modificar els fitxers Markdown

git add .

git commit -m "Actualització de la pràctica"

git push
```

Després del `push`, el workflow de GitHub Actions s'encarrega del procés
de construcció i publicació.

------------------------------------------------------------------------

## 📌 Pràctiques

  -----------------------------------------------------------------------
  Pràctica                            Descripció
  ----------------------------------- -----------------------------------
  **Pràctica 2**                      Col·laboració amb GitHub mitjançant
                                      Fork i Pull Request

  **Pràctica 3**                      MkDocs, tema Risonia i GitHub Pages
  -----------------------------------------------------------------------

La **Pràctica 2** inclou el treball amb repositoris, `git clone`,
modificació de fitxers, `fork`, `git push` i creació d'un Pull Request.

La **Pràctica 3** documenta la creació del projecte MkDocs, la
instal·lació del tema Risonia, la generació del lloc web i la publicació
en GitHub Pages.

------------------------------------------------------------------------

## 👨‍💻 Autor

**Cristian Climent Alfonso**

**Cicle formatiu:** Administració de sistemes informàtics en xarxa
(ASIR)

**Assignatura:** Implantació d'Aplicacions Web

------------------------------------------------------------------------

## 🔗 Enllaços

-   **[Web de la
    documentació](https://climent97.github.io/Practica-3-MkDocs-Risonia-i-GitHub-Pages/)**
-   **[Repositori del
    projecte](https://github.com/climent97/Practica-3-MkDocs-Risonia-i-GitHub-Pages)**

------------------------------------------------------------------------

> *Documentació desenvolupada com a part de les pràctiques d'ASIR.*
