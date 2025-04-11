# NLPProject
## this is the repository of NLP SS 25 Project at HS Aalen

### Tabelle zur Speicherung der Daten

| Spalte          | Datentyp        | Beschreibung                                                                 |
|-----------------|-----------------|------------------------------------------------------------------------------|
| `ID`            | INTEGER / UUID  | Eindeutiger Bezeichner der Bewertung                                        |
| `Title`    | TEXT            | Titel des Spiels                                                            |
| `Subitle`    | TEXT            | Untertitel des Spiels                                                            |
| `URL`    | TEXT            | URL zur Originalbewertung auf IGN                                           |
| `Author`        | TEXT            | Autor:in der Bewertung                                                      |
| `Posted`   | DATE            | Veröffentlichungsdatum der Bewertung                                        |
| `Modified`   | DATE            | Veränderungsdatum der Bewertung                                        |
| `Score`         | FLOAT           | Bewertung in numerischer Form (z. B. 7.5)                                   |
| `Long_text`   | TEXT            | Vollständiger Bewertungstext (für NLP-Analysen)                             |
|  `Review_text`  | TEXT            | Kurzer Text, der vor der Berwetung steht, Zusammenfassung |
| `Verdict`| TEXT | Unten nach dem Articel finale Zusammenfassung |
| `Quotes` | TEXT            | Die Fettgedruckten Zitate in den Artikeln   |
| `Scraped_at`    | TIMESTAMP       | Zeitpunkt der letzten Erhebung der Daten (z. B. für Aktualität / Logging)   |
