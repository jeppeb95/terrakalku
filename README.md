# Terrarie Kalkulator — Android APK

## Sådan får du din APK (trin for trin)

### Trin 1: Opret GitHub konto
1. Gå til **github.com**
2. Klik "Sign up" og opret en gratis konto

---

### Trin 2: Opret et nyt repository
1. Klik det grønne **"New"** knap (eller gå til github.com/new)
2. Navngiv det `terrarie-kalkulator`
3. Vælg **Public**
4. Klik **"Create repository"**

---

### Trin 3: Upload filerne
1. På dit nye repository, klik **"uploading an existing file"**
2. Upload ALLE filer fra denne mappe — **bevar mappestrukturen!**
   - Du kan trække hele mappen ind i browseren
3. Klik **"Commit changes"**

**Vigtigt:** Filstrukturen skal se sådan ud på GitHub:
```
terrarie-kalkulator/
├── .github/
│   └── workflows/
│       └── build.yml
├── www/
│   └── index.html
├── capacitor.config.json
└── package.json
```

---

### Trin 4: Vent på bygningen (~5-8 minutter)
1. Klik på fanen **"Actions"** øverst i dit repository
2. Du vil se et job køre med navnet "Build Android APK"
3. Vent til den grønne flueben dukker op ✅

---

### Trin 5: Download din APK
1. Klik på det færdige job i Actions
2. Scroll ned til **"Artifacts"**
3. Klik **"terrarie-kalkulator-debug"** for at downloade

---

### Trin 6: Installer på din telefon
1. Overfør APK-filen til din Android-telefon (via USB, mail, Google Drive osv.)
2. Åbn filen på telefonen
3. Hvis Android spørger om tilladelse til at installere fra ukendte kilder → tillad det
4. Følg installationsguiden

---

## Fejl? Tjek dette
- Er alle 4 filer/mapper uploadet korrekt?
- Er `.github/workflows/build.yml` stien bevaret? (`.github` mappen starter med et punktum)
- Klik på det røde kryds i Actions for at se fejlbeskeden
