# NLPProject

## this is the repository of NLP SS 25 Project at HS Aalen

### Tabelle zur Speicherung der Daten

| Spalte                   | Datentyp       | Beschreibung                                                                                                                 |
| ------------------------ | -------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| `ID`                     | INTEGER / UUID | Eindeutiger Bezeichner der Bewertung                                                                                         |
| `Title`                  | TEXT           | Titel des Spiels                                                                                                             |
| `Subitle`                | TEXT           | Untertitel des Spiels                                                                                                        |
| `URL`                    | TEXT           | URL zur Originalbewertung auf IGN                                                                                            |
| `Author`                 | TEXT           | Autor:in der Bewertung                                                                                                       |
| `Posted`                 | DATE           | Veröffentlichungsdatum der Bewertung                                                                                         |
| `Modified`               | DATE           | Veränderungsdatum der Bewertung                                                                                              |
| `Score`                  | FLOAT          | Bewertung in numerischer Form (z. B. 7.5)                                                                                    |
| `Long_text`              | TEXT           | Vollständiger Bewertungstext (für NLP-Analysen)                                                                              |
| `Review_text`            | TEXT           | Kurzer Text, der vor der Berwetung steht, Zusammenfassung                                                                    |
| `Verdict`                | TEXT           | Unten nach dem Articel finale Zusammenfassung                                                                                |
| `Quotes`                 | TEXT           | Die Fettgedruckten Zitate in den Artikeln                                                                                    |
| `Scraped_at`             | TIMESTAMP      | Zeitpunkt der letzten Erhebung der Daten (z. B. für Aktualität / Logging)                                                    |
| `Tokenized_Long_Text`    | TEXT           | Einzelne Tokens aus dem Text (weiß nicht genau ob wir das überhaupt brauchen ist glaub fast das gleiche wie der Text selbst) |
| `Preprocessed_Long_Text` | TEXT           | Long_Text preprocessed (kleinbuchstaben, lemmatisierung, ohne stoppwörter, zahlen und satzzeichen entfernt)                  |


## Project Struktur

| Datei                                     | Beschreibung                                                                                       |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Classification\_LSTM.ipynb**            | Enthält ein LSTM-Modell zur Textklassifikation (z. B. Review-Bewertung).                           |
| **Classification\_RidgeRegression.ipynb** | Implementiert eine Klassifikation auf Basis Ridge Regression (lineares Modell).                    |
| **crawL\_links.ipynb**                    | Crawlt Links aus Webseiten –  Startpunkt für Datensammlung.                              |
| **links\_scraping.ipynb**                 | Führt Web Scraping auf gecrawlten Links aus, extrahiert Inhalte.                                   |
| **Preprocessing.ipynb**                   | Textbereinigung, Tokenisierung, Stopword-Entfernung.                         |
| **RAG.ipynb**                             | Retrieval-Augmented Generation: Kombination von Information Retrieval + generativer Modellantwort. |
| **sentiment\_analyse.ipynb**              | Analysiert die Stimmung (positiv/negativ/neutral) von Texten.                                      |
| **suchmaschine.ipynb**                    | Enthält eine einfache Suchmaschinen                             |
| **best\_review\_lstm.pth**                |  trainiertes LSTM-Modell                                               |
| **reviews.csv**                           | Liste aller gecrawlten Links                             |
| **scrape\_errors.csv**                    | CSV-Datei mit protokollierten Fehlern beim Scraping.                                               |
| **scraped\_data.db**                      | Lokale SQLite-Datenbank mit den gesammelten Textdaten.                                  |
| **README.md**                             |  Überblick über das Projekt                                      |
