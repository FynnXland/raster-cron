# Sicherheitsrichtlinie

## Eine Lücke melden

**Bitte kein öffentliches Issue.** Melde sie privat über GitHub:
[**Schwachstelle melden**](https://github.com/FynnXland/raster-cron/security/advisories/new)
(auch im Tab *Security* des Repos). Schreib dazu, was betroffen ist, wie man es nachstellt und ob du
genannt werden möchtest. Echte persönliche Daten gehören auch in eine private Meldung nicht.

raster-cron wird von einer Person in der Freizeit gepflegt. Eine Antwort kommt innerhalb von 7 Tagen.

## Geltungsbereich

- Das Repo enthält nur den Workflow `raster-maintenance`. Der Schlüssel `RASTER_KEY` liegt als
  GitHub-Secret und nicht im Repo.
- Der Bot Raster läuft als Cloudflare Worker und liegt nicht in diesem Repo.
- Nicht dazu gehören Schwachstellen in GitHub Actions oder bei Cloudflare selbst, die gehören zu den
  jeweiligen Anbietern.
