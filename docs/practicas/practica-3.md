# Pràctica 3 — MkDocs i GitHub Pages

## Introducció

En aquesta pràctica es crea un projecte de documentació amb MkDocs i s'utilitza el tema **Risonia**. Posteriorment, el projecte es publica en GitHub Pages.

## 1. Crear l'entorn virtual

Primer es crea un entorn virtual independent per al projecte.

```bash
python -m venv .venv2
```

Després s'activa l'entorn virtual i s'instal·la MkDocs juntament amb el tema Risonia.

```bash
pip install mkdocs
pip install mkdocs-risonia-theme
```

També es comprova la versió instal·lada de MkDocs.

## 2. Crear el projecte

Es crea la carpeta del projecte i es prepara l'estructura de documentació.

MkDocs utilitza `mkdocs.yml` com a fitxer principal de configuració i la carpeta `docs/` per als documents Markdown.

## 3. Configurar el tema Risonia

En el fitxer `mkdocs.yml` es configura el tema Risonia.

La documentació queda organitzada mitjançant pàgines Markdown.

## 4. Provar la web localment

Per comprovar el resultat abans de publicar-lo es pot executar:

```bash
mkdocs serve
```

Això permet visualitzar el lloc web localment.

## 5. Construir el lloc

Es comprova que el projecte es pot construir correctament:

```bash
mkdocs build
```

MkDocs genera el lloc estàtic dins de la carpeta `site/`.

## 6. Preparar el repositori

Es configura un `.gitignore` per evitar pujar fitxers que no formen part del projecte, com l'entorn virtual i la carpeta generada `site/`.

## 7. Publicar en GitHub Pages

El projecte es puja al repositori de GitHub i es publica en GitHub Pages.

El lloc resultant és:

https://climent97.github.io/Practica-3-MkDocs-Risonia-i-GitHub-Pages/

## Conclusió

En aquesta pràctica s'ha creat una documentació web amb MkDocs, s'ha configurat el tema Risonia i s'ha publicat el resultat mitjançant GitHub Pages.
