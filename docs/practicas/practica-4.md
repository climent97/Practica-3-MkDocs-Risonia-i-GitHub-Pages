# Pràctica 4 — Desplegament en GitHub Pages

## Introducció

Aquesta pràctica continua el projecte de la pràctica 3. L'objectiu és configurar GitHub Actions perquè la documentació es construïsca i es desplegue automàticament en GitHub Pages.

## 1. Crear el workflow

Primer es comprova la branca actual i la connexió amb el repositori remot.

A continuació es crea la carpeta:

```text
.github/workflows/
```

i dins d'ella el fitxer:

```text
deploy.yml
```

El workflow s'encarrega de construir la documentació amb MkDocs i publicar-la en GitHub Pages.

## 2. Configurar GitHub Pages

En el repositori de GitHub es va a:

**Settings → Pages**

i en l'apartat de compilació i desplegament se selecciona:

**GitHub Actions**

GitHub documenta aquest mecanisme com una forma de construir i desplegar llocs de GitHub Pages mitjançant workflows. 

## 3. Comprovar el workflow

Es fa un primer commit i un `push` per comprovar que la integració contínua funciona correctament.

```bash
git add .
git commit -m "Añadimos integracion continua con GitHub Actions"
git push
```

Després, en:

**GitHub → repositori → Actions**

es pot comprovar el resultat del workflow.

## 4. Actualitzar la pàgina automàticament

Es modifica la documentació, concretament `docs/index.md`, i es realitza:

```bash
git add docs/index.md
git commit -m "Actualizacion de la pagina web en markdown"
git push
```

El workflow s'executa de nou i construeix i desplega la nova versió.

## 5. Resultat

En la pràctica es comprova que GitHub Actions finalitza correctament i que la pàgina web queda actualitzada després del `push`, sense haver de fer manualment un `deploy`.

## Flux final

```text
Canvi en Markdown
       ↓
git add
       ↓
git commit
       ↓
git push
       ↓
GitHub Actions
       ↓
mkdocs build
       ↓
GitHub Pages
       ↓
Web actualitzada
```

## Conclusió

Amb GitHub Actions s'automatitza el procés de construcció i desplegament de la documentació. D'aquesta manera, els canvis enviats al repositori poden arribar automàticament a la web.
