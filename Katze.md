# 🐱🐟 Katze fängt Fisch

Ein kleines Browser-Spiel, gebaut von Fred (10 Jahre) zusammen mit seinem Papa Toby per Vibe Coding mit Claude Code.

---

## 🎯 Was wir bauen wollen

Ein einfaches, buntes Geschicklichkeitsspiel im Browser:

- Eine **Katze 🐱** steht unten am Bildschirm.
- **Fische 🐟** fallen von oben in zufälligen Abständen und an zufälligen Positionen.
- Spieler bewegt die Katze nach **links/rechts**, um die Fische zu fangen.
- Jeder gefangene Fisch = **+1 Punkt**.
- Berührt ein Fisch den Boden → **Game Over**.

---

## 👦 Für wen ist das?

- Hauptspieler: Fred (10 Jahre)
- Soll auch funktionieren auf: Sophias Tablet, Papas Handy, Omas Laptop
- Sprache der UI: **Deutsch** ("Punkte", "Spiel vorbei", "Nochmal spielen")

---

## 🛠️ Technische Anforderungen

- **Eine einzige `index.html`-Datei** mit allem drin (HTML, CSS, JavaScript inline).
  - Grund: einfaches Deployment auf Vercel ohne Build-Step.
- **Keine externen Libraries** (kein React, kein Phaser etc.) – nur Vanilla JS.
- **HTML5 Canvas** für das Spielfeld.
- **Responsive**: Soll auf Desktop UND Smartphone laufen.
- **Touch-Steuerung**: Auf dem Handy soll man die Katze mit dem Finger bewegen können (ziehen oder tippen).
- **Tastatur-Steuerung**: Pfeiltasten ← / → am Desktop.
- Funktioniert offline, sobald die Datei einmal geladen ist.

---

## 🎨 Look & Feel

- **Kinderfreundlich & bunt** (kein dunkles "Gamer"-Theme).
- **Hintergrund**: Hell, freundlich – z.B. Himmelblau mit Wolken, oder eine Wiese.
- **Katze**: Emoji 🐱 als Spielfigur (groß, gut sichtbar, ca. 60–80px).
- **Fisch**: Emoji 🐟 (ca. 40–50px). Optional verschiedene Fisch-Emojis 🐟🐠🐡 für Abwechslung.
- **Punkte-Anzeige**: Oben links, groß und gut lesbar.
- **Game-Over-Screen**: Mittig, mit Endpunktzahl und großem "Nochmal spielen"-Button.
- **Sound** (optional, erst später): kleiner "Plopp" beim Fangen.

---

## 🎮 Spielmechanik – Details

- Katze-Geschwindigkeit: Soll sich smooth anfühlen, nicht zu träge.
- Fisch-Fallgeschwindigkeit: Am Anfang gemütlich, mit jedem Punkt etwas schneller.
- Fisch-Spawn-Rate: Anfangs alle ~1,5 Sek ein neuer Fisch, wird mit der Zeit häufiger.
- Kollisionserkennung: Großzügig – soll Spaß machen, nicht frustrieren.

---

## 🚀 Deployment

- **GitHub-Repo**: `cat-catches-fish` (öffentlich, damit Vercel zugreifen kann).
- **Vercel**: Verbunden mit dem GitHub-Repo, deployed automatisch bei jedem Push.
- **Ziel-URL**: Wird ein vercel.app-Link sein, den wir teilen können.

---

## 📋 Phasen-Plan

### Phase 1: Grundspiel (erst hier zum Laufen bringen!)
- [ ] Katze unten, bewegbar per Pfeiltasten
- [ ] Fische fallen von oben
- [ ] Kollision Katze ↔ Fisch zählt Punkte
- [ ] Game Over wenn Fisch den Boden berührt
- [ ] Neustart-Button

### Phase 2: Mobile & Polish
- [ ] Touch-Steuerung für Handy/Tablet
- [ ] Responsive Layout
- [ ] Game-Over-Screen schön gestalten
- [ ] Schwierigkeitsgrad steigt mit der Zeit

### Phase 3: Extras (nur wenn Fred Lust hat)
- [ ] Highscore (im Browser gespeichert via localStorage)
- [ ] Sound beim Fangen
- [ ] Bombe 💣 als Hindernis (Game Over beim Fangen)
- [ ] Verschiedene Fischsorten mit verschiedenen Punktwerten
- [ ] Goldener Fisch 🌟 als Bonus

---

## 💬 Arbeitsweise mit Claude Code

- Wir arbeiten **iterativ**: Erst das Grundspiel, dann Schritt für Schritt erweitern.
- Fred darf **auf Deutsch** prompten und Wünsche äußern.
- **Kleine Commits** nach jeder funktionierenden Änderung – nicht 100 Sachen auf einmal.
- Nach jeder Änderung: kurz lokal im Browser testen.
- Bei Fehlern: einfach die Fehlermeldung an Claude Code zurückgeben.

---

## 📂 Projektstruktur (Soll-Zustand)

```
cat-catches-fish/
├── index.html       ← Das ganze Spiel
├── Katze.md         ← Diese Datei (Projekt-Briefing)
├── README.md        ← Kurzbeschreibung für GitHub
└── .gitignore       ← Standard für Web-Projekte
```

---

## 🧒 Über Fred (damit du ihn richtig abholst)

- Fred ist 10 Jahre alt und macht hier seine **ersten Schritte im Coding**.
- Er kennt Scratch ein bisschen, hat aber noch keinen "echten" Code geschrieben.
- Bitte erkläre Dinge **kindgerecht und auf Deutsch**, wenn er nachfragt.
- Wenn etwas zu kompliziert wird: einen Schritt zurück und einfacher machen.
- Bei Erfolg: gerne mal Applaus 🎉 – Motivation ist Gold wert.

---

## 🎯 Erstes Ziel

Nach der ersten Session soll Fred ein **funktionierendes Grundspiel** haben, das auf seinem Rechner läuft. Alles Weitere kommt in den nächsten Sessions.

**Los geht's!** 🚀
