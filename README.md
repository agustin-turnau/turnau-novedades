# Turnau — Novedades

> ## ⚠️ Esto NO es la app.
>
> Acá no hay código de Turnau y nunca lo hubo: es **marketing**.
> **Todo el producto —app mobile, web, panel, backend— vive en
> [`agustin-turnau/turnau`](https://github.com/agustin-turnau/turnau)**, el monorepo
> principal. Si el problema se ve adentro de la app o del panel, **se arregla allá**.

## Qué hay acá

| | |
|---|---|
| `index.html` | La página de novedades: HTML estático de una sola página, servido por GitHub Pages en `agustin-turnau.github.io/turnau-novedades`. CSS embebido, sin build, sin dependencias, no consume ninguna API |
| `img/mail/` | Los assets de los mails de novedades que salen por Brevo (`vn1-…`, `vn2-…`, `w0–w6`, los "compo") |
| `img/` (raíz) | Las imágenes de la landing |
| `Turnau-Novedades.pdf` | El PDF que Lio manda por WhatsApp |

Nada más. Ni un `.ts`, `.tsx`, `.js`, `.json` ni `.sql` — ni ahora ni en ningún commit
desde que arrancó el repo.

### La trampa

`img/mail/` está lleno de **screenshots y mockups de pantallas reales de la app**
(`vn2-ficha.png` es la ficha médica, `vn1-agenda.png` la agenda, etc.). Es fácil abrir una
de esas imágenes, reconocer la pantalla y pensar que la pantalla se edita acá. **Son
píxeles.** La pantalla se edita en el monorepo.

## Los repos de Turnau

| Repo | Qué es | Cuándo se toca |
|---|---|---|
| [`turnau`](https://github.com/agustin-turnau/turnau) | **El producto entero** (monorepo pnpm: mobile, web, panel, backend) | Todo bug o feature |
| `turnau-novedades` (este) | Marketing: landing, mails, PDF | Solo cuando hay novedades que comunicar |
| `turnau-crminterno` | CRM interno de clientes nuestro, se maneja por separado | Solo para ese CRM |

## Editarlo

Abrí `index.html` en el navegador y listo — no hay que instalar nada.
Las imágenes van comprimidas: los mails de Brevo se abren desde el celular.
