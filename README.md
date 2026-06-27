# trening-tracker
# Trening · badminton

Tracker postępów planu treningowego — badminton, bieganie, siła.

**[→ Otwórz aplikację](https://TWOJ-LOGIN.github.io/NAZWA-REPO/)**

## Co robi

- Pokazuje dzisiejszą sesję wg harmonogramu planu (Pon/Czw badminton, Wt siła A, Śr Z2, Pt siła B, Sob interwały)
- Formularze dopasowane do każdego typu treningu (ciężar + powt. + RPE dla siły, HR recovery dla interwałów, status barku wszędzie)
- Oblicza tonnage, śledzi trend HR recovery i tętna w grze
- Ostrzega przy skoku objętości biegu >10%, rosnącym RPE, dyskomforcie barku
- Wyświetla 8-tygodniowy cykl z aktualną fazą (Adaptacja → Baza → Intensyfikacja → Deload → Ocena)

## Dane

Dane siedzą w `localStorage` przeglądarki — bez backendu, bez konta.

**Backup (rób co tydzień):**
1. Dziś → Ustawienia → Eksport JSON
2. Zapisz do `Google Drive / Trening_2026 / Backup / backup_YYYY-MM-DD.json`

**Przeniesienie na inny telefon / komputer:**
1. Eksport JSON na starym urządzeniu
2. Import JSON na nowym — zastępuje wszystkie dotychczasowe dane

## Struktura projektu

```
index.html       ← cała aplikacja (jeden plik, zero zależności)
README.md
.gitignore
```

## Wdrożenie

GitHub Pages: Settings → Pages → Source: `main` / `/ (root)` → Save.

## Planowane etapy

| Etap | Co | Status |
|------|-----|--------|
| 1 | Formularze + localStorage + wykresy | ✅ gotowe |
| 2 | Rozszerzone statystyki, trend objętości | — |
| 3 | Synchronizacja Google Sheets / Firebase | — |
| 4 | Alerty fatigue, eksport CSV | — |
| 5 | PWA (ikonka na home screen, offline) | — |
