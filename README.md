# CouchHUD Katalog / CouchHUD Catalog

## Deutsch

Das ist der Standard-Katalog für [CouchHUD](https://github.com/kewe87/CouchHUD): eine Liste von Plugins und Skins, die man in CouchHUD direkt installieren und aktualisieren kann (*Einstellungen › Darstellung › Neue Skins installieren* bzw. im Expertenmodus *Plugins & Skins*).

- `index.json` ist der Katalog, `index.json.sig` seine Signatur. CouchHUD vertraut der Standardquelle nur mit gültiger Signatur.
- Die `.zip`-Pakete hängen als Assets an den Releases (Tag `<name>-<version>`, z. B. `wand-1.0.0`). Jeder Eintrag enthält den SHA-256 seines Pakets, ohne passende Prüfsumme wird nichts installiert.
- `skins/` enthält den Quellcode der Skins des Katalogs, `icons/` die Symbole.

### Eintrag einreichen

1. Öffne ein Issue oder einen Pull Request mit dem Link zum **öffentlichen Quellcode** deines Plugins oder Skins und einer kurzen Beschreibung. Format und Paketaufbau stehen in der [Plugin-Dokumentation](https://github.com/kewe87/CouchHUD/blob/master/docs/PLUGINS.md#katalog) und in [SKINS.md](https://github.com/kewe87/CouchHUD/blob/master/docs/SKINS.md).
2. Der Maintainer prüft den Quellcode. Plugins laufen mit den Rechten des Benutzers, deshalb wird nichts ungesehen aufgenommen.
3. Bei positiver Prüfung baut der Maintainer das Paket, legt das Release an, trägt Version und Prüfsumme in `index.json` ein und signiert den Index. **Die Signatur erstellt nur der Maintainer**; der private Schlüssel verlässt seinen Rechner nie. Pull Requests an `index.json` oder `index.json.sig` werden deshalb nicht so übernommen, wie sie sind.

## English

This is the default catalog for [CouchHUD](https://github.com/kewe87/CouchHUD): a list of plugins and skins that can be installed and updated from inside CouchHUD (*Settings › Appearance › Install new skins*, or *Plugins & Skins* in expert mode).

- `index.json` is the catalog, `index.json.sig` its signature. CouchHUD only trusts the default source with a valid signature.
- The `.zip` packages are attached to the releases (tag `<name>-<version>`, for example `wand-1.0.0`). Every entry carries the SHA-256 of its package; nothing is installed without a matching checksum.
- `skins/` holds the source of the catalog's skins, `icons/` the icons.

### Submitting an entry

1. Open an issue or a pull request with a link to the **public source code** of your plugin or skin and a short description. The format and package layout are described in the [plugin docs](https://github.com/kewe87/CouchHUD/blob/master/docs/PLUGINS.md#katalog) and in [SKINS.md](https://github.com/kewe87/CouchHUD/blob/master/docs/SKINS.md).
2. The maintainer reviews the source. Plugins run with the user's rights, so nothing is added unseen.
3. After a positive review the maintainer builds the package, creates the release, adds version and checksum to `index.json` and signs the index. **Only the maintainer signs**; the private key never leaves their machine. Pull requests that change `index.json` or `index.json.sig` are therefore not merged as they are.
