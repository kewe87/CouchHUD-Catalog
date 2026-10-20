# Sicherheit / Security

## Deutsch

Sicherheitsprobleme im Katalog (zum Beispiel ein Eintrag mit Schadcode oder eine falsche Prüfsumme) bitte **vertraulich** über [„Report a vulnerability“](https://github.com/kewe87/CouchHUD-Catalog/security/advisories/new) melden, nicht als öffentliches Issue.

Der Index `index.json` ist signiert (ECDSA P-256, Kontext `couchhud-catalog-v1`). CouchHUD prüft die Signatur mit dem eingebauten Schlüssel, Fingerprint (SHA-256 über SPKI):
`247bba62849ddfeab8749a38488791807bffa33c72347ea20931870dbbb7709f`.
Jeder Download wird außerdem gegen die SHA-256-Prüfsumme im Index geprüft.

Lücken in CouchHUD selbst bitte im [CouchHUD-Repo](https://github.com/kewe87/CouchHUD/security/advisories/new) melden.

## English

Please report security problems in the catalog (for example an entry with malicious code or a wrong checksum) **privately** via ["Report a vulnerability"](https://github.com/kewe87/CouchHUD-Catalog/security/advisories/new), not as a public issue.

`index.json` is signed (ECDSA P-256, context `couchhud-catalog-v1`). CouchHUD checks the signature with its built-in key, fingerprint (SHA-256 over SPKI):
`247bba62849ddfeab8749a38488791807bffa33c72347ea20931870dbbb7709f`.
Every download is also checked against the SHA-256 in the index.

Vulnerabilities in CouchHUD itself belong in the [CouchHUD repository](https://github.com/kewe87/CouchHUD/security/advisories/new).
