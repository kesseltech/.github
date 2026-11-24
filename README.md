# KesselTech auf GitHub

Dieses Repository enthält das öffentliche Profil der Organisation
[KesselTech](https://github.com/kesseltech). Die Profilseite selbst steht in
[profile/README.md](profile/README.md).

## Inhalt

| Datei | Zweck |
|---|---|
| `profile/README.md` | Öffentliche Profilseite |
| `external/brand/logo/png/` | Logos für helle und dunkle Darstellung, unverändert aus einem Release von `brand` |
| `vendir.yml`, `vendir.lock.yml` | Welche Dateien aus welchem Release (nur freigegebene, kein Manifest) und der genaue Commit |
| `renovate.json` | Renovate hebt das Release-Tag und holt die Dateien neu |
| `scripts/check` | Prüftor: jede im Profil verlinkte Datei existiert |

## Logos

Die Logos kommen aus einem Release des privaten Repos `brand`. vendir holt davon nur die zwei
freigegebenen Dateien nach `external/brand/` (Handbuch CODE-8), kein Manifest und nichts sonst, weil
dieses Repository öffentlich ist. Neue Releases bringt Renovate als PR. Von Hand, mit Lesezugriff auf
`brand` (etwa über `gh auth setup-git`): Tag in `vendir.yml` ändern, `vendir sync`, `scripts/check`.
Die Dateien werden nie bearbeitet. Eine weitere Datei kommt nur nach ausdrücklicher Freigabe in
`includePaths`.

## Pflege

Die Seite ist öffentlich: sachlich, ohne Emojis, im Wortlaut der Website. Die Bildadressen zeigen
absichtlich auf dieses Repository, damit die Seite unabhängig von privaten Repositories funktioniert.
