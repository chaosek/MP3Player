# 🎵 MP3 Player PWA

Jednoduchý MP3 přehrávač jako Progressive Web App s 5 vizualizacemi.  
Funguje v prohlížeči i jako nainstalovaná aplikace na Androidu a PC.

## Vizualizace

| Režim | Popis |
|-------|-------|
| **Bars** | Frekvenční sloupcový analyzátor |
| **Scope** | Osciloskopu — průběh zvukové vlny |
| **Plasma** | Psychedelická plazma reagující na bas/výšky |
| **Circle** | Kruhový spektrální analyzátor |
| **Spectrum** | Duhový spektrogram |

## Jak spustit přes GitHub Pages

1. **Vytvoř nové GitHub repo** (např. `mp3player`)
2. **Nahraj všechny soubory** do rootu repozitáře:
   ```
   index.html
   manifest.json
   sw.js
   icons/
     icon-192.png
     icon-512.png
   README.md
   ```
3. V nastavení repozitáře jdi na **Settings → Pages**
4. Pod „Source" vyber **main branch / root**
5. Klikni **Save** — za chvíli bude app na adrese:
   ```
   https://<tvoje-jmeno>.github.io/<repo-nazev>/
   ```

## Instalace na Android

1. Otevři URL v **Chrome** na Androidu
2. Chrome zobrazí banner „Přidat na plochu" nebo použij menu (⋮) → **Instalovat aplikaci**
3. Aplikace se přidá na domovskou obrazovku a bude fungovat jako nativní app

## Instalace na PC (Chrome / Edge)

- V adresním řádku se zobrazí ikona instalace (⊕)
- Nebo menu → **Instalovat MP3 Player**

## Funkce

- 📂 Nahrání více MP3 souborů najednou → playlist
- ⏮ ⏭ Přepínání skladeb, ⏪ ⏩ přetáčení o 10s
- 📊 5 vizualizací přepínatelných za chodu
- 🔊 Regulace hlasitosti
- 📱 Ovládání ze zámkové obrazovky (Media Session API)
- 📶 Funguje offline po první návštěvě (Service Worker)

## Technologie

- Vanilla JS + Web Audio API
- Canvas 2D vizualizace
- PWA (manifest + service worker)
- Media Session API pro lock screen ovládání
- Žádné závislosti, žádný build step
