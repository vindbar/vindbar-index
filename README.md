# vindbar-Index

Welche GEO-Agenturen und KI-SEO-Dienstleister nennen ChatGPT, Gemini, Perplexity, Claude, Google AI Overviews und Google AI Mode, wenn jemand im deutschsprachigen Raum danach fragt? Ich zähle das jeden Monat nach. Hier liegen die Daten dazu offen: jede Antwort im Wortlaut, die Zählung und der Fragensatz.

Die lesbare Fassung steht auf [vindbar.de/vindbar-index](https://vindbar.de/vindbar-index), die vollständige Methodik auf [vindbar.de/vindbar-index/methodik](https://vindbar.de/vindbar-index/methodik).

## Ausgaben

| Ausgabe | Monat | Antworten | Wochenläufe | Festgeschrieben | Spitzengruppe | Meistgenannter, Antworten auf Dienstleisterfragen | vindbar selbst | Seite |
|---|---|---|---|---|---|---|---|---|
| 1 | September 2026 | 1.440 | 4 | 01.10.2026 | Claneo | 310 von 1.077 | 0 von 1.440 | [2026-09](https://vindbar.de/vindbar-index/2026-09) |

Die Spitzengruppe ist ein Band, kein Platz: Anbieter, deren Streuung sich überlappt, stehen gemeinsam darin. Mein eigenes Ergebnis steht in jeder Ausgabe mit in der Zählung.

## So wird gemessen

- **Fragen:** 20 feste Kauffragen (Fragensatz v3), formuliert so, wie Suchende sie tippen. Fragen dürfen hinzukommen, aber nie umformuliert und nie entfernt werden.
- **Systeme:** ChatGPT, Gemini, Perplexity, Claude, Google AI Overviews und Google AI Mode, jedes mit der Websuche seines Anbieters.
- **Weg:** Messung über Schnittstellen, nicht in den Chatfenstern selbst: Perplexity über OpenRouter, ChatGPT, Gemini und Claude über DataForSEO mit der Websuche des jeweiligen Anbieters, Google AI Overviews und Google AI Mode über DataForSEO. Ohne System-Prompt, die Frage als einzige Nachricht eines leeren Gesprächs.
- **Takt:** jeden Montag ein Lauf mit drei Wiederholungen je Frage und System. Am Ersten des Folgemonats wird die Ausgabe festgeschrieben und ändert sich danach nicht mehr.
- **Zählweise:** exakte Wortgrenzen gegen eine gepflegte Anbieterliste mit Aliassen. Zwei Listen, Dienstleister (Agenturen und Personen) und Werkzeuge, jede nur über die Fragen, die nach ihr suchen.
- **Unsicherheit:** Anteil, Standardfehler und Band stehen je Anbieter in den Dateien.

## Dateien

| Pfad | Inhalt |
|---|---|
| `ausgaben/JJJJ-MM.json` | Die Ausgabe: Ranglisten, Wochenwerte, Methodik |
| `ausgaben/JJJJ-MM-dienstleister.csv`, `ausgaben/JJJJ-MM-werkzeuge.csv` | Dieselbe Zählung als Tabelle |
| `wochen/JJJJ-MM-TT.json` | Rohdaten eines Wochenlaufs: jede Antwort im Wortlaut mit Modell-ID, Prompt-Hash und den mitgelieferten Quellen |
| `wochen/JJJJ-MM-TT-auswertung.json` | Auswertung des Laufs: Nennungen je Anbieter, System und Frage |
| `fragensatz/` | Die Fragen mit Absicht und Hash |
| `kalibrierung/` | Die Antworten der echten Gemini-Oberfläche, gegen die der Abrufweg geprüft wurde |

Ausgaben und Wochenläufe sind dieselben Dateien wie unter `https://vindbar.de/daten/`. Jede Ausgabe ist hier ein Release.

## Korrektur

Ausgabe 1: Erstmessung vom 12.09.2026 zurückgezogen und mit Methodikversion 2 neu gemessen. In der Erstmessung haben ChatGPT und Gemini ohne Abruf geantwortet: 0 von 30 Zellen mit Quellen, alle 600 Zitate der Ausgabe stammten aus einer einzigen Engine (Perplexity). Eine Rangliste, die zu zwei Dritteln aus dem Trainingsstand der Modelle besteht, misst nicht, wer in KI-Antworten sichtbar ist. Die zurückgezogene Fassung liegt weiter offen unter `ausgaben/2026-09-methodik1-zurueckgezogen.json`, ihre Rohdaten unter `wochen/2026-09-12.json`. Das Korrekturprotokoll steht in der [Methodik](https://vindbar.de/vindbar-index/methodik#korrektur).

## Zitieren

> Licht, Marco (2026): vindbar-Index, Ausgabe 1, September 2026. vindbar. https://vindbar.de/vindbar-index/2026-09

Die Angaben für Literaturverwaltungen stehen in `CITATION.cff`.

## Lizenz

Die Daten stehen unter [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de). Wer zitiert, nennt die Quelle und das Datum.

## Herausgeber

Marco Licht, [vindbar](https://vindbar.de). Fragen und Korrekturen an marco@vindbar.de oder als Issue in diesem Repository.

## English summary

The vindbar-Index counts every month which GEO agencies and AI search consultants in the German-speaking market (Germany, Austria, Switzerland) are named by ChatGPT, Gemini, Perplexity, Claude, Google AI Overviews and Google AI Mode. 20 fixed buyer questions, three repetitions per question and system every week, one frozen edition per month. This repository holds the verbatim answers, the counts and the question set under CC BY 4.0.
