# raster-cron

Teil von [Fynnland](https://fynn.land) · [Discord](https://discord.gg/JTHPxAxFpE)

Taktgeber für den Discord-Bot „Raster“ des Servers Fynnland Hub. Der Bot läuft als Cloudflare Worker ohne eigenen Cron.
Der Workflow `raster-maintenance` ruft alle 5 Minuten dessen Aufräumlauf auf, damit leere eigene Sprachkanäle von selbst
verschwinden.

Der Aufruf ist durch ein Secret (`RASTER_KEY`) geschützt, das nicht in diesem Repo steht. Ohne Schlüssel antwortet der Worker
mit 403.

Hinweis: GitHub startet geplante Läufe nach bestem Bemühen, einzelne Läufe können sich um einige Minuten verspäten.

GitHub schaltet geplante Workflows in öffentlichen Repos ab, wenn 60 Tage lang nichts im Repo passiert. Dann stoppt der
Aufräumlauf, ohne dass etwas fehlschlägt. Abhilfe: unter *Actions* den Workflow `raster-maintenance` wieder einschalten.

## Lizenz

[MIT](LICENSE), Copyright (c) 2026 FynnXland.
