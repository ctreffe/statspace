---
editor_options: 
  markdown: 
    wrap: 72
---

# Methodenskript zum Testen von Nullhypothesen

-   Beschreibung des Normalfalls: Wir postulieren einen Effekt und
    möchten diesen anhand erhobener Daten zeigen. Effekte zeigen sich
    dann oftmals als Unterschiede in der AV zwischen verschiedenen
    Gruppen. Dabei ist unser wissenschaftliches Arbeiten darauf
    ausgelegt, dass wir nur dann sagen, dass wir den vermuteten Effekt
    gefunden haben, wenn wir uns sehr sicher sind, dass beobachtete
    Unterschiede in der AV nicht ein Zufallsergebnis sind. Dies nennen
    wir eine konservative Herangehensweise und veranschaulicht wird
    diese immer durch ein festgelegtes Alphafehler-Niveau von 0.05. Der
    Alphafehler ist dabei ein Maß für die Wahrscheinlichkeit, dass der
    beobachtete (oder ein noch stärkerer) Effekt nur ein Zufallsergebnis
    darstellt (dass wir das Datenmuster bei Daten erhalten würden, in
    denen es definitiv keinen Effekt gibt sondern nur die normale
    Fehlervarianz)

-   Da diese Beschreibung ziemlich abstrakt ist, sollten wir das an
    einem konkreten Beispiel aus der Praxis erläutern, dass auch die
    Wichtigkeit des Alphafehlers bzw. der konservativen Herangehensweise
    verdeutlicht. Am besten eignet sich vielleicht eine
    Wirksamkeitshypothese für eine Therapie oder ein Medikament. Wir
    könnten das auch auf Corona münzen, aber eigentlich finde ich das
    nicht so gut. Entscheidend ist, dass wir klar machen, dass
    Medikamente (Homöopathie?) nur dann zugelassen werden und eingesetzt
    werden sollten, wenn wir uns sicher sind, dass sie wirken. Ein
    unwirksames Medikament zu verabreichen ist ein Worst Case bei
    medizinischen Behandlungen. Der Grund dafür ist, dass ein nicht
    wirksames Medikament auch ohne direkte negative Effekte die Lage von
    Patient:innen verschlechtert, weil zugunsten des unwirksamen
    Medikamentes vielleicht auf eine Behandlung mit anderen, wirksamen
    Medikamenten verzichtet wird. Daher gibt es hohe Hürden für die
    Medikamentenzulassung

-   Zusammen passen beide vorherigen Punkte, weil im Kern die Vermeidung
    eines Alphafehlers zurecht priorisiert wird. Nun lassen sich aber
    auch Fragestellungen und Probleme finden, in denen umgekehrt der
    Worst Case wäre, dass man keinen Effekt annimmt, obwohl einer da
    ist, dass man also einen Effekt übersieht. Ein Beispiel aus der
    Praxis kann die Erforschung von Umweltgiften und ihrer Schädlichkeit
    für den menschlichen Organismus oder die Tier- und Pflanzenwelt sein
    (Klimawandel?). Hier will man schädigende Effekte definitiv nicht
    übersehen

-   Nun dreht sich in unserer Testlogik um, was eine konservative
    Herangehensweise ist. Wir wollen nicht mehr länger den Alphafehler
    minimieren, sondern den Betafehler. Wir wollen uns nun also sehr
    sicher sein, dass wir einen eventuellen Effekt nicht übersehen, wenn
    er da ist. Erst wenn wir dies mit einer konservativen
    Herangehensweise gezeigt haben, sollten wir auch an der Aussage
    festhalten, dass es einen Effekt nicht gibt.

-   Dass diese umgekehrte Testlogik normalerweise nicht zum Einsatz
    kommt sehen wir an dem Sprichwort "Absence of Evidence is not
    Evidence of Absence". Wir minimieren normalerweise den Alphafehler
    und behandeln den Betafehler eher zweitrangig (seit die Testpower
    mehr in den Fokus rückt trifft diese Aussage nicht ganz zu, aber das
    hat eher etwas mit Replizierbarkeit zu tun als mit der Vermeidung
    eines Betafehlers. *Johannes fragen:* Darf man das so sagen? Stehen
    hinter überlegungen zur Power und zur minimierung des Betafehlers
    wirklich unterschiedliche Ansätze?)

-   Im Skript könnten wir vielleicht bei der Fragestellung zum
    Umweltgift auch mal mit konkreten Rechenbeispielen arbeiten und
    konkret zeigen, welche Konsequenz es haben kann, wenn man eigentlich
    die Nullhypothese kritisch testen will, dann aber alles so belässt
    wie bei einer kritischen Prüfung der Gegenhypothese. Das passiert
    oft in Forschungsartikeln und ich frage Thomas mal nach einem
    klassischen Beispiel aus Gruppenlernen oder Gruppenleistung, da habe
    ich das als Student gehört und gelernt

-   Wenn wir eine Fragestellung untersuchen, bei der es wichtiger ist,
    die Nullhypothese kritisch zu hinterfragen als die Gegenhypothese
    (wenn wir umgangssprachlich also zeigen wollen, dass es keinen
    Effekt gibt), dann müssen wir also unsere Testlogik so anpassen,
    dass am Ende der abgewandelte Satz "Absence of Evidence is Evidence
    of Absence" gilt.

-   Das gelingt uns erstmal ohne sonstige Veränderungen an unserer
    Erhebung, wenn wir einfach das kritische Alphaniveau anheben, z.B.
    von 0.05 auf 0.2. Alpha- und Betafehler verhalten sich so
    zueinander, dass wenn alles andere gleich ist (Stichprobengröße und
    Effektstärke), der Betafehler sinkt, wenn man einen höheren
    Alphafehler zulässt. Das sollte konzeptuell völlig klar sein, denn
    wenn man eher den Fehler zulässt einen eigentlich nicht vorhandenen
    Effekt anzunehmen, dann muss das die Wahrscheinlichkeit reduzieren,
    dass man einen eigentlich vorhandenen Effekt nicht annimmt

-   Eine andere Maßnahme zur Verringerung des Betafehlers ist die
    Erhöhung des Stichprobenumfangs. Hier sollte vielleicht nochmal
    daran erinnert werden, dass die Testpower als 1-Beta definiert ist.
    Wenn wir also eine Powerstarke Studie durchführen, dann ist die
    Wahrscheinlichkeit einen Effekt zu übersehen entsprechend gering.
    Wir reden sonst über Power wie gesagt eher beim Thema
    Replizierbarkeit. Dort ist die Idee, dass unsere Ergebnisse leichter
    replizierbar sind wenn wir Powerstarke Studien durchführen. Da muss
    man natürlich um die Ecke denken, dass Underpowered Studies in
    Kombination mit einem Filedrawer-Bias ein Problem für die
    Replizierbarkeit darstellen. Kurz illustriert: Wenn ich 5 Studien
    mit je 30 Versuchspersonen durchführe und davon wird eine
    signifikant, kann ich die 4 anderen in der Schublade verschwinden
    lassen. Das geht nicht, wenn ich nur eine Studie mit 150 Personen
    durchführe. Die kann ich zwar auch im Filedrawer verschwinden
    lassen, aber zumindest setze ich dann keine falschen Behauptungen in
    die Welt (hier bietet sich natürlich ein Link zum berüchtigten
    XKCD-Jellybeans Comic an). Dieser ganze Punkt führt vielleicht zu
    weit weg von dem eigentlichen Thema, dann lassen wir ihn raus. *Ich
    sehe aber schon, wie dieses Skript und das Skript zur Effektstärke
    einen klaren Anknüpfungspunkt zum Thema Testpower und
    Replizierbarkeit bieten...*

-   In diesem Skript gibt es klare Implikationen für die
    wissenschaftliche und für die praktische Perspektive. Bei der
    wissenschaftlichen Perspektive halten wir fest, dass man unabhängig
    von statistischen Verfahren und deren Ergebnissen immer auch die
    Testlogik mitdenken muss, um die (selteneren aber durchaus
    auftretenden) Situationen zu erkennen, in denen man nicht die
    Gegenhypothese sondern die Nullhypothese kritisch testen möchte. In
    diesen Situationen sollten die Rahmenbedingungen der Testung
    (Testpower, Stichprobenumfang, ggf. adjustiertes Alhpafehlerniveau)
    auch einen kritischen Test ermöglichen. Diesen Punkt kann man sicher
    auch mit simulierten Daten zu den oben vorgeschlagenen
    Praxisbeispielen illustrieren (wenn das das Skript nicht zu lang
    macht)

-   Für die Praktikerperspektive bleibt zu sagen, dass wir erkennen
    müssen, dass Interventionsentscheidungen nicht immer zwingend auf
    einem kritischen Test eines Effekts basieren müssen, sondern auch
    auf einem kritischen Test eines Nulleffekts basieren können (siehe
    das Beispiel zu Umweltgiften und dann z.B. potenziellen
    Einsatzverboten und Regulierungen, siehe Debatten um Düngemittel
    oder Schädlingsbekämpfungsmittel). Auch für Praktiker:innen ist es
    also bei der Beurteilung der wissenschaftlichen Evidenz ganz
    entscheidend, dass sie erkennen können, wann eine Intervention auf
    Basis der Aussage "Absence of Evidence is Evidence of Absence"
    abgeleitet werden kann

-   Für mündliche Prüfungen gilt es diese Unterschied sicher zu erkennen
    und entsprechend bei regulären kritischen Tests der Gegenhypothese
    dem Motto "Absence of Evidence is not Evidence of Absence" zu folgen
    und genau zu erkennen, wann "Absence of Evidence is Evidence of
    Absence" gilt oder sagen zu können, durch welche Mittel man diese
    Aussage in einer Studie gültig machen kann. Dafür hätte ich hier
    gerne wieder, wie beim Kausalitätsskript, einen eigenen Kasten, weil
    die Frage immer vorkommt und weil die Studierenden sie einfach zu
    oft in der Prüfung versemmeln

-   Andere Generelle Frage: Gibt es sowas wie einen Zentralen Kern von
    Skripten, den wir klar abgrenzen können und der die Grundlage für
    das Verständnis aller wissenschaftlicher Studien darstellt? Hier
    meine Themenvorschläge:

    -   Effektstärke und Signifikanz
    -   Testpower und Replizierbarkeit
    -   Testlogik für Nullhypothesen und Gegenhypothesen (Alpha- und
        Betafehler) bzw. NHST
    -   Kausalität
    -   Konfundierung
    -   Multiple Analysen und Befundmuster

    Also: Quasi alles was wir dieses Semester gemacht haben plus ein
    zusätzliches Thema. Sollten wir das als Skript dann auch noch ins
    Auge fassen? Für mich wären das dann die "Kernkompetenzen" bzw.
    "Kernthemen". Dafür sollten wir eine passende snappy
    Kategorienbezeichnung finden. Ich finde was mit Kern oder Core
    ziemlich gut (Core Concepts? Kernkonzepte?), weil das auch in diese
    Analogie vom Themennetz passt und diese Themen gehören definitiv ins
    Zentrum (zentrale Konzepte? Kritische Konzepte?)
