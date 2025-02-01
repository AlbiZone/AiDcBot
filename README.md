# DC-Zone Bot Projekt Struktúra

## 📁 Gyökér Könyvtár
```
/dcbot/
├── 📁 handlers/
│   └── commandHandler.js       # Parancsok kezelése és betöltése
│
├── 📁 src/
│   └── 📁 features/           # Bot parancsok mappája
│       ├── 📁 ai/             # AI parancs
│       │   └── index.js
│       │
│       ├── 📁 help/           # Help parancs
│       │   ├── index.js
│       │   └── commands.js
│       │
│       ├── 📁 math/           # Matematikai parancs
│       │   └── index.js
│       │
│       └── 📁 ping/           # Ping parancs
│           └── index.js
│
├── config.json                 # Központi konfigurációs fájl
├── index.js                   # Bot belépési pont
└── package.json               # Projekt függőségek
```

## 📝 Fájlok Részletezése

### 🔧 Alap Fájlok
- `index.js`: A bot fő belépési pontja. Itt történik:
  - Konfiguráció betöltése
  - Discord kliens inicializálása
  - Parancsok regisztrálása
  - Event handlerek beállítása

- `config.json`: Központi konfigurációs fájl
  - Bot token és kliens ID
  - Feature beállítások
  - Parancsok engedélyezése/tiltása
  - API kulcsok és egyéb beállítások

### 📁 Handlers
- `commandHandler.js`: Parancskezelő rendszer
  - Parancsok dinamikus betöltése
  - Parancsok végrehajtása
  - Parancsok újratöltése

### 📁 Features (src/features/)
Minden parancs saját mappában:

#### 🤖 AI Parancs (ai/)
- `index.js`: Gemini AI integráció
  - AI kérések kezelése
  - Válaszok formázása
  - Várakozási sor kezelése

#### ℹ️ Help Parancs (help/)
- `index.js`: Help parancs logika
- `commands.js`: Parancsok listája és leírása

#### 🔢 Math Parancs (math/)
- `index.js`: Matematikai műveletek
  - Kifejezések értékelése
  - Biztonsági ellenőrzések
  - Eredmények formázása

#### 🏓 Ping Parancs (ping/)
- `index.js`: Egyszerű ping-pong parancs
  - Bot válaszidő mérése
  - API válaszidő mérése

## 🔄 Parancsok Kezelése
1. Minden parancs egy külön mappában található
2. Minden parancsnak van egy `index.js` fájlja
3. A parancsok a következő struktúrát követik:
   - `data`: SlashCommand definíció
   - `name`: Parancs neve
   - `description`: Parancs leírása
   - `execute()`: Parancs végrehajtási logika

## ⚙️ Konfiguráció Kezelése
- Minden parancs beállításai a `config.json`-ban találhatók
- A parancsok ki/bekapcsolása az `enabled` tulajdonsággal
- Különböző beállítások parancsokhoz (pl. API kulcsok, limitek)

## 🔍 Példa Parancs Útvonal
Ha például az AI parancsot keressük:
1. `/dcbot/src/features/ai/index.js`
2. Kapcsolódó konfig: `/dcbot/config.json` -> features.ai szekció
