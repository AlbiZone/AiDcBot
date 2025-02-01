# ADB Bot 🤖

## A Projekt Története 📖

Hey! 👋

Egy nap arra gondoltam: "Mi lenne, ha csinálnék egy Discord botot úgy, hogy gyakorlatilag fogalmam sincs a programozásról?" Ez a projekt ennek a kíváncsiságnak az eredménye.

Eredetileg azt hittem, hogy csak ennyi lesz:
1. Megkérdezem az AI-t
2. Kimásolom a kódot (Ctrl+C, Ctrl+V)
3. Elindítom a szervert
4. Letesztelem
5. Kész!

Az igazság viszont az, hogy ez a projekt sokkal többé vált. Ahelyett, hogy csak másoltam volna a kódot, elkezdtem érteni, hogy mi miért történik. Rengeteget tanultam a JavaScript-ről, a Discord botok működéséről és általában a programozásról.

## Funkciók 🎮

| Parancs | Leírás |
|---------|---------|
| `/ai`   | AI asszisztens (Gemini) |
| `/math` | Matematikai számítások |
| `/help` | Parancsok és súgó |
| `/ping` | Rendszer státusz |

## Projekt Struktúra 📁

```
dcbot/
│
├── index.js
│   └── (Bot indítási pont)
│
├── config.json
│   └── (Beállítások és kulcsok)
│
├── handlers/
│   └── commandHandler.js
│       └── (Parancskezelő rendszer)
│
└── src/
    └── features/
        ├── ai/
        ├── math/
        ├── help/
        └── ping/
```

## Telepítés 🚀

```bash
# Projekt letöltése
git clone [repo link]

# Függőségek telepítése
npm install

# Config beállítása
# (config.json szerkesztése)

# Bot indítása
node index.js
```

## Tanulási Folyamat 📚

Amit kezdőként tanultam a projekt során:

- JavaScript alapok megértése
- Node.js működése
- API-k használata
- Config fájlok kezelése
- Git alapok
- Discord.js könyvtár használata
- Aszinkron műveletek kezelése
- Hibakeresés és javítás
- Kód strukturálás

## Fontos Figyelmeztetés ⚠️

**⚠️ Kísérleti Projekt - Használat Saját Felelősségre!**

Ez a projekt jelenleg is aktív fejlesztés alatt áll. Rendszeresen érkeznek frissítések és új funkciók, azonban:

1. A kódot nagyrészt AI generálta
2. Nem ment át professzionális biztonsági auditáláson
3. Nem követi az összes fejlesztési best practice-t
4. A GitHub kezelését még tanulom, így a frissítések időnként késhetnek
5. Nem ajánlott éles/production környezetben való használatra

## Fejlesztési Státusz 🔧

A projekt folyamatos fejlesztés alatt áll. Tervezett fejlesztések:
- Új AI modellek integrációja
- További parancsok hozzáadása
- Biztonsági fejlesztések
- Kód optimalizáció
- GitHub workflow beállítása (amint megtanulom a használatát)

## Záró Gondolatok 💭

Ez a projekt bizonyítja, hogy az AI segítségével akár programozói háttér nélkül is el lehet indulni a fejlesztés világában. Bár az eredmény nem tökéletes, a tanulási folyamat és a megszerzett tudás felbecsülhetetlen értékű.

---

*Fejlesztés alatt álló projekt | AI asszisztált fejlesztés | v1.0.0-alpha* ✨
