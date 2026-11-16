# Lernkarten Modul 2 · Prozessaufnahme und Modellierung

84 Karten. Grundlage: Begleitskript Modul 2 (Stand 18.06.2026). Dazu kommen die 10 Quizfragen und die 20 Kurs-Flashcards (Dubletten zusammengeführt, Tag Kurs-Flashcard). Karten mit **[Eigener Selbstcheck]** (Kapitel 4) und **[Ergänzung]** stammen nicht aus dem Skript und sind gekennzeichnet.

Anki-Import: `modul2_lernkarten_anki.csv` (Notiztyp „Einfach“, Trennzeichen und Tags werden automatisch erkannt).


## Kapitel 1 · Prozesse aufnehmen, bevor man sie modelliert

**1. Was besagt das Bild vom Prozess-Eisberg?**

Nur ein kleiner Teil der Prozessrealität ist auf den ersten Blick sichtbar. Darunter liegen Workarounds, Ausnahmen, Medienbrüche und implizites Wissen.

**2. Warum ist die Ist-Aufnahme die Grundlage jeder Prozessoptimierung?**

Ohne sauberes Ist gibt es kein gutes Soll.

**3. Welche drei Methoden der Prozessaufnahme gibt es, und wie sollte man sie einsetzen?**

Interview, Beobachtung (Gemba) und Dokumentenanalyse, im Idealfall kombiniert.  
  
<i>Kurs-Flashcard: „Nenne drei Methoden der Prozessaufnahme.“</i>

**4. Interview als Aufnahmemethode: Stärke und Schwäche?**

Stärke: tiefste Einblicke.  
Schwäche: abhängig vom Gesprächspartner.

**5. Beobachtung (Gemba) als Aufnahmemethode: Was ist das und was ist ihre Stärke?**

„Geh dorthin, wo die Arbeit passiert“. Zeigt die tatsächliche statt der dokumentierten Realität.

**6. Dokumentenanalyse als Aufnahmemethode: Stärke und Schwäche?**

Stärke: breiter Überblick.  
Schwäche: Dokumente sind oft veraltet oder idealisiert.

**7. Wie kann KI bei der Dokumentenanalyse helfen?**

KI (z. B. Claude/ChatGPT) hilft, Prozessschritte aus QM-Handbüchern und E-Mails zu extrahieren.

**8. Welche Fragetechnik nutzt man im Prozess-Interview?**

Offene Fragen („Erzähl mir, wie das abläuft“) statt geschlossener; W-Fragen systematisch stellen; bei Selbstverständlichkeiten nachhaken.

**9. Welche sechs W-Fragen stellst du im Prozess-Interview systematisch?**

Wer, Was, Wann, Wie, Womit, Warum.

**10. Nenne die drei typischen Fallen im Prozess-Interview.**

1) Suggestivfragen  
2) Den Wunschprozess statt der Realität erfassen  
3) Nur Führungskräfte befragen

**11. Wer ist die Primärquelle bei der Prozessaufnahme?**

Die Prozessausführenden, nicht die Führungskräfte.

**12. Selbstcheck 1.1: Was meint der Prozess-Eisberg und welche Konsequenz hat er für die Aufnahme?**

Nur die Spitze der Prozessrealität ist sichtbar; darunter liegen Workarounds, Ausnahmen, Medienbrüche und implizites Wissen.  
Konsequenz: Man darf sich nicht auf das Offensichtliche oder Dokumentierte verlassen, sondern muss Methoden kombinieren (v. a. Beobachtung, Nachhaken bei Selbstverständlichkeiten), um das echte Ist zu erfassen. Ohne sauberes Ist kein gutes Soll.

**13. Selbstcheck 1.2: Nenne die drei Aufnahmemethoden mit je einer Stärke und Schwäche.**

Interview: + tiefste Einblicke / − abhängig vom Gesprächspartner  
Beobachtung (Gemba): + zeigt die tatsächliche Realität / − (nicht im Skript genannt; typisch: aufwändig, Beobachtete verhalten sich evtl. anders)  
Dokumentenanalyse: + breiter Überblick / − oft veraltet oder idealisiert

**14. Selbstcheck 1.3: Warum sind die Prozessausführenden wichtiger als die Führungskraft?**

Sie sind die Primärquelle: Sie kennen die tatsächliche Arbeit inkl. Workarounds, Ausnahmen und implizitem Wissen. Führungskräfte beschreiben eher den Wunsch- oder Sollprozess.


## Kapitel 2 · BPMN-Grundlagen

**15. Wofür steht BPMN, und welcher Standard liegt BPMN 2.0 zugrunde?**

Business Process Model and Notation; standardisiert als ISO/IEC 19510.  
  
<i>Kurs-Flashcard: „Was bedeutet BPMN?“</i>

**16. Warum ist BPMN als gemeinsame Prozesssprache wertvoll?**

Fachabteilung, IT und Management können sie gleichermaßen lesen, vergleichbar mit Noten in der Musik.

**17. Was bedeutet die 80/20-Regel bei BPMN?**

Mit wenigen Grundelementen modellierst du die meisten Prozesse.

**18. Nenne die Grundbausteine von BPMN.**

Events, Activities, Gateways, Sequence Flow, Message Flow, Pools und Lanes.

**19. Welche drei Arten von Events unterscheidet das Skript?**

Start-, Zwischen- und End-Event.

**20. Wofür stehen in BPMN Activities, Gateways sowie Pools und Lanes?**

Activities: Aufgaben  
Gateways: Verzweigungen  
Pools und Lanes: Beteiligte und Rollen

**21. Was ist der Unterschied zwischen Sequence Flow und Message Flow?**

Sequence Flow: Ablauf innerhalb eines Pools.  
Message Flow: Kommunikation zwischen Pools.  
  
<i>Kurs-Flashcard: „Was unterscheidet Sequence Flow von Message Flow?“</i>

**22. Nenne die fünf häufigsten BPMN-Anfängerfehler.**

1) Kein Start- oder End-Event  
2) Gateways nicht geschlossen (jeder Split braucht einen Join)  
3) Bedingungen an Pfeilen vergessen (Default Flow markieren)  
4) Message Flow innerhalb eines Pools  
5) Zu viele Elemente in einem Diagramm

**23. Was gehört innerhalb eines Pools hin: Sequence Flow oder Message Flow?**

Sequence Flow. Message Flow innerhalb eines Pools ist ein Anfängerfehler.

**24. Was tust du gegen vergessene Bedingungen an Gateway-Pfeilen?**

Bedingungen an die ausgehenden Pfeile schreiben und einen Default Flow markieren.

**25. Welche Tools/Quellen nennt das Skript für BPMN?**

Wikipedia: BPMN und bpmn.io (Modellierungs-Tool).

**26. Selbstcheck 2.1: Wofür steht BPMN und warum ist eine gemeinsame Notation wertvoll?**

Business Process Model and Notation (BPMN 2.0, ISO/IEC 19510). Wertvoll, weil Fachabteilung, IT und Management dieselbe standardisierte Sprache lesen, wie Noten in der Musik; das vermeidet Missverständnisse.

**27. Selbstcheck 2.2: Was ist der Unterschied zwischen Sequence Flow und Message Flow?**

Sequence Flow verbindet Elemente innerhalb eines Pools (Ablaufreihenfolge). Message Flow verbindet verschiedene Pools (Nachrichtenaustausch zwischen Beteiligten).

**28. Selbstcheck 2.3: Nenne drei der fünf Anfängerfehler.**

Drei aus: kein Start-/End-Event; Gateways nicht geschlossen; Bedingungen an Pfeilen vergessen; Message Flow innerhalb eines Pools; zu viele Elemente in einem Diagramm.


## Kapitel 3 · BPMN fortgeschritten und KI-gestützt

**29. Was sind Sub-Prozesse, und mit welchem Bild erklärt das Skript sie?**

Hierarchische Zerlegung eines Prozesses, wie Zoom-Stufen in einer Karte.

**30. Unterschied eingebetteter Sub-Prozess vs. Call Activity?**

Eingebetteter Sub-Prozess: lebt im Elternprozess.  
Call Activity: wiederverwendbar (ruft einen eigenständigen Prozess auf).

**31. Welche Faustregel gilt für die Größe eines BPMN-Diagramms?**

Max. 15–20 Elemente pro Diagramm, sonst zerlegen.

**32. Wofür nutzt man Timer Events, und welches Symbol haben sie?**

Uhr-Symbol. Für zeitgesteuerte Starts, Wartezeiten und Deadlines.  
  
<i>Kurs-Flashcard: „Was ist ein Timer Event?“</i>

**33. Was ist ein Error Boundary Event (Symbol, Zweck, Verhalten)?**

Blitz am Rand einer Aktivität; dient der Fehlerbehandlung; ist immer unterbrechend (die Aktivität wird abgebrochen).

**34. Wie benennt man Activities nach Best Practice? Beispiel?**

Verb-Objekt, z. B. „Rechnung prüfen“.

**35. Wie benennt man Events nach Best Practice? Beispiel?**

Als Zustand, z. B. „Bestellung eingegangen“.

**36. In welcher Reihenfolge und mit welchem Layout modellierst du?**

Happy Path zuerst, Ausnahmen danach. Layout von links nach rechts, Ausnahmen nach unten.

**37. Wofür kann KI beim BPMN-Modellieren eingesetzt werden?**

Prozessbeschreibung in eine BPMN-Elementliste übersetzen; bestehende Modelle auf Fehler prüfen; Prozessvarianten (Ist, Soll, Automatisiert) generieren.

**38. Welche Arbeitsteilung gilt zwischen dir und der KI beim Modellieren?**

Die KI liefert den Entwurf, die fachliche Korrektheit prüfst du. (Und: erst selbst zeichnen, dann KI prüfen lassen.)

**39. Selbstcheck 3.1: Wann zerlegst du einen Prozess in Sub-Prozesse?**

Wenn ein Diagramm zu groß wird (Faustregel: mehr als 15–20 Elemente). Außerdem für Teile, die wiederverwendet werden (dann als Call Activity).  
  
<i>Kurs-Flashcard: „Wann nutzt du einen Sub-Prozess in BPMN?“</i>

**40. Selbstcheck 3.2: Wozu dient ein Error Boundary Event?**

Zur Fehlerbehandlung: Es sitzt (Blitz-Symbol) am Rand einer Aktivität, fängt dort auftretende Fehler ab, bricht die Aktivität immer ab und leitet in einen Ausnahmepfad.

**41. Selbstcheck 3.3: Wie benennst du Activities und Events korrekt?**

Activities als Verb-Objekt („Rechnung prüfen“), Events als Zustand („Bestellung eingegangen“).


## Kapitel 4 · Wertstromanalyse und Schwachstellen

**42. Woher stammt die Wertstromanalyse (VSM)?**

Aus dem Toyota-Produktionssystem (Lean).

**43. Was zeigt eine Wertstromanalyse, und worauf liegt der Fokus?**

Material- und Informationsfluss, mit Fokus auf die Zeit. Sie trennt wertschöpfende Zeit von Verschwendung.  
  
<i>Kurs-Flashcard: „Was ist Wertstromanalyse (VSM)?“</i>

**44. Wie ergänzen sich BPMN und VSM?**

BPMN zeigt die Logik, VSM zeigt, wo Zeit verloren geht.

**45. Welche drei Kriterien muss eine wertschöpfende Tätigkeit erfüllen?**

1) Sie verändert das Produkt  
2) Der Kunde würde dafür zahlen  
3) Sie wird beim ersten Mal richtig gemacht

**46. Nenne Beispiele für nicht wertschöpfende Tätigkeiten.**

Warten, Genehmigungsschleifen, Transport, Nacharbeit.

**47. Wie berechnet man den Wertschöpfungsanteil?**

Wertschöpfungsanteil = Wertschöpfungszeit / Gesamtdurchlaufzeit × 100 %

**48. Rechenbeispiel Schadensmeldung: 45 Min Bearbeitung bei 30 Arbeitstagen Durchlaufzeit. Wie hoch ist der Wertschöpfungsanteil?**

≈ 0,3 %.  
Rechnung (mit 8-h-Arbeitstag): 30 × 8 × 60 = 14.400 Min; 45 / 14.400 ≈ 0,31 %.  
Achtung: Mit Kalenderzeit (24 h) wären es nur ≈ 0,1 %. Die Zeitbasis immer angeben.

**49. Warum ist der Wertschöpfungsanteil in Verwaltungsprozessen oft viel niedriger als bei physischer Wertschöpfung?**

In reinen Verwaltungsprozessen besteht die Durchlaufzeit überwiegend aus Warten und Schleifen. Steckt physische Wertschöpfung im Strom (Backen, Ausliefern), liegt der Anteil deutlich höher. Merksatz: rechnen statt schätzen.

**50. Nenne die sieben Verschwendungsarten (Muda).**

1) Überproduktion  
2) Wartezeit  
3) Transport  
4) Überbearbeitung  
5) Bestände  
6) Unnötige Bewegung  
7) Fehler/Nacharbeit  
  
<i>Kurs-Flashcard: „Nenne drei der sieben Verschwendungsarten (Muda).“</i>

**51. Welche achte Verschwendungsart nennt die moderne Lean-Erweiterung (im Kurs optional)?**

Ungenutztes Mitarbeiter-Potenzial.

**52. Wofür stehen Kaizen-Blitze in der Wertstromkarte, und welche Verbesserungshebel nennt das Skript?**

Sie markieren Verbesserungspotenziale vom Ist zum Soll. Hebel: Zusammenlegen, Pull, Automatisieren, Parallelisieren.

**53. Auf welchen vier Ebenen bewertet die Schwachstellenmatrix?**

Zeit, Kosten, Qualität, Risiko.

**54. Aus welchen vier Teilen besteht das kompakte Dokumentationspaket?**

Prozesssteckbrief, BPMN-Modell, Wertstromkarte, Schwachstellenmatrix.

**55. [Eigener Selbstcheck] 4.1: Was unterscheidet die Wertstromanalyse von BPMN?**

BPMN bildet die Ablauflogik ab (wer macht was in welcher Reihenfolge, mit welchen Verzweigungen). VSM bildet Material- und Informationsfluss mit Fokus auf Zeit ab und macht sichtbar, wo Zeit verloren geht (wertschöpfend vs. Verschwendung).

**56. [Eigener Selbstcheck] 4.2: Wann ist eine Tätigkeit wertschöpfend? Prüfe: „Antrag zur Freigabe an die Abteilungsleitung weiterleiten“.**

Wertschöpfend = verändert das Produkt, Kunde würde zahlen, beim ersten Mal richtig.  
Weiterleiten zur Freigabe verändert das Produkt nicht und der Kunde würde dafür nicht zahlen: nicht wertschöpfend (Genehmigungsschleife/Transport von Information).

**57. [Eigener Selbstcheck] 4.3: Ein Prozess hat 2 h Bearbeitungszeit bei 10 Arbeitstagen (à 8 h) Durchlaufzeit. Wertschöpfungsanteil?**

2 h / (10 × 8 h) × 100 % = 2 / 80 × 100 % = 2,5 %.

**58. [Eigener Selbstcheck] 4.4: Nenne die sieben Verschwendungsarten und ordne zu: Ein Bericht wird ausführlicher erstellt als vom Empfänger benötigt.**

Überproduktion, Wartezeit, Transport, Überbearbeitung, Bestände, unnötige Bewegung, Fehler/Nacharbeit.  
Zuordnung: Überbearbeitung (mehr Aufwand/Qualität als gefordert). Wird der Bericht zusätzlich erstellt, obwohl ihn niemand braucht: Überproduktion.

**59. [Eigener Selbstcheck] 4.5: Wie kommst du vom Ist zum Soll, und was gehört ins Dokumentationspaket?**

Im Ist-Wertstrom Verbesserungspotenziale mit Kaizen-Blitzen markieren (Zusammenlegen, Pull, Automatisieren, Parallelisieren) und Schwachstellen in der Matrix nach Zeit, Kosten, Qualität, Risiko bewerten.  
Paket: Prozesssteckbrief, BPMN-Modell, Wertstromkarte, Schwachstellenmatrix.


## Quiz Modul 2 (10 Fragen)

**60. Quiz 1: Angebotsprozess der Schreinerei, SIPOC-Methode. Wer ist der primäre „Customer“ (C)?<br>A: Holzhändler, der das Material liefert<br>B: Potenzieller Kunde, der eine Anfrage stellt<br>C: Schreiner, der das Angebot kalkuliert<br>D: Architekt, der die Baupläne erstellt**

<b>B</b>. Customer = Empfänger des Prozessergebnisses (Output). Beim Angebotsprozess ist das der anfragende Kunde, der das fertige Angebot erhält.  
<i>Hinweis: SIPOC kommt im Begleitskript nicht vor, siehe Ergänzungskarte.</i>

**61. Quiz 2: Im Interview sagt Klaus Müller: „Dann wird das Angebot erstellt, das ist ja klar.“ Welche Reaktion entspricht der gelernten Fragetechnik?<br>A: Nicken und „Angebotserstellung“ notieren<br>B: „Erstellt das Angebot Ihr Meister oder die Bürokraft?“<br>C: „Wer genau erstellt das Angebot und welche Werkzeuge werden dafür genutzt?“<br>D: „Können wir den Schritt überspringen und zum Versand kommen?“**

<b>C</b>. Bei Selbstverständlichkeiten mit offenen W-Fragen nachhaken (Wer, Womit), um tatsächliche Schritte, Personen und Werkzeuge aufzudecken.  
B ist eine geschlossene Entweder-oder-Frage und gibt die Antwort schon vor.

**62. Quiz 3: Bestellprozess Bäckerei Wagner. Filiale, Zentrale und Backstube sind interne Abteilungen derselben Firma und sollen sichtbar sein. Wie stellst du sie in BPMN dar?<br>A: Drei Pools mit Message Flows<br>B: Drei Lanes in einem Pool „Bäckerei Wagner“<br>C: Drei aufeinanderfolgende User Tasks<br>D: Drei Sub-Prozesse auf oberster Ebene**

<b>B</b>. Interne Abteilungen als Lanes in einem Pool. Pools stehen für eigenständige Teilnehmer (typisch externe Organisationen). User Tasks und Sub-Prozesse sind Aktivitäten, keine Organisationseinheiten.  
<i>Kritik: „nur für externe Organisationen“ ist zu absolut, siehe Frage 4.</i>

**63. Quiz 4: Die Filiale (eigener Pool) sendet eine Bestellung an die Zentrale (zweiter Pool). Womit modellierst du den Informationsaustausch?<br>A: Sequence Flow, weil die Schritte nacheinander erfolgen<br>B: Message Flow zwischen den beiden Pools<br>C: Annotation<br>D: Gemeinsamer Sub-Prozess „Datenübertragung“**

<b>B</b>. Zwischen Pools nur Message Flow; Sequence Flow darf Pool-Grenzen nicht überschreiten.  
<i>Kritik: Frage 3 sagt, Filiale und Zentrale gehören als Lanes in einen Pool. Hier sind sie zwei Pools. Beides ist modellierbar, aber die Fragen widersprechen sich.</i>

**64. Quiz 5: Belegprozess Hoffmann. „Wenn nach 14 Tagen eine Original-Rechnung immer noch fehlt, soll automatisch eine Mahnung an den Mandanten gehen.“ Welches BPMN-Symbol?<br>A: Exklusives Gateway, das prüft, ob 14 Tage vergangen sind<br>B: Error Event, weil eine fehlende Rechnung ein Fehler ist<br>C: Timer Event, angehängt an den Task „Warten auf Rechnung“<br>D: Paralleles Gateway, das den Mahnprozess startet**

<b>C</b>. Ein Timer Event modelliert den zeitbasierten Ausnahmepfad nach Ablauf der Frist. Error Events sind für technische/fachliche Fehler, ein Gateway kann nicht „warten“.  
<i>Kritik: Ob unterbrechend oder nicht-unterbrechend, sagt die Lösung nicht. Soll nach der Mahnung weiter auf die Rechnung gewartet werden, ist ein nicht-unterbrechendes Timer-Boundary-Event (gestrichelt) richtig. Sauberer wäre ohnehin ein Event-basiertes Gateway (Rechnung eingegangen vs. 14 Tage vergangen) statt eines Tasks „Warten“.</i>

**65. Quiz 6: Schmidt-Logistik disponiert nach einer Frachtanfrage entweder Standard-LKW, Kühltransport oder Schwertransport, immer nur eine Option. Welches Gateway?<br>A: Parallel (AND)<br>B: Inklusiv (OR)<br>C: Exklusiv (XOR)<br>D: Event-basiert**

<b>C</b>. XOR: genau eine von mehreren Alternativen. Bedingungen an die Pfeile schreiben, Default Flow markieren.  
<i>Hinweis: Gateway-Typen stehen nicht im Begleitskript, siehe Ergänzungskarte.</i>

**66. Quiz 7: Wertstromanalyse Wagner. Bestellungen werden abends gesammelt und erst am nächsten Morgen bearbeitet. Welche Verschwendungsart primär?<br>A: Überproduktion<br>B: Unnötiger Transport<br>C: Warten<br>D: Fehler**

<b>C</b>. Der Vorgang liegt unbearbeitet, die Wertschöpfung steht still.  
<i>Anmerkung: Das Sammeln (Batching) erzeugt zugleich Bestände (liegende Bestellungen). „Primär“ macht C trotzdem zur besten Antwort.</i>

**67. Quiz 8: Welche zentrale Erkenntnis über Prozessaufnahme liefert der Hoffmann-Mailverlauf?<br>A: Prozesse sind meist perfekt dokumentiert und werden exakt befolgt<br>B: Der reale Ist-Prozess enthält oft unstrukturierte Schleifen und weicht von der Theorie ab<br>C: Interviews sind die einzig verlässliche Methode<br>D: Prozessaufnahme ist nur in Produktionsbetrieben sinnvoll**

<b>B</b>. Der Mailverlauf zeigt den tatsächlichen Ablauf voller Ausnahmen und Rückfragen, die in einer idealisierten Beschreibung fehlen (Prozess-Eisberg).

**68. Quiz 9: Wertstromkarte Wagner: Bearbeitungszeit 15 Minuten, Durchlaufzeit 8 Stunden. Was sagt das Verhältnis?<br>A: Geringer Wertschöpfungsanteil, hohe Liegezeiten<br>B: Die Mitarbeiter arbeiten sehr langsam<br>C: Fast 100 % wertschöpfend<br>D: Mit schnelleren Computern auf 15 Min reduzierbar**

<b>A</b>. 15 / 480 Min ≈ 3,1 %. Der große Rest ist Warten bzw. Liegen.  
<i>Kritik: Die Lösung setzt Bearbeitungszeit mit Wertschöpfung gleich. Nach der Skript-Definition ist auch Bearbeitungszeit nur teilweise wertschöpfend (z. B. Nacharbeit), der echte Anteil liegt also bei höchstens 3,1 %.</i>

**69. Quiz 10: Im Müller-Profil werden drei Workarounds erwähnt. Warum musst du sie als Digitalisierungsmanager verstehen?<br>A: Um Regelbrecher zu identifizieren<br>B: Weil Workarounds oft auf Schwachstellen oder fehlende Funktionen hinweisen<br>C: Um zu beweisen, dass die Doku fehlerhaft ist<br>D: Weil Workarounds immer ineffizient sind und sofort weg müssen**

<b>B</b>. Workarounds zeigen, wo der offizielle Prozess lückenhaft ist oder die Realität nicht abbildet. Sie sind ein Startpunkt für echte Verbesserungen.  
<i>Anmerkung: Die Antwort sagt „Soll-Prozess“. Gemeint ist der offizielle bzw. vorgegebene Prozess; ein Soll im Sinne der Optimierung gibt es da noch nicht.</i>


## Ergänzungen (nicht im Skript, aber im Quiz gefragt)

**70. [Ergänzung, nicht im Skript] Wofür steht SIPOC?**

Supplier, Input, Process, Output, Customer. Grobe Prozessübersicht auf einer Seite: wer liefert was, welche 5–7 Hauptschritte, was kommt heraus, wer empfängt es. Customer = Empfänger des Outputs.  
  
<i>Kurs-Flashcard: „Was ist eine SIPOC-Analyse?“</i>

**71. [Ergänzung, nicht im Skript] Welche vier Gateway-Typen braucht man in BPMN, und wann nutzt man welchen?**

XOR (exklusiv, „X“): genau ein Pfad.  
AND (parallel, „+“): alle Pfade gleichzeitig, kein Bedingungstext.  
OR (inklusiv, „O“): ein oder mehrere Pfade.  
Event-basiert: das zuerst eintretende Ereignis entscheidet (z. B. Nachricht kommt vs. Frist läuft ab).

**72. [Ergänzung, nicht im Skript] Unterbrechendes vs. nicht-unterbrechendes Boundary Event?**

Unterbrechend (durchgezogener Rand): Die Aktivität wird abgebrochen, der Prozess läuft nur im Ausnahmepfad weiter.  
Nicht-unterbrechend (gestrichelter Rand): Die Aktivität läuft weiter, zusätzlich startet ein paralleler Pfad (z. B. Erinnerung/Mahnung).  
Error Boundary Events sind immer unterbrechend, Timer- und Message-Boundary-Events gibt es in beiden Varianten.


## Kurs-Flashcards (neu, ohne Dubletten)

**73. [Kurs] Was ist der Unterschied zwischen Soll- und Ist-Prozess?**

Ist-Prozess: wie der Prozess heute tatsächlich abläuft, inkl. Workarounds, Ausnahmen, Medienbrüchen.  
Soll-Prozess: der angestrebte, verbesserte Zielprozess.  
Merksatz aus dem Skript: Ohne sauberes Ist kein gutes Soll.

**74. [Kurs] Was ist der Unterschied zwischen Pool und Lane in BPMN?**

Pool: ein eigenständiger Prozessbeteiligter (typisch eine Organisation). Zwischen Pools nur Message Flow.  
Lane: Unterteilung innerhalb eines Pools für Rollen oder Abteilungen. Zwischen Lanes läuft Sequence Flow.

**75. [Kurs] Was ist ein exklusives Gateway (XOR)?**

Eine Verzweigung, bei der genau einer von mehreren Pfaden genommen wird (Raute mit „X“ oder leer). Bedingungen an die ausgehenden Pfeile schreiben, Default Flow markieren. Beim Zusammenführen wartet es nicht, sondern lässt den ankommenden Pfad durch.

**76. [Kurs] Wofür steht bpmn.io?**

bpmn.io „steht“ für nichts, es ist kein Akronym. Es ist ein kostenloses, browserbasiertes Open-Source-Werkzeug (von Camunda) zum Zeichnen von BPMN-Diagrammen.  
<i>Die Frage ist schief gestellt; gemeint ist wohl „Was ist bpmn.io?“</i>

**77. [Kurs] Was ist ein Error Event?**

Ein Ereignis (Blitz-Symbol) für Fehlerbehandlung. Als End-Event wirft es einen Fehler; als Boundary Event am Rand einer Aktivität fängt es ihn ab, bricht die Aktivität immer ab und leitet in einen Ausnahmepfad.

**78. [Kurs] Was ist der Zweck eines Prozess-Steckbriefs?**

Eine einseitige Kurzbeschreibung eines Prozesses als Teil des Dokumentationspakets (mit BPMN-Modell, Wertstromkarte, Schwachstellenmatrix). Typischer Inhalt: Name, Ziel, Prozesseigner, Start und Ende, Input/Output, Kunden, Beteiligte, IT-Systeme, Kennzahlen.  
<i>Inhalt ist eine Ergänzung aus allgemeinem Wissen; das Skript nennt den Steckbrief nur. Mit eurer Kursvorlage abgleichen.</i>

**79. [Kurs] Beispiel: Workaround bei der Müller-Schreinerei.**

<i>Antwort aus Kursmaterial ergänzen (Müller-Profil, das mir nicht vorliegt).</i>  
Laut Quiz nennt das Profil drei Workarounds. Allgemein gilt: Ein Workaround ist ein inoffizieller Umweg, der eine Lücke im offiziellen Prozess oder System überbrückt, und damit ein Hinweis auf eine Schwachstelle.

**80. [Kurs] Was ist ein „Digital Gemba Walk“?**

<i>Antwort aus Kursmaterial ergänzen. Der Begriff steht nicht im Skript und ist kein feststehender Fachbegriff.</i>  
Naheliegende Lesart: Gemba-Prinzip (dort hinschauen, wo die Arbeit passiert) übertragen auf digitale Arbeit, also Mitarbeitenden am Bildschirm über die Schulter schauen, Klickwege, Systemwechsel und Medienbrüche beobachten.

**81. [Kurs] Was ist der Unterschied zwischen Durchlauf- und Bearbeitungszeit?**

Durchlaufzeit: gesamte Zeit vom Start bis zum Ende des Prozesses, inkl. Warte- und Liegezeiten.  
Bearbeitungszeit: Zeit, in der aktiv am Vorgang gearbeitet wird.  
Achtung: Bearbeitungszeit ist nicht automatisch Wertschöpfungszeit (z. B. Nacharbeit).

**82. [Kurs] Wozu dient eine Schwachstellenmatrix?**

Sie sammelt die gefundenen Schwachstellen eines Prozesses und bewertet sie auf vier Ebenen: Zeit, Kosten, Qualität, Risiko. So lassen sich Verbesserungen priorisieren. Teil des Dokumentationspakets.

**83. [Kurs] Beispiel: Prozessbeteiligte bei Wagner-Filialen.**

<i>Antwort aus Kursmaterial ergänzen.</i>  
Aus dem Quiz bekannt: Filiale, Zentrale und Backstube (interne Abteilungen, in BPMN als Lanes in einem Pool „Bäckerei Wagner“). Weitere Beteiligte (z. B. Kunden, Lieferanten, Fahrer) stehen vermutlich im Fallmaterial.

**84. [Kurs] Was ist der Zweck eines Cross-Reviews von BPMN-Modellen?**

<i>Genaue Kursdefinition aus Kursmaterial ergänzen.</i>  
Allgemein: Andere prüfen dein Modell (und du ihres) auf Notationsfehler (z. B. die fünf Anfängerfehler), fachliche Korrektheit und Verständlichkeit. Wer den Prozess nicht kennt, merkt am schnellsten, was unklar ist.


## Kritische Anmerkungen zum Skript

Das Skript ist insgesamt solide, aber an einigen Stellen verkürzt oder unpräzise. Für Prüfungen lohnt es sich, das zu wissen:

1. **„Jeder Split braucht einen Join“ ist eine Modellierungskonvention, keine BPMN-Regel.** Die Spezifikation erlaubt offene Gateways. Als Stilregel (strukturierte Modelle, weniger Fehler bei parallelen Pfaden) ist sie sinnvoll, als „Fehler“ ist sie überzogen.
2. **Gateway-Typen fehlen komplett.** Das Skript nennt Gateways nur als „Verzweigungen“, erklärt aber nicht XOR (exklusiv), AND (parallel) und OR (inklusiv). Ohne diese Unterscheidung kann man den Anfängerfehler „Bedingungen an Pfeilen vergessen“ gar nicht richtig verstehen: Bedingungen braucht man an XOR/OR-Gateways, nicht an AND. Das solltest du dir zusätzlich ansehen.
3. **„Activities (Aufgaben)“ ist verkürzt.** Activity ist der Oberbegriff; Task (Aufgabe) und Sub-Prozess sind Unterarten. Kapitel 3 nutzt Sub-Prozesse dann ja auch als Activities.
4. **Timer Events:** korrekt, aber unvollständig. Anders als Error Boundary Events können Timer Boundary Events auch nicht-unterbrechend sein (gestrichelter Rand). Die Aussage „Error Boundary Events sind immer unterbrechend“ stimmt.
5. **„Max. 15–20 Elemente“** ist eine Kurs-Faustregel, keine Norm. In der Literatur gibt es andere Werte (z. B. die Modellierungsrichtlinien „7PMG“ nach Mendling: Modelle mit über 50 Elementen zerlegen). Als Lernwert die Kurszahl nehmen, aber nicht als Standard verkaufen.
6. **Rechenbeispiel 0,3 % ohne Zeitbasis.** 45 Min / 30 Arbeitstage ergibt nur dann ≈ 0,3 %, wenn man 8-h-Arbeitstage ansetzt (14.400 Min). Mit Kalenderzeit wären es ≈ 0,1 %. Gerade weil das Skript „rechne statt schätzen“ fordert, hätte die Annahme dastehen müssen.
7. **„Kaizen-Blitz“ ist doppeldeutig.** Im Skript ist das Symbol in der Wertstromkarte gemeint (engl. *kaizen burst*). Der Begriff wird aber auch für einen kurzen, intensiven Verbesserungsworkshop verwendet (*Kaizen Blitz*). Nicht verwechseln.
8. **VSM-Herkunft verkürzt.** Die Methode stammt aus Toyotas „Material- und Informationsflussdiagrammen“; bekannt gemacht als Value Stream Mapping wurde sie durch Rother/Shook („Learning to See“, 1998). Für die Kursprüfung reicht „Toyota/Lean“.
9. **„Schwachstellenmatrix“ und „Prozesssteckbrief“** sind keine genormten Begriffe, sondern Kurs-/Praxiswerkzeuge. Die vier Ebenen (Zeit, Kosten, Qualität, Risiko) sind die Kursdefinition.
10. **Gemba:** Wörtlich heißt Gemba „der tatsächliche Ort“. „Geh dorthin, wo die Arbeit passiert“ beschreibt eher den Gemba Walk bzw. das Prinzip Genchi Genbutsu. Inhaltlich passt es, sprachlich ist es vermischt.
11. **Kapitel 1, Beobachtung:** Das Skript nennt für Gemba nur eine Stärke, keine Schwäche, obwohl Selbstcheck 1.2 genau das abfragt. Typische Schwächen: zeitaufwändig, Momentaufnahme (seltene Ausnahmen sieht man nicht), und Beobachtete arbeiten unter Beobachtung oft anders (Hawthorne-Effekt). Das ist in der Musterantwort als Ergänzung gekennzeichnet.
12. **Kapitel 4 endet ohne Selbstcheck.** Die fünf Karten „[Eigener Selbstcheck]“ habe ich ergänzt; sie bleiben inhaltlich beim Skript, nur 4.2–4.4 sind Anwendungsaufgaben mit eigenen Beispielen.


## Kritische Anmerkungen zum Quiz

Das Quiz ist brauchbar, die Lösungen sind im Kern richtig. Einige Punkte sind aber unsauber:

1. **Fragen 3 und 4 widersprechen sich.** Frage 3 lehrt: Filiale und Zentrale sind interne Abteilungen, also Lanes in einem Pool, Pools „nur für externe Organisationen“. Frage 4 modelliert genau diese beiden als zwei Pools. Fachlich ist beides möglich: Man nimmt getrennte Pools, wenn interne Einheiten eigenständige Prozesse mit eigener Steuerung haben. Das „nur“ in Frage 3 ist deshalb zu absolut. Für die Kursprüfung gilt vermutlich: intern gleich Lanes.
2. **Frage 5 ist unvollständig erklärt.** Die Anforderung klingt so, als solle man nach der Mahnung weiter auf die Rechnung warten. Dann braucht es ein **nicht-unterbrechendes** Timer-Boundary-Event, was die Lösung nicht sagt. Außerdem ist ein Task „Warten auf Rechnung“ schlechter Stil, weil Warten keine Arbeit ist. Sauberer wäre ein Event-basiertes Gateway oder ein Message-Zwischenereignis mit Timer. C bleibt trotzdem die beste der vier Antworten.
3. **Das Quiz fragt Stoff ab, der nicht im Begleitskript steht:** SIPOC (Frage 1), die Gateway-Typen XOR/AND/OR/Event-basiert (Frage 6) und der Begriff Bearbeitungszeit (Frage 9). Dafür habe ich drei Karten mit **[Ergänzung]** angelegt.
4. **Frage 9 setzt Bearbeitungszeit mit Wertschöpfung gleich.** Das widerspricht der Definition aus Kapitel 4 (wertschöpfend heißt auch „beim ersten Mal richtig“). 3,1 % ist die Obergrenze, nicht der Wertschöpfungsanteil.
5. **Frage 7:** Das abendliche Sammeln ist Warten, erzeugt aber auch Bestände. „Primär“ rettet die Frage, eindeutig ist sie nicht.
6. **Kleinigkeiten:** Frage 2, Antwort C ist eine Doppelfrage (eigentlich ein Interview-Fehler, besser einzeln fragen). Frage 10 spricht vom „Soll-Prozess“, gemeint ist der offizielle Prozess. Fragen 8 und 10 beziehen sich auf Kursmaterial (Mailverlauf, Müller-Profil), das ich nicht kenne; die Karten funktionieren trotzdem ohne.

## Anmerkungen zu den 20 Kurs-Flashcards

- 8 der 20 Kursfragen decken sich mit vorhandenen Karten. Dort habe ich keine Dublette angelegt, sondern die bestehende Karte mit dem Tag **Kurs-Flashcard** markiert (in dieser Datei steht der Kurs-Wortlaut darunter).
- 12 Kursfragen sind neu dazugekommen (Präfix **[Kurs]**).
- **„Wofür steht bpmn.io?“ ist schief gestellt.** bpmn.io ist kein Akronym, sondern ein Werkzeug. Gemeint ist wohl „Was ist bpmn.io?“.
- **Vier Karten setzen Kursmaterial voraus, das mir fehlt** (Müller-Workaround, Wagner-Beteiligte, Digital Gemba Walk, Cross-Review). Sie tragen den Tag **Kursmaterial_fehlt** und den Hinweis „Antwort aus Kursmaterial ergänzen“. Was dort steht, ist eine allgemeine Einordnung und kein Kurswissen. Bitte ersetzen, sobald du das Material hast.
- „Digital Gemba Walk“ ist kein etablierter Fachbegriff, sondern offenbar eine Kurs-Prägung. Im Skript kommt er nicht vor.
- Prozess-Steckbrief, SIPOC, Pool/Lane-Unterschied, XOR und Durchlauf-/Bearbeitungszeit werden in den Kurs-Flashcards abgefragt, im Begleitskript aber kaum oder gar nicht erklärt. Das Skript allein reicht für Quiz und Flashcards also nicht.
