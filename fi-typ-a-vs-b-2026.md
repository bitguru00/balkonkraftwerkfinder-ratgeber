# FI-Schutzschalter Typ A oder Typ B am Balkonkraftwerk

**Autor:** Redaktion Balkonkraftwerkfinder · **Stand:** 26.08.2026 · **Status der Seite:** AI-bearbeitet, redaktionell geprüft

Kurze Antwort: In Wohnungen sitzt fast immer ein FI **Typ A**. Der sieht Wechsel- und pulsierende Gleichfehlerströme. **Typ B** sieht zusätzlich glatte Gleichfehlerströme. Für PV-Wechselstromkreise verlangt DIN VDE 0100-712:2016 grundsätzlich Typ B — **es sei denn**, der Wechselrichter-Hersteller gibt einen anderen Typ frei. Viele Steckersolargeräte bringen eine eigene Fehlerstromüberwachung mit. Das ersetzt keine Elektrofachkraft und ist keine Installationsanweisung.

Shops verkaufen Sets. Die Frage „welcher FI hängt vor meiner Balkondose?“ steht nicht auf der Produktkarte.

## Die drei Typen, ohne Verkäufer-Kürze

| Typ | Was er erkennt | Typische Rolle im Wohnungsbau |
|---|---|---|
| A | Wechselfehlerstrom und pulsierender Gleichfehlerstrom | Standard-FI hinter der Zählerschrank-Verteilung |
| F | zusätzlich Mischfrequenzen (z. B. Frequenzumrichter) | eher Waschmaschine, Wärmepumpe, nicht der Default |
| B | zusätzlich glatte Gleichfehlerströme | oft gefordert, wo Wechselrichter DC-seitig Fehler erzeugen können |

Ein glatter Gleichfehlerstrom kann einen Typ-A-FI so vormagnetisieren, dass er **nicht mehr** zuverlässig auf einen späteren Wechselfehler reagiert. Deshalb ist die Typfrage bei PV keine Geschmacksfrage.

Normbezug (nicht die Volltext-Norm, sondern die Herstellerauslegung dazu): SMA, Technische Information „Kriterien für die Auswahl einer Fehlerstrom-Schutzeinrichtung“, RCD-TI-de-45, Version 4.5. Zitat der dort referenzierten Forderung: Wird eine Fehlerstrom-Schutzeinrichtung für den Schutz des PV-Wechselstrom-Kreises verwendet, muss sie vom Typ B sein. Ausnahme: Der Hersteller des Wechselrichters erteilt die Freigabe für andere RCD-Typen. Datei: [files.sma.de/downloads/RCD-TI-de-45.pdf](https://files.sma.de/downloads/RCD-TI-de-45.pdf) (abgerufen 26.08.2026). Die Information gilt für SMA-Geräteklassen in dem Dokument; sie ist **kein** Freifahrtschein für jeden Mini-WR.

Personenschutz allgemein: DIN VDE 0100-410 (automatische Abschaltung). PV-spezifisch: DIN VDE 0100-712. Steckersolar-Produkt: DIN VDE V 0126-95.

## Was die Steckersolar-Produktnorm zusätzlich macht

Das Umweltbundesamt (Seite „Steckersolargeräte (Balkonkraftwerke)“, zuletzt aktualisiert 18.03.2026) verweist auf die Produktnorm **DIN VDE V 0126-95**. Schuko am Haushaltsstromkreis ist danach nur unter weiteren Schutzmaßnahmen und nur bis zu einer Modulleistung von 960 Watt normgerecht beschrieben; darüber Energiesteckvorrichtung oder Festanschluss durch eine Elektrofachkraft (VDE V 0100-551-1). Quelle: [UBA Steckersolargeräte](https://www.umweltbundesamt.de/themen/klima-energie/erneuerbare-energien/photovoltaik/steckersolargeraete-balkonkraftwerke).

Viele Mini-Wechselrichter führen intern eine Residual-Current-Monitoring-Unit (RCMU). Das ist eine Überwachung **im Gerät**, kein Nachweis, dass der vorhandene Typ-A-FI im Kasten denselben Job macht. Ob der Hersteller Typ A vor dem Gerät **freigibt**, steht im Datenblatt oder in der Konformitäts-/Herstellererklärung — nicht im Shop-Titel.

Anschlussart (Schuko vs. Wieland) ist eine andere Frage als der FI-Typ: [Schuko oder Wieland](https://balkonkraftwerkfinder.de/hilfe/schuko-oder-wieland).

## 800 W Ausgang ist nicht der FI

Die EEG-Sonderregeln seit dem Solarpaket (16.05.2024) gelten für Steckersolargeräte mit **Wechselrichterleistung** bis 800 Watt und **Modulleistung** bis 2.000 Watt. Das sind getrennte Größen. Der FI kennt keine Wp-Zahl. Details: [800-W-Regelung](https://balkonkraftwerkfinder.de/800w-regelung).

Registrierung bleibt: Marktstammdatenregister, ohne Extra-Meldung beim Netzbetreiber in diesen Grenzen. Quelle: [Bundesnetzagentur, Balkon-Solaranlagen](https://www.bundesnetzagentur.de/DE/Fachthemen/ElektrizitaetundGas/ErneuerbareEnergien/Solaranlagen/Balkon_table.html) (abgerufen 26.08.2026). Ablauf: [Anmeldung](https://balkonkraftwerkfinder.de/anmeldung).

Mieter brauchen zusätzlich die Zumutbarkeitsprüfung nach [§ 554 Abs. 1 BGB](https://www.gesetze-im-internet.de/bgb/__554.html) (abgerufen 26.08.2026) — das ist Erlaubnis der baulichen Veränderung, keine Elektroabnahme. Einordnung: [Mieter](https://balkonkraftwerkfinder.de/mieter).

## Was du prüfen kannst, ohne den Kasten umzubauen

1. Welcher FI-Typ steht auf dem vorhandenen Schalter (A, F, B — Aufdruck)?
2. Steht im Wechselrichter-Handbuch eine **ausdrückliche Freigabe** für Typ A, oder nur „RCMU integriert“?
3. Hängt die Balkondose hinter einem FI, der auch Küche/Bad schützt — ein Auslösen legt dann mehr als den Balkon still.
4. Ist die Dose überhaupt dein Wohnungsstromkreis, nicht der Allgemeinstrom? Dazu: der Schwestertext zum Allgemeinstromzähler und [Zwei- oder alter Zähler](https://balkonkraftwerkfinder.de/hilfe/zweirichtungszaehler-alter-zaehler).
5. Kein Gerät tauschen „auf Verdacht“. Auswahl und Einbau bleiben Aufgabe einer Elektrofachkraft; abweichende Herstellerfreigaben gelten nur für das genannte Gerät.

Sets vergleichen, ohne FI-Theater: [Vergleich](https://balkonkraftwerkfinder.de/vergleich). Ertrag hängt von Lage und Verschattung ab: [Rechner](https://balkonkraftwerkfinder.de/rechner). Speicher ändert den FI-Typ nicht von allein: [Speicher nachrüsten anmelden](https://balkonkraftwerkfinder.de/hilfe/speicher-nachruesten-anmelden).

Wir nennen hier keine Preise, keine Pflicht zum Sofort-Tausch und keine Zertifikate, die wir nicht am Gerät geprüft haben.

## FAQ

**Muss ich vor jedem Balkonkraftwerk den FI auf Typ B tauschen?**
Nicht pauschal. DIN VDE 0100-712:2016 fordert Typ B, **wenn** ein FI den PV-Wechselstromkreis schützt — mit Hersteller-Ausnahme für andere Typen. Ob dein Mini-WR unter diese Ausnahme fällt, steht nur in **seiner** Freigabe.

**Reicht der FI Typ A, weil das Set „steckerfertig“ ist?**
Steckerfertig beschreibt die Produktnorm und den Stecker, nicht automatisch den Typ im Zählerschrank. Ohne Herstellerfreigabe für Typ A bleibt die 712-Logik: Typ B.

**Ist das eine Abnahme?**
Nein. Diese Seite ist Recherche. Keine Elektro-, Rechts- oder Sicherheitsberatung. Bei Unsicherheit: Fachkraft plus Datenblatt, nicht Foren-Daumenregeln.

**Quellen (Stand 26.08.2026):** SMA RCD-TI-de-45 Version 4.5 (Verweis auf DIN VDE 0100-712:2016); UBA Steckersolargeräte (18.03.2026); BNetzA Balkon-Solaranlagen; § 554 BGB. Recherche, keine Beratung.
