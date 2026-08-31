# 🌐 Online-Formulare – Hosting-Anleitung

In diesem Ordner liegen fertige Web-Formulare, die du als **Link** verschicken kannst.
Ausfüllungen werden automatisch per E-Mail an **j.poschmann@drk-coe.de** geschickt
(über den kostenlosen Dienst [FormSubmit.co](https://formsubmit.co) – kein eigener Server nötig).

```
online/
├─ index.html                    ← Übersichtsseite mit Links zu beiden Formularen
├─ auszubildende-umfrage.html    ← Umfrage für Auszubildende
├─ fachkraefte-bewertung.html    ← Bewertung durch Fachkräfte
└─ styles.css                    ← Optik (Rot/Weiß, mobilfreundlich)
```

## ⚠️ Wichtig: Erstaktivierung

FormSubmit schickt beim **allerersten** Absenden eines Formulars eine
Bestätigungs-E-Mail an `j.poschmann@drk-coe.de`. Diese einmalig bestätigen
("**Activate Email**" klicken) – danach funktionieren alle weiteren
Absendungen automatisch ohne Bestätigung.

## 🚀 Kostenlos online stellen mit GitHub Pages (empfohlen)

Damit du einen **echten Link** hast, den du per WhatsApp/E-Mail verschicken kannst,
muss die Seite irgendwo öffentlich gehostet werden. GitHub Pages ist kostenlos:

1. Kostenlosen Account auf https://github.com anlegen (falls noch nicht vorhanden).
2. Neues **öffentliches** Repository erstellen, z.B. `drk-umfragen`.
3. Die drei Dateien aus dem `online/`-Ordner hochladen:
   - Im Browser auf der Repo-Seite: **Add file → Upload files**
   - `index.html`, `auszubildende-umfrage.html`, `fachkraefte-bewertung.html`, `styles.css` hineinziehen
   - **Commit changes** klicken
4. Im Repo: **Settings → Pages**
   - Unter "Branch": `main` auswählen, Ordner `/ (root)`, **Save**
5. Nach ca. 1 Minute ist die Seite erreichbar unter:
   ```
   https://DEIN-BENUTZERNAME.github.io/drk-umfragen/
   ```
   - Umfrage-Link: `.../auszubildende-umfrage.html`
   - Bewertungs-Link: `.../fachkraefte-bewertung.html`

Diesen Link kannst du beliebig oft per WhatsApp, E-Mail oder QR-Code teilen.

## 🔄 Alternative ohne GitHub

Falls dir GitHub zu umständlich ist, kannst du stattdessen kostenlose
Drag-&-Drop-Hoster nutzen, z.B. **Netlify Drop**: https://app.netlify.com/drop
– dort einfach den `online/`-Ordner hineinziehen, sofort erhältst du einen Link.

## ✏️ Formular anpassen

Öffne die `.html`-Dateien in VS Code und ändere Text zwischen den `<label>`- oder
`<textarea>`-Tags. Die E-Mail-Adresse für den Empfang steht ganz oben im
`<form action="https://formsubmit.co/...">`-Tag – dort kannst du bei Bedarf
eine andere Adresse eintragen.
