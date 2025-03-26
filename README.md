# NLPProject
## this is the repository of NLP SS 25 Project at HS Aalen

### Tabelle zur Speicherung der Daten

| Spalte          | Datentyp        | Beschreibung                                                                 |
|-----------------|-----------------|------------------------------------------------------------------------------|
| `id`            | INTEGER / UUID  | Eindeutiger Bezeichner der Bewertung                                        |
| `game_title`    | TEXT            | Titel des Spiels                                                            |
| `genre??`         | TEXT            | Genre des Spiels (z. B. Action, RPG etc.)                                   |
| `review_url`    | TEXT            | URL zur Originalbewertung auf IGN                                           |
| `author`        | TEXT            | Autor:in der Bewertung                                                      |
| `review_date`   | DATE            | Veröffentlichungsdatum der Bewertung                                        |
| `score`         | FLOAT           | Bewertung in numerischer Form (z. B. 7.5)                                   |
| `review_text`   | TEXT            | Vollständiger Bewertungstext (für NLP-Analysen)                             |
| `scraped_at`    | TIMESTAMP       | Zeitpunkt der letzten Erhebung der Daten (z. B. für Aktualität / Logging)   |
