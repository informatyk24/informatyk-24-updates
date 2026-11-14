# Informatyk-24 Updates

Centralne repozytorium wydań i metadanych aktualizacji Informatyk-24 CMS.

## Kanały
- `stable` — wydania stabilne dla środowiska strona5.

## Struktura
- `manifest.json` — metadane aktualnej wersji.
- `changelog.json` — lista zmian.
- `releases/` — paczki ZIP opublikowanych wydań.

## Zasady bezpieczeństwa
- Publikujemy wyłącznie paczki aktualizacyjne i metadane.
- Nie publikujemy kodów dostępu, haseł, tokenów ani danych klientów.
- Każda paczka musi mieć SHA-256, zgodny z manifestem.
- CMS musi weryfikować schemat manifestu, wersję, docelowe środowisko i sumę SHA-256 przed instalacją.
- Sprawdzenie aktualizacji nie instaluje jej automatycznie.

## Status
Repozytorium przygotowywane dla mechanizmu Update Manager 2.0.
