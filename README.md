# Marketing-Skill

Ein Skill für Claude. Der Marketing-Skill lernt aus ein paar deiner Texte, wie du klingst, und schreibt dann alles in dieser Stimme: Content-Plan mit Hooks, Antworten auf Google-Bewertungen, Erfolgsgeschichten, Landingpage, Lead Magnet und Newsletter. Der Recycler macht aus einem einzigen Video zehn Posts, ein Karussell, einen Newsletter und drei Reel-Skripte. Kostenlos, MIT-Lizenz.

| Modul | Was es macht |
| --- | --- |
| **Markenstimme** | Aus 3 bis 10 eigenen Texten entsteht ein Stimmprofil: wie du klingst, wie nicht, welche Wörter du nie benutzt. |
| **Content-Plan** | Vier Wochen Content mit fertigen Hooks, Säulen und CTAs, der auf deine Angebote zuläuft. |
| **Bewertungen** | Antworten auf Google-Bewertungen, auch auf die gemeinen. Souverän, datenschutzsicher, in zwei Varianten. |
| **Erfolgsgeschichte** | Ein kurzes Interview, daraus eine Case Study für die Website, eine Kurzfassung für Social Media und ein Einzeiler fürs Angebot. |
| **Recycler** | Ein Video, Podcast oder Artikel wird zu zehn Posts, einem Karussell, einem Newsletter und drei Reel-Skripten. |
| **Landingpage** | Texte für eine Sales- oder Leistungsseite nach bewährtem Aufbau, mit FAQ, Seitentitel und Meta-Beschreibung. |
| **Lead Magnet** | Drei Ideen, dann der fertige Lead Magnet plus Opt-in-Text, Willkommensmail und zwei Nachfass-Mails. |
| **Newsletter** | Aus den Stichpunkten der Woche wird ein Newsletter mit drei Betreff-Varianten. |

## Installation

### Claude-App (Web, Desktop)

Am schnellsten: den Link in einen neuen Chat einfügen und Claude bitten, den Skill zu installieren:

```
https://github.com/Ultra-Smashed/marketing-skill

Installier diesen Skill für mich.
```

Oder von Hand:

1. [`marketing.zip`](https://github.com/Ultra-Smashed/marketing-skill/raw/main/marketing.zip) herunterladen (nicht entpacken).
2. In Claude unter **Settings → Capabilities** den Schalter **Code execution and file creation** einschalten. In der neueren Ansicht heißt er **Create and edit files**.
3. **Customize → Skills** öffnen, auf **+** klicken, dann **Create skill → Upload a skill** und die ZIP-Datei wählen.

Als Plugin: **Customize → Plugins**, bei den persönlichen Plugins auf **+**, dann **Add from a repository** und `Ultra-Smashed/marketing-skill` eintragen.

Die Menünamen stehen hier so, wie Anthropic sie in der Hilfe nennt. In der deutschen Oberfläche können sie übersetzt sein.

### Claude Code

Als Plugin:

```
/plugin marketplace add Ultra-Smashed/marketing-skill
/plugin install marketing@marketing
```

Oder den Ordner kopieren:

```bash
git clone https://github.com/Ultra-Smashed/marketing-skill.git
cp -r marketing-skill/skills/marketing ~/.claude/skills/
```

## Benutzen

Einfach schreiben, was du brauchst, zum Beispiel:

> Lern, wie ich schreibe. Hier sind drei meiner Posts und eine Mail.

> Hier ist das Transkript meines letzten Videos. Mach daraus Content für zwei Wochen.

> Antworte auf diese 1-Stern-Bewertung, souverän und ohne Kundendaten.

Lege die Markenstimme in Claude-Projekten als Projektdatei ab. Dann kennt jeder neue Chat in dem Projekt deinen Ton, ohne dass du ihn neu erklärst.

## Dateien

```
skills/marketing/SKILL.md            Ablauf, Module, Regeln
skills/marketing/modes/               eine Anleitung pro Modul
skills/marketing/references/          Nachschlagewerk
marketing.zip                       derselbe Skill-Ordner als ZIP für die Claude-App
.claude-plugin/                     plugin.json, marketplace.json
```

Nach einer Änderung im Skill-Ordner die ZIP neu bauen: `cd skills && zip -r ../marketing.zip marketing`.

Anleitung: [thanisch.co/wissen/guides/marketing-skill-claude](https://thanisch.co/wissen/guides/marketing-skill-claude)

MIT-Lizenz, siehe [LICENSE](LICENSE). Von [Christopher Thanisch](https://thanisch.co).
