# Publikowanie paczek Informatyk-24

Aby opublikować wydanie automatycznie:

1. Wgraj jeden plik ZIP do katalogu `incoming/` w repozytorium (Add file → Upload files).
2. Zatwierdź commit na gałęzi `main`.
3. GitHub Actions uruchomi workflow **Publish Informatyk-24 update**.
4. Workflow zweryfikuje `release.json`, środowisko `strona5`, integralność ZIP i SHA-256 wszystkich plików.
5. Jeśli walidacja przejdzie, utworzy GitHub Release `vX.Y.Z`, doda ZIP jako asset, zaktualizuje `manifest.json` i `changelog.json`, a następnie usunie tymczasowy ZIP z repozytorium.

Można też uruchomić workflow ręcznie w Actions → Publish Informatyk-24 update → Run workflow i wskazać ścieżkę istniejącego pliku ZIP.

Wymagane uprawnienie workflow: **Settings → Actions → General → Workflow permissions → Read and write permissions**.

Nie umieszczaj w paczkach haseł, tokenów, plików `.env`, kopii baz danych ani danych klientów.
