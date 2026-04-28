# 🚗 AutoSerwis — PWA Tracker Serwisowy

Prosta aplikacja PWA do śledzenia serwisów samochodowych. Działa offline, zapisuje dane lokalnie na telefonie.

## Instalacja na iPhonie

1. Otwórz link do aplikacji w **Safari**
2. Kliknij ikonę **Udostępnij** (kwadrat ze strzałką w górę)
3. Wybierz **"Dodaj do ekranu głównego"**
4. Gotowe! Apka pojawia się jak normalna aplikacja 📱

## Wdrożenie na GitHub Pages (krok po kroku)

### 1. Załóż konto na GitHub
Wejdź na [github.com](https://github.com) i zarejestruj się (bezpłatne).

### 2. Utwórz nowe repozytorium
- Kliknij **"New repository"**
- Nazwa: `autoserwis` (lub inna)
- Ustaw na **Public**
- Kliknij **"Create repository"**

### 3. Wgraj pliki
Masz dwa sposoby:

**Sposób A — przez przeglądarkę (najprostszy):**
- W repozytorium kliknij **"uploading an existing file"**
- Przeciągnij wszystkie pliki z tego folderu
- Kliknij **"Commit changes"**

**Sposób B — przez terminal (Git):**
```bash
git init
git add .
git commit -m "AutoSerwis PWA"
git remote add origin https://github.com/TWOJA-NAZWA/autoserwis.git
git push -u origin main
```

### 4. Włącz GitHub Pages
- Wejdź w **Settings** → **Pages**
- Source: **Deploy from a branch**
- Branch: **main** / **(root)**
- Kliknij **Save**

### 5. Gotowe!
Po ~2 minutach Twoja apka będzie dostępna pod adresem:
```
https://TWOJA-NAZWA.github.io/autoserwis/
```

## Struktura plików

```
autoserwis/
├── index.html      — główna aplikacja
├── manifest.json   — konfiguracja PWA
├── sw.js           — service worker (offline)
├── README.md       — ta instrukcja
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## Funkcje

- ✅ Śledzenie 4 typów serwisów (olej, opony, przegląd, inne)
- ✅ Statusy: OK / Wkrótce / Zaległe
- ✅ Historia napraw z kosztami
- ✅ Dane zapisywane lokalnie (localStorage)
- ✅ Działa offline
- ✅ Instalowalna na iOS i Android
