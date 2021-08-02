---
title: "macOS mit GPG konfigurieren"
description: "<a href='https://m.hrstmnn.de' style='color: white; text-decoration: none;'>← zurück zur Startseite</a>"
---

## GPG im Terminal benutzen

- mit `brew install gnupg pinentry-mac` installieren
- gegebenenfalls `export GPG_TTY=$(tty)` in `~/.zshrc` ergänzen
- Pinentry für GPG
  - ist wie mit <a href="https://gpg4win.org" target="blank">Gpg4win und Kleopatra</a> unter Windows unter anderem ein grafisches Pop-Up zum Passwort eingeben, wenn man den GPG-Key verwendet
  - kann das Passwort anschließend im macOS-Schlüsselbund sichern
  - muss aber noch aktiviert werden, dafür in der Datei `~/.gnupg/gpg-agent.conf` ergänzen: `pinentry-program /usr/local/bin/pinentry-mac`
- Installation testen mit: `echo "test" | gpg --clearsign`

## GPG Suite: Keychain und Services

- mit `brew install --cask gpg-suite` installieren
- <a href="https://gpgtools.tenderapp.com/kb/faq/uninstall-gpg-suite" target="blank">Demo von GPG Mail entfernen</a>

## Konfiguration mit Git

- `git config --global user.signingkey YOUR_GPG_KEY`
- `git config --global commit.gpgsign true`
