# Pràctica 1 — Branques i unions

## Introducció

En aquesta pràctica es treballa amb branques de Git i amb les unions entre branques. També es provoca un conflicte per comprovar el procés de resolució.

## 1. Crear la branca `primera`

Primer es crea una branca anomenada `primera` en el repositori local.

```bash
git branch
git branch primera
git branch
git checkout primera
```

Es comprova que la branca `primera` conté els mateixos fitxers que la branca `main`.

## 2. Crear un fitxer i fusionar la branca

Des de la branca `primera` es crea un fitxer nou i després es fusiona amb la branca principal.

En aquest cas no es produeix cap conflicte perquè el fitxer és nou i no hi havia una modificació diferent del mateix fitxer en la branca principal.

```bash
git merge primera
```

El resultat mostra una fusió *Fast-forward*.

## 3. Esborrar la branca `primera`

Una vegada feta la fusió, s'elimina la branca:

```bash
git branch -d primera
```

## 4. Crear la branca `segona` i provocar un conflicte

A continuació es crea la branca `segona` i es modifica un fitxer.

Després es canvia a `main`, es modifica el mateix fitxer i es fa un altre commit. Quan es prova de fusionar les dues branques apareix un conflicte.

```bash
git merge segona
```

El fitxer presenta els marcadors de conflicte:

```text
<<<<<<< HEAD
Contingut de la branca main
=======
Contingut de la branca segona
>>>>>>> segona
```

## 5. Resoldre el conflicte i sincronitzar la branca

Es modifica el fitxer per deixar el contingut correcte, s'afegeix el canvi i es crea el commit corresponent.

```bash
git add .
git commit -m "He solucionat el conflicte"
```

Finalment, la branca `segona` es sincronitza amb el repositori remot:

```bash
git push origin segona
```

## Conclusió

En aquesta pràctica s'ha treballat amb la creació i eliminació de branques, les unions entre branques i la resolució d'un conflicte de Git.
