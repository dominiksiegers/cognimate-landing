# CogniMate — Landingpage

Marketing-/Referenz-Landingpage für **CogniMate**, einen persönlichen AI „Chief of Staff" (Human-in-the-loop, EU-gehostet, self-hosted).

Die Seite präsentiert das Produkt nach außen und führt Interessenten über ein Kontaktformular zum Erstgespräch („Mit Vertrieb sprechen"). Sie dient zugleich als Referenzprojekt für maßgeschneiderte AI-Assistenz-Entwicklung.

## Aufbau

Eine einzelne, selbst-enthaltene `index.html` — kein Build-Schritt, keine Abhängigkeiten.

- **Zweisprachig** DE/EN (Umschalter, in `localStorage` gemerkt)
- **Dark-/Light-Mode** (folgt System-Einstellung, manuell umschaltbar)
- **Responsive** inkl. Mobile-Navigation
- **Scroll-Reveal**-Animationen (respektiert `prefers-reduced-motion`)
- **Kontaktformular** via [Web3Forms](https://web3forms.com) (AJAX, kein Backend nötig)

## Vor dem Launch — zwei Handgriffe

1. **Kontaktformular verbinden:** Auf [web3forms.com](https://web3forms.com) mit deiner Ziel-E-Mail einen kostenlosen Access-Key holen und in `index.html` den Platzhalter
   `REPLACE_WITH_WEB3FORMS_ACCESS_KEY` (Feld `access_key`) ersetzen.
2. **Sichtbar machen:** Sobald öffentlich auffindbar gewünscht, im `<head>` die Zeile
   `<meta name="robots" content="noindex">` entfernen.

## Lokal ansehen

```bash
python3 -m http.server 4321
# → http://localhost:4321
```

## Hosting

GitHub Pages (Branch `main`, Root). Custom-Domain jederzeit per `CNAME`-Datei nachrüstbar.

---

Entwickelt mit Claude Code. Design-Sprache abgeleitet aus dem CogniMate-Prototyp (Apple × Asana).
