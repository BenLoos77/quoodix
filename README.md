# Quoodix Website — Onepager

**Stand:** Mai 2026  
**Projekt:** Quoodix · ein Projekt der B77 GmbH

---

## Inhalt dieses Pakets

- `index.html` — Hauptseite (Onepager mit allen Sektionen)
- `impressum.html` — Impressum
- `datenschutz.html` — Datenschutzerklärung
- `README.md` — diese Datei

Alle drei HTML-Dateien gehören in **dasselbe Verzeichnis** auf dem Webserver. Die internen Verlinkungen funktionieren nur, wenn sie zusammenliegen.

---

## Sektionen der Hauptseite

1. **Hero** — Wortmarke, Tagline
2. **Was wir tun** — Manifest mit Audio-Player
3. **01 Beratung** — KI-DNA, mit Audio-Player
4. **02 Tools** — Eigene Tools (Marlo) + individuelle Lösungen
5. **Spotlight: Agenten** — KI-Agenten im Auftrag, mit drei Beispielen
6. **03 Anwendungen** — Bento-Grid mit sieben Anwendungsfeldern
7. **Zitat** — „Industrielle Revolutionen haben den Mittelstand nie gestoppt..."
8. **04 Über uns / Team** — Marken-Story und Founder-Profile
9. **Kontakt** — Erstgespräch-CTA
10. **Footer** — Impressum, Datenschutz, Copyright

---

## Vor dem Live-Gehen unbedingt erledigen

### 1. Impressum vervollständigen

Im `impressum.html` sind drei Platzhalter, die mit echten Daten gefüllt werden müssen:

- **Registergericht** (vermutlich Amtsgericht Siegen, bitte verifizieren)
- **Handelsregisternummer** (HRB ...)
- **USt-ID der GmbH** (eigene neue ID, nicht die alte DE352933500)

Falls die GmbH noch nicht im Handelsregister eingetragen ist:
„B77 GmbH" → vorübergehend „B77 GmbH i. G." (in Gründung) bis Eintragung erfolgt.

### 2. Telefonnummer im Hero/Kontakt-Bereich

In `index.html` steht aktuell der Platzhalter `+49 271 XXX XX XX`. Ersetzen durch die echte Quoodix-Nummer.
Aktuelle Stelle: Suchen nach `+49271XXXXXXX` (im `tel:`-Link) und `+49 271 XXX XX XX` (im sichtbaren Text).

### 3. Echte Beispiel-Agenten oder Status-Pille anpassen

In der Spotlight-Sektion sind drei Beispiel-Agenten mit Status „live im einsatz" markiert:
- Maschinenbau · Angebots-Agent
- Handel & E-Commerce · Service-Agent
- Beratung & Dienstleistung · Recherche-Agent

**Falls diese Agenten noch nicht live bei echten Kunden laufen:** Status auf „beispielhaft" oder ähnliches ändern, oder die Branchen/Inhalte durch echte Cases ersetzen, sobald vorhanden.

### 4. Datenschutzerklärung anwaltlich prüfen lassen

Die mitgelieferte `datenschutz.html` ist eine solide Basis, deckt:
- E-Mail-Kontakt (mailto-Links)
- Web Speech API (Audio-Player)
- Google Fonts (CDN-Hinweis)
- Hosting (generisch beschrieben)
- LinkedIn/Instagram (sind aktuell rausgenommen, daher kein Eintrag dafür)
- DSGVO-Rechte vollständig

**Empfehlung:** Vor Live-Gehen einmal von einem Anwalt oder über eRecht24-Premium prüfen lassen. Spätestens wenn Marlo als SaaS-Produkt live geht, **muss** die Datenschutzerklärung überarbeitet werden (Auftragsverarbeitung, internationale Datenübermittlung, etc.).

### 5. Hosting wählen

Empfehlung für statischen HTML-Onepager:
- **Vercel** (kostenlos, sehr schnell, hervorragend für statische Seiten)
- **Netlify** (kostenlos, ähnliche Qualität)
- **IONOS / Strato** (klassisch, ca. 5 €/Monat, deutsches Hosting)

Im Datenschutz-Text aktuell generisch formuliert. Sobald Hosting feststeht: konkreten Anbieter ergänzen.

### 6. Google Fonts lokal hosten (optional, aber empfohlen)

Aktuell werden „Inter" und „JetBrains Mono" über Google Fonts CDN geladen. Das ist DSGVO-grenzwertig (LG-München-Urteil 2022).

Sicherer Weg: Schriftarten herunterladen (von [google-webfonts-helper](https://gwfh.mranftl.com/fonts)), lokal hosten und im CSS einbinden. Aufwand: ca. 30 Minuten beim Webentwickler.

### 7. Social Media (optional)

Aktuell sind LinkedIn und Instagram aus dem Footer rausgenommen. Sobald die Profile angelegt sind, können sie wieder eingefügt werden — der CSS-Code dafür existiert noch in der Datei.

---

## Audio-Player Hinweis

Die zwei Audio-Player auf der Seite („Ausführliche Version anhören" im Manifest und „Beratung anhören" in der Beratungs-Sektion) nutzen die **Web Speech API** des Browsers — also die im jeweiligen Betriebssystem installierte Sprachsynthese.

Qualität variiert je nach Browser/OS:
- macOS/iOS: gute deutsche Stimmen (Anna, Markus)
- Windows: durchwachsen (Hedda, Stefan)
- Android: stark unterschiedlich

**Falls die Audio-Qualität nicht gefällt:** Eigene MP3-Aufnahmen produzieren (z.B. Benjamin spricht selbst ein, oder professionelle Sprecherin), MP3 hochladen und das JavaScript anpassen, sodass die MP3 abgespielt wird statt der Browser-Stimme.

---

## Marken-Asset Hinweise

- **Markenfarbe:** Cyber Cyan `#00F5FF` als Akzent, sonst Schwarz/Weiß
- **Schriften:** Inter (Body), JetBrains Mono (technische Marker)
- **Markenverb:** quoodixfizieren (ohne mittleres i)
- **Schreibweise:** Quoodix (nur Q groß)
- **Tonalität:** Sie-Form, professionell-warm, subtil genderneutral

---

## Kontakt für Rückfragen

E-Mail: hello@quoodix.io

---

© 2026 Quoodix · ein Projekt der B77 GmbH
