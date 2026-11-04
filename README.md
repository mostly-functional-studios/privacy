# Mostly Functional Studios – Privacy Page

Eine statische, responsive, zweisprachige Datenschutzerklärung (DE/EN) für GitHub Pages.
Keine Build-Tools, JavaScript-Bibliotheken, Cookies oder extern geladenen Schriftarten.

## Vor Veröffentlichung – unbedingt bearbeiten

Die Seite ist eine **auszufüllende Vorlage**, keine geprüfte Rechtsberatung. Prüfe beide Sprachversionen (`index.html`, `en/index.html`).

1. Suche und ersetze in beiden Dateien:
   - `REPLACE_LEGAL_NAME` → korrekter rechtlicher Name / UG nach Gründung (nicht den Status UG behaupten, bevor er besteht)
   - `REPLACE_POSTAL_ADDRESS` → vollständige ladungsfähige Anschrift
   - `REPLACE_CONTACT_EMAIL` → erreichbare Datenschutz-E-Mail (kommt auch in `mailto:`-Links vor)
2. Entferne in **beiden** HTML-Dateien die `<div class="draft-note" ...>...</div>`-Hinweisbox, **erst nachdem** du alles geprüft hast.
3. Prüfe, ob die App(s) **wirklich** AdMob und Google UMP einsetzen und ob alle aufgelisteten Verarbeitungen zutreffen. Für jede weitere Integration (z. B. Firebase Analytics, Crashlytics, Login, Cloud Saves, In-App-Käufe, AdSense H5 Games Ads, weitere Werbepartner/SDKs) ist die Erklärung zu ergänzen.
4. **Wichtig:** In der App muss der UMP-Datenschutzoptionen-Einstieg unter Einstellungen tatsächlich existieren, wenn UMP ihn verlangt. Der Text auf dieser Seite implementiert den Button **nicht**. Falls der Menüpunkt anders heißt, den Wortlaut in beiden HTML-Dateien anpassen.
5. Bei Kinder-Zielgruppen: Google Play Families Policy, Google Ads-Regeln für Kinder, Einwilligung und gegebenenfalls spezielle Maßnahmen prüfen. Die Vorlage ist hierfür keine pauschale Freigabe.
6. Mit dem Datenschutzformular in **AdMob → Datenschutz und Mitteilungen** und der **Google Play → App-Inhalt → Datensicherheit**-Erklärung abgleichen; keine widersprüchlichen Angaben.
7. Vor Veröffentlichung durch eine fachkundige Person rechtlich prüfen lassen, insbesondere Rechtsgrundlagen, Übermittlungen und Aufbewahrungsfristen.

## GitHub Pages veröffentlichen

1. Erstelle ein öffentliches GitHub-Repository, z. B. `privacy`.
2. Lade **den Inhalt dieses Ordners** hoch, sodass `index.html` direkt im Repository-Hauptverzeichnis liegt (nicht eine Ebene tiefer).
3. Öffne **Settings → Pages → Build and deployment**.
4. Wähle **Deploy from a branch**, **main** und **/(root)**, dann **Save**.
5. Die Seite wird typischerweise unter `https://GITHUB-USERNAME.github.io/privacy/` verfügbar. Die englische Version ist unter `/privacy/en/` erreichbar. Bei einer eigenen Domain kann die URL anders aussehen.
6. Trage die endgültige öffentliche URL in **AdMob → Privacy & messaging** und in der **Google Play Console** ein. Verlinke sie auch im Spielmenü.

## Lokal testen

```bash
python3 -m http.server 8000
```

Dann `http://localhost:8000` und `http://localhost:8000/en/` öffnen.

## Dateien

- `index.html` – Deutsch (Standard)
- `en/index.html` – English
- `assets/styles.css` – gemeinsames responsives Design
- `assets/favicon.svg` – minimalistisches Symbol
- `.nojekyll` – direkte statische Bereitstellung ohne Jekyll

### Quellen für die Prüfung

- Google Play – User Data: https://support.google.com/googleplay/android-developer/answer/10144311
- Google AdMob – European regulations messages: https://support.google.com/admob/answer/10114014
- Google UMP – Android: https://developers.google.com/admob/android/privacy
- GitHub Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

Stand der Vorlage: 04.11.2026.
