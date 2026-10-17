# Doko Demo Issho: Let's Gakkou! (PSP) — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Traducción al **español de España**, directamente desde el japonés, de *Doko Demo Issho: Let's Gakkou!*.
Te conviertes en profe de Toro y las demás pokepis: les enseñas palabras, participas en las clases y
actividades del colegio y las acompañas durante el curso, hasta la graduación.

Se distribuye únicamente un **parche**. Necesitas tu propia copia japonesa del juego.

## Estado

Última versión: **[v1.0](https://github.com/johanderohan/doko-demo-issho-lets-gakkou-traduccion-es/releases/tag/v1.0)**. Estado: **en revisión**.

- Guiones, clases, conversaciones, menús, diccionario inicial y textos del ejecutable traducidos.
- Rótulos de la interfaz, horario, mapa del colegio, tienda y pantallas de palabras en castellano.
- Teclado con tildes, ñ, ¡ y ¿; lectura latina para las palabras que enseñas.
- Palabras encadenadas adaptadas a las letras; pestañas del Memo ordenadas por inicial.
- Adaptación de juegos lingüísticos que dependen del japonés, conservando la ambientación de Japón.

### Comprobaciones y límites

Traducción y revisión asistidas por IA, con biblia de términos y voces, revisión editorial de los
lotes, revisión de las palabras insertadas por el jugador y comprobaciones automáticas de etiquetas,
codificación, referencias y memoria. **No ha habido revisión humana independiente.**

Se han realizado recorridos y pruebas dirigidas en PPSSPP: introducción, nombres con letras españolas,
clases de varias familias, enseñarle palabras a las pokepis, menús, tienda, Memo, palabras encadenadas,
despedidas de las cinco pokepis y graduación. Parte de las escenas tardías se alcanzó mediante el
depurador. No equivale a una partida completa desde principio a fin.

El parche se ha reaplicado al original y el resultado se ha comparado byte por byte con la candidata.
La auditoría de la ISO comprueba los 175 guiones, recursos, límites de memoria y referencias del ejecutable,
incluida la simulación de carga en varias direcciones. Las pruebas negativas detectan referencias ausentes.
No se ha probado en PSP real ni en PS Vita con Adrenaline.

Limitaciones conocidas:

- Los nombres y palabras del jugador pueden producir frases peculiares y páginas adicionales.
- Las lecturas largas en mayúsculas pueden ocupar dos líneas en los combates de palabras.
- El logotipo, determinados letreros de ambientación y nombres de los créditos permanecen como en el original.
- El vídeo extra se conserva sin traducir.
- Los servicios de Internet desaparecidos no se restauran. Los modos de red no se han probado entre consolas.
- El ejecutable que recibe otra PSP mediante «Compartir juego» queda fuera de la adaptación de letras españolas.

## Cómo aplicar el parche

La versión compatible es la **ISO japonesa UCJS-10039**, versión de disco 1.01:

| Dato del original | Valor |
|---|---|
| Archivo | `Doko Demo Issho - Let's Gakkou! (Japan).iso` |
| Tamaño | 295.632.896 bytes |
| MD5 | `3ec14cc0e1e4eb7ebe0e9d74ea0a39df` |
| SHA-256 | `5a6df905dc0fd487c825927c8e603d067b741354c6acc3a1df73b0ac4e4ac4cd` |

Descarga el archivo `.xdelta` de **[Releases](https://github.com/johanderohan/doko-demo-issho-lets-gakkou-traduccion-es/releases)**.
Aplícalo directamente sobre el original con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o xdelta3:

```bash
xdelta3 -d -s "Doko Demo Issho - Let's Gakkou! (Japan).iso" Doko.Demo.Issho.Lets.Gakkou.ES.v1.0.xdelta "Doko Demo Issho - Let's Gakkou! (ES).iso"
```

La ISO resultante debe medir **317.407.232 bytes** y tener MD5 **`dc042776426a7be9cdb8fbb8630f6a76`**.

| Huella SHA-256 | Valor |
|---|---|
| ISO traducida | `89d8e9d9b7a0dc12eac9d185d786974edf48372bed4227b663e48b34b5ed8cfa` |
| Parche xdelta | `7674283e7c5a9d26e0011a0e36c3d2641a303d0c7879dc5015022d2ba311d03b` |

El ejecutable de la ISO traducida no está cifrado; su uso en consola requiere un entorno compatible.

## Cambios

### v1.0 — 17 de octubre de 2026

- Primera versión de la traducción: guiones, clases, menús, diccionario y rótulos de interfaz.
- Teclado con letras españolas, encadenadas por letras y Memo por inicial.
- Ajustes del horario, descripciones de disfraces y referencias reubicables del ejecutable.

## Créditos

- Traducción, revisión, herramientas y parche: johanderohan, con ayuda de IA.
- Pruebas y depuración con PPSSPP.
- Tipografía de los rótulos: M PLUS Rounded 1c, licencia SIL OFL 1.1.

Si encuentras una errata o un problema, abre una [incidencia](https://github.com/johanderohan/doko-demo-issho-lets-gakkou-traduccion-es/issues) con una captura y la escena.

## Aviso

Proyecto de traducción no oficial, sin relación con Sony Interactive Entertainment.
No se distribuye la ISO: el parche requiere una copia del juego que ya tengas.
