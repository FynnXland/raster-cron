# raster-cron

Taktgeber für den Discord-Bot „Raster“ des Servers Fynnland Hub. Der Bot läuft als Cloudflare Worker ohne eigenen Cron.
Der Workflow `raster-maintenance` ruft alle 5 Minuten dessen Aufräumlauf auf, damit leere eigene Sprachkanäle von selbst
verschwinden.

Der Aufruf ist durch ein Secret (`RASTER_KEY`) geschützt, das nicht in diesem Repo steht. Ohne Schlüssel antwortet der Worker
mit 403.

Hinweis: GitHub startet geplante Läufe nach bestem Bemühen, einzelne Läufe können sich um einige Minuten verspäten.
