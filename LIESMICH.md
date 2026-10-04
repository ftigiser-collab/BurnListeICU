# BurnICU V1 — Testversion 3.0.0-test10

## Hochladen
Den Ordner `test/` komplett ins Repo **BurnICU** legen (neben die bisherige `index.html`).
Aufruf danach: https://ftigiser-collab.github.io/BurnICU/test/

Die bisherige App unter `/BurnICU/` bleibt unverändert und läuft weiter.

## Speicher
- Testversion speichert unter `burnicu_v3` — getrennt von der alten App (`burnstation_v1`) und von der Besten Liste (`schicht_v1`).
- Demo-Patienten: Menü (⋯) → „Demo-Daten laden". Vor echtem Einsatz über Menü leeren.
- iOS: Eine zum Home-Bildschirm hinzugefügte App hat eigenen Speicher, getrennt vom Safari-Tab.

## Updates
`index.html` ersetzen, in `sw.js` die VERSION hochzählen (`burnicu-v3-test11` …) und in `version.json` die Version anpassen.

## Neu in test10
- Antikoagulation: Retentionswerte (Krea, Harnstoff) werden aus dem Labor übernommen bzw. direkt abgefragt; CrCl (Cockcroft-Gault) und eGFR (CKD-EPI 2021). Fachinfo-Grenzen für Enoxaparin, Dalteparin und Heparin mit Anpassungsvorschlag zum Übernehmen; Hinweise bei steigendem Kreatinin, erhöhter Clearance und niedrigem Gewicht. Erinnerung, wenn Kreatinin fehlt oder älter als 24 h ist.

## Neu in test9
- Menüs auf das Haus zugeschnitten: Viszeral-, Gefäßchirurgie, Gynäkologie und Geburtshilfe entfernt (Diagnosen, Infektfoki, Arztbrief-Baustein, Konsile, Abdomen-Chips); ergänzt um Plastische Chirurgie, UCH und NeuroCH (Diagnosen, Interventionen, Eingriffe, Neuro-/Wund-Befunde, Konsile).
- Inhalationstrauma: AIS 0–4 und Rußausdehnung (Verbrennung und Pulmo-Chips).
- CAM-ICU (Neuro-Chips, schlanker Modus, Fokus bei positiv).
- IAP als Messreihe mit Trend und IAH-Grad (Abdomen), Erinnerung nach Messabstand.
- Verbandswechsel: letzter Wechsel mit Ort, Analgosedierung und Besonderheiten, nächster Termin, Erinnerung mit den Erfahrungen des letzten Wechsels.
- Zugänge & Devices mit Liegetag, Hinweis bei langer Liegedauer bzw. Lage durch verbrannte Haut.
- Toter Code der alten Demo entfernt.

## Neu in test8
- Schlanker Modus: Schalter „schlank“ oben rechts (statt Hell/Dunkel-Knopf; Layout weiter über das Menü ⋯). Pro Patient nur Tag, Diagnose, Verlauf, Hb/Leukozyten/CRP/Krea/Laktat/p/F, Sedierung (inkl. RASS), Analgesie, NA, Diurese, Basislaufrate und großes To-Do-Feld — direkt in „Meine Schicht“ und in der Patientenansicht eintragbar, mit eigenem schlanken Ausdruck.
- Gleiche Daten in beiden Modi: alles, was schlank eingetragen wird, steht im Grundmodus an der passenden Stelle (und umgekehrt).

## Neu in test7
- Antiinfektiva: je Substanz „→ gegen <Erreger des Patienten>“, sonst „empirisch bei <Infektfokus/Infektdiagnose>“, sonst Warnung „Indikation prüfen“ (auch im Fokus). Steht im Infekt-Panel, in der Liste und auf der Übergabe.
- SBT-Vorschlag, wenn PEEP und ASB ≤ 10 cmH2O (mit Voraussetzungen und „vorher klären“), als Erinnerung und im Pulmo-Teil; per Tipp dokumentierbar.
- Ausdruck: Antiinfektiva nur noch im Infekt-Kasten, nicht zusätzlich in der Medis-Zeile.

## Neu in test6
- Basislaufrate der Infusion mit Verlauf: im Diurese-Panel änderbar, im Stundenraster je Stunde unter der Diurese, Änderungen dezent markiert (▴▾); Titrationsvorschlag per Tipp übernehmbar, nach frischer Änderung erst Wirkung abwarten.
- Automatisch verteilte Diurese-Stunden mit kleinem Sternchen (*).
- Katecholamine (mit Trendpfeil und µg/kg/min) in der Hämodynamik, nicht mehr in der Medis-Zeile des Ausdrucks.
- Beatmung im Pulmo-Teil getrennt von den übrigen Pulmo-Befunden (App und Ausdruck).
- Ausdruck: Stundenraster mit zweiter Zeile „Infusion ml/h“.

## Neu in test5
- Diurese: Eintrag = ml seit letztem Eintrag; Lücken werden gleichmäßig auf die Stunden verteilt (≈). Stundenraster der Schicht im Diurese-Panel und vorbefüllt auf dem Ausdruck. Ziel immer auch in ml/h.
- Bilanzziel und „verfehlt“ nur noch dezent, nicht mehr rot, nicht mehr im Fokus.
- To-Do-Reiter: Umschalter nach Priorität / nach Patient.
- Organisation & Aufklärung: Ehegatte/Partner, Betreuer, Aufklärungen Eingriffe/Tracheotomie/Transfusion/PEG — fehlende dezent markiert, steht in Liste, Übergabe und Blanko.
- Druck: Schockphase raus, Fokus je Organsystem, Baustellen umrandet, Labor als eigener Streifen je System, Verlauf vollständig (Aufnahme und letzte 48 h fett), Verlauf auch im Blanko.
- Dopplungen entfernt (Perfusoren, Beatmung, Anti-Xa, Eingriffe, Verlaufsereignisse, Hauptproblem-Zeile).

## Neu in test4
- Bilanzziel-Vorschlag mit „Weg der Findung“ (Phase, ELWI, Lunge, Volumenstatus, kumulative Bilanz, Katecholamine, Laktat, GEDI), per Tipp übernehmbar; verfehltes Bilanzziel wird markiert.
- Bereiche „erledigt für diese Schicht“: automatisch oder per ✓ abhaken, dann minimiert.
- Diagnosevorschläge der Verbrennungs-ITS; Parkland entfernt (mod. Brooke 2 ml/kg/%).
- Labor: Reiter Infekt nach Niere; Parametername antippen → Folgewert direkt eintragen.
- Eingriff „erfolgt“ → Ergebnisfenster mit Befund und Übergabe-Markierung.
- Rate ändern: alte Zahl wird beim Antippen ersetzt (Infusionsrate, Medikamente).
- Vorerkrankungen nur noch in den Stammdaten.
- Infekt-Check Erreger vs. Antiinfektivum; Vancomycin → Spiegel-To-Do automatisch.
- Beatmung strukturiert (BIPAP: Pinsp, PEEP, ΔP automatisch, ASB, FiO2, Spontananteil) mit Trendpfeilen.

## Neu in test3
- Noradrenalin: Standardperfusor 5 mg/50 ml (100 µg/ml). Umrechnung ml/h ↔ µg/kg/min nach Gewicht; Konzentration je Patient unter „Laufende Medikation“ unten änderbar, abweichende Konzentration erscheint in eckigen Klammern.

## Neu in test2
- Fokus & Erinnerungen: relevante Trends automatisch (Labor mit Relevanzschwellen, Katecholamine, Beatmung, Diurese, PiCCO, Anti-Xa, HIT-Verdacht), Erinnerungen als ☐ auf dem Ausdruck.
- Trendpfeile bei Dosisänderung von Perfusoren (Medikament antippen, Dosis ändern).
- Antikoagulation: Enoxaparin/Dalteparin/Heparin i.v., Anti-Xa-Zielbereiche, Dosis nach Gewicht, CrCl, Anpassungsvorschlag, nächster Spiegel.
- Druck: Schreibraum mit Diurese-Stundenraster und Notizzeilen (abschaltbar).

## Abkürzungen
ABSI Abbreviated Burn Severity Index · CPI Cardiac Power Index · ELWI extravaskulärer Lungenwasserindex · GEDI global-enddiastolischer Volumenindex · HI Herzindex · IAP intraabdomineller Druck · ITS Intensivstation · KDIGO Kidney Disease: Improving Global Outcomes · PiCCO Pulse Contour Cardiac Output · POD postoperativer Tag · PWA Progressive Web App · rBaux revidierter Baux-Score · SVRI systemischer Gefäßwiderstandsindex · SW Service Worker · V1 Verbrennungs-ITS · VKOF verbrannte Körperoberfläche · NMH niedermolekulares Heparin · UFH unfraktioniertes Heparin · HIT heparininduzierte Thrombozytopenie · CrCl Kreatinin-Clearance (Cockcroft-Gault) · eGFR geschätzte glomeruläre Filtrationsrate (CKD-EPI) · NA Noradrenalin · FiO2 inspiratorische O2-Fraktion · PEEP positiver endexspiratorischer Druck · p/F Horovitz-Quotient · CRP C-reaktives Protein · ΔP Driving Pressure (Pinsp − PEEP) · Pinsp inspiratorischer Druck · ASB assistierte Spontanatmung · BIPAP Biphasic Positive Airway Pressure · ELWI extravaskulärer Lungenwasserindex · GEDI global-enddiastolischer Volumenindex · MRSA methicillinresistenter S. aureus · ESBL Extended-Spectrum-Betalaktamase · SBT Spontanatmungsversuch (Spontaneous Breathing Trial) · RASS Richmond Agitation-Sedation Scale · CAM-ICU Confusion Assessment Method for the ICU · AIS Abbreviated Injury Score · IAH intraabdominelle Hypertension · ACS abdominelles Kompartmentsyndrom · ZVK zentraler Venenkatheter · PVK peripherer Venenkatheter · DK Dauerkatheter · SPK suprapubischer Katheter · EVD externe Ventrikeldrainage · ICP intrakranieller Druck · CPP zerebraler Perfusionsdruck · VW Verbandswechsel · UCH Unfallchirurgie · NeuroCH Neurochirurgie · Hb Hämoglobin · Krea Kreatinin · PCT Procalcitonin
