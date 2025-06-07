---
tags:
  - Agents
  - AI
  - Technologie
  - EnBW
  - IBM
  - Meeting
---

# Video
[Learning-Session_ IBM about agentic AI-20250506_153335-Besprechungsaufzeichnung.mp4](https://myenbw.sharepoint.com/:v:/r/sites/digitaloffice/Shared%20Documents/Webinare,%20Events%20und%20Veranstaltungen/Learning-Session_%20IBM%20about%20agentic%20AI-20250506_153335-Besprechungsaufzeichnung.mp4?csf=1&web=1&e=FMcmet&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)

# Copilot Zusammenfassung:

- **Einführung in Agentic AI:** Björn Schmitz und seine Kollegen von IBM Consulting geben einen Überblick über Agentic AI und deren Anwendungsmöglichkeiten. Sie erklären, wie Agenten in verschiedenen Bereichen eingesetzt werden können, um komplexe Aufgaben zu lösen und die Arbeit zu verbessern. 1:51
    
- **Anwendungsfälle von Agentic AI:** Björn Schmitz und Daniel Ehmann präsentieren drei Anwendungsfälle von Agentic AI: Produktentwicklung, Energiesektor und Kundenservice. Sie zeigen, wie Agenten in diesen Bereichen eingesetzt werden können, um Prozesse zu optimieren und Herausforderungen zu bewältigen. 2:41
    
- **Technische Umsetzung von Agentic AI:** Daniel Ehmann erklärt die technische Umsetzung von Agentic AI und zeigt Best Practices auf. Er erläutert, wie Agenten miteinander kommunizieren und Werkzeuge einsetzen, um Aufgaben zu lösen. 7:18
    
- **Regulatory Reporting:** Daniel Ehmann stellt eine Anwendung von Agentic AI im Bereich Regulatory Reporting vor. Er zeigt, wie Agenten dabei helfen können, regulatorische Berichte effizienter zu erstellen und die Kosten zu reduzieren. 14:48
    
- **Skalierbarkeit von Agentic AI:** Daniel Ehmann erklärt, wie die Agentic AI Lösung skaliert werden kann, um verschiedene Module und Berichte zu erstellen. Er zeigt, wie die Lösung auf ehemalige Berichte trainiert werden kann, um die Effizienz zu steigern. 25:00
    
- **Antragsdokumente im Energiesektor:** Adrian Wellhausen präsentiert einen Use Case für Agentic AI im Energiesektor. Er zeigt, wie Agenten bei der Erstellung von Antragsdokumenten helfen können, indem sie relevante Informationen suchen, Texte generieren und die Qualität der Dokumente prüfen. 34:44
    
- **Kundenservice:** Daniel Ehmann stellt eine Agentic AI Lösung für den Kundenservice vor. Er zeigt, wie Agenten in einem Chatbot eingesetzt werden können, um Kundenanfragen effizient zu beantworten und die Kundenzufriedenheit zu steigern. 50:13
    
- **Technische Implementierung:** Fernanda fragt nach der technischen Implementierung von Agentic AI. Daniel Ehmann erklärt, dass verschiedene Technologien und Modelle verwendet werden, darunter Python und Open Source Modelle. 58:22

# Transkript

0:07  
Doch wieder. Und jetzt seht ihr mich ja wieder und hört mich wieder. Wie kommt es zu diesem Setup, dass dass wir so heute hier sitzen? Wir sind mit ein paar Leuten aus dem DO sind wir im, Ich glaube im März war es früher ne sind wir zum zum Jenny I Roundtable von IBM waren wir eingeladen weil wir uns auch mal anschauen wollten hey was passiert denn eigentlich beim Thema Agents schon schon wirklich ne also bis dahin ich gebe es zu ich habe viel gelesen man sieht irgendwelche youtube Videos man weiß aber nicht was passiert wirklich schon mit Agenten und bei der Konferenz.

  
0:36  
Haben wir dann gesehen, dass IBM zusammen mit Kunden schon tatsächlich Agenten umgesetzt hat und weil wir das dort gesehen haben, haben wir gedacht, Hey, das könnte auch einfach spannend für die en BW sein. Wir fragen einfach mal die Kollegen, also von daher schon mal vielen, vielen Dank für dass ihr, dass ihr da die Bereitschaft habt, ob sie einfach das wissen, was wir bei anderen Unternehmen schon gemacht haben, ob sie die Erfahrung einfach mit uns teilen würden, damit wir auch herausfinden, was sind eigentlich die Herausforderungen in der Praxis, wenn man, wenn man Agenten einsetzt, ich glaube, wie stehen da jetzt gerade am Anfang die ersten POC.

  
1:06  
Sind geplant und von daher freuen wir uns heute, dass ihr hier seid, dass ihr eure Erfahrung mit uns teilt. Vielen, vielen Dank dafür und ich freue mich auf die Inhalte, die ihr mitgebracht habt. Vielen Dank breit und genau Björn, ja vielen Dank, die Bühne gehört euch genau. Dann erstmal herzlichen Dank für die Einladung, machen wir natürlich sehr gerne.

  
1:30  
Mein Name ist Björn Schmitz, Ich bin Social Partner hier bei IBM Consulting, verantworte da die Themen Data und AI und ich habe noch 2 Kollegen mitgebracht, die sich jetzt gleich auch vorstellen. Der Daniel und der Adrian, beides technische Experten bei uns, die kennen sowohl die Anwendungsseite natürlich sehr gut, kennen aber auch, wenn es dort in die Richtung Fragen gibt, die technischen Hintergründe, die Fallstricke, die Erfahrung aus vergangenen Projekten.

  
1:59  
Also von unserer Seite aus können wir das sehr, sehr gerne interaktiv gestalten. Wenn Fragen sind, gern den Chat nutzen oder auch direkt reinfragen, weil es ist ja eine Learning Session eman ne, so habe ich es verstanden und genauso möchten wir es eigentlich auch aufsetzen genau, ich würde 2 Sätze vielleicht zur Einleitung sagen.

  
2:23  
Wir haben heute ganz kurzen Überblick noch mal zu agentic AI für diejenigen, die den ersten Learning Talk nicht gehört haben, aber ich hatte verstanden von Franziska, dass es dazu auch schon eine Session gab. Das heißt, wir halten uns nicht lange mit den Definitionen, aufgehen dann in 3 Anwendungsfälle rein, das ist einer der aus der Produktentwicklung kommt, den wird der Dani vorstellen, wird da auch ein bisschen drauf eingehen.

  
2:49  
Wie wir technisch das Thema Agentic AI umsetzen, was dort Best practices sind, wie das gut funktioniert, wie man es gut skalieren kann, zeigen dann einen Case, der eher sag ich mal aus dem Energiesektor kommt, wo es um Zulassung und Profilprozesse geht und schauen dann noch mal, weil es natürlich auch sehr relevant ist in das Thema Kunde rein. Wie kann ich solche Technologien im Kundenservice einsetzen und in kundennahen Funktionen?

  
3:19  
Wo man sich ja eigentlich immer so ein bisschen ja zurückhält, weil man sagt, Oh, da kann viel schiefgehen, aber auch da ist natürlich sehr viel Potenzial drin. Am Ende machen wir ganz kurz ein Webup wie kann man starten, wie kann man auch niederschwellig gucken, welche Use Cases geeignet sind für gentic AI und gerne wie gesagt eine Diskussion draus machen und dann schauen wir, in welche Richtung uns das heute trägt, genau.

  
3:47  
Vielleicht als Einleitung noch mal ganz kurz gentic AI ist ein ist ein klasses Stichwort, aber worum es natürlich eigentlich geht, ist unsere Arbeit und wie wir mit AI unsere Arbeit auch verbessern können, wie wir uns Unterstützung holen können. Und ich bin jetzt 10 Jahre in dem Feld, ich muss sagen ich mach das super gerne, aber AI war immer auch ein Nischenthema und das war deshalb ein Nischenthema, weil wir als Menschen natürlich sehr gut sind.

  
4:17  
Zu planen. Wir können eine Bilanz lesen, wir verstehen sofort, was auf einer Tabelle ist. Wir können im Kundensupport und im Vertrieb im Team arbeiten, sehr empathisch mit Leuten sprechen können, unterschiedliche Probleme reflektieren, Werkzeuge einsetzen, um die zu lösen. Und das alles sind natürlich Themen gewesen, die uns als Menschen ausmachen und die zeigen, warum wir komplexe Tätigkeiten eben gut lösen können.

  
4:44  
Und ich glaube, das ist eigentlich der Anspruch, den agentic AI zumindest nach allen Regeln der Kunst und nach allen Zeitungsartikeln und so weiter auch teilweise zumindest erfüllen soll. Das heißt, wenn wir von agentischen Designs sprechen, dann geht es eigentlich darum, dass ein Team von Agenten, also nicht nur ein einzelnes GPT Modell, sondern eben ein Team unterschiedlicher AI Agents.

  
5:13  
Werkzeuge einsetzen kann zum Beispiel eine Abfrage einer Datenbank machen kann oder einen Eintrag in eine SAP Kapelle schreiben kann und durch diese Werkzeuge eben Aufgaben löst, die wir täglich auch alle lösen müssen, nämlich ein Ziel verfolgen und ein Bericht schreiben, eine Analyse machen, eine Zusammenfassung von Financial Reports machen, das heißt?

  
5:42  
Was durch JAI in diese Welt der Agenten reinkommt, ist dynamisches planen, die Nutzung von Werkzeugen, die Möglichkeit, aus Fehlern zu lernen, also auch wirklich zu reflektieren, ist das, was ich dort geschrieben hab, ist das, was ich dort zusammengefasst hab, ist das richtig, ja oder nein und das Ganze passiert eben nicht sequenziell, sondern quasi in einem Team von einzelnen Agenten.

  
6:11  
Und wie das genau passiert, um es auch ein bisschen Anfassbarer zu machen, das wird uns der Daniel zeigen. Anhand von einem konkreten Case in der Produktentwicklung. Dani, damit würd ich an dich übergeben. OK, vielen Dank.

  
6:31  
Lass mich kurz sehr gut, also vielleicht kurz noch 23 Worte zu mir, weil wir uns noch nicht kennen. Ich bin Daniel Ehmann, Global Tech Lead für Agent KI Applikation über unser IBM Consulting Business weltweit hinweg und ich darf mich seit rund 10 Jahren mit künstlicher Intelligenz befassen, habe meinen Phg und Postdoc in Apply Machine Learning absolviert und Computer Science.

  
6:59  
In Oxford studiert und ich darf euch heute durch mich agentica i Applikationen führen. Ich teile ganz gerne meinen Screen und setze da fort wo der Björn aufgehört hat, so könnt ihr das sehen sehr gut. OK vielen Dank.

  
7:25  
Um noch mal genau da anzusetzen, wo Björn gerade aufgehört hat, also das letzte Jahr hat sehr stark, wie die linke Seite hier ausgeschaut, wo es ne Single Agent The I Interaction war. Ihr hattet ne Frage an Chat GPT und Chat, GPT kam zurück mit einer Antwort wo wir jetzt hingehen ist wie Björn gerade gesagt hat sind Multi Agenten Systeme wo wir mehrere Agenten haben die autonom miteinander zusammenarbeiten können.

  
7:51  
Um komplexere Aufgaben und Problemstellungen zu lösen. Das heißt, wir geben unsere Aufgabe oder stellen unsere Frage an ein ganzes Team von EA Agenten, die dann für uns die Frage oder die das Problem lösen und jeder von diesen Agenten ist sehr spezialisiert, der kann in Tools greifen, wie Bian gesagt hat, wir können autonom das Internet durchforsten, wir können in strukturierte Datenbanken greifen.

  
8:19  
Wir sprechen also im wahrsten Sinne des Wortes von Machine to machine communication. Diese Agenten sprechen miteinander in Englisch und können so sich so koordinieren und komplexere Aufgaben und Problemstellungen zu lösen. Und jeder von diesen Kreisen ist ein Language Model und es können entweder proprietäre Language Models sein, von Open AI und Tropic oder Google oder eben Open Source Language Models von IBM von Missrall.

  
8:49  
Oder netto, in die wir hier greifen können. Aber ich glaub das setzt so the Stage for worver Moving to Words und was ganz wichtig ist, ist, dass wir wirklich von mit dem Move von Links zu recht von von Single to Multi Agent AI Applikationen, dass wir von China Assistance with Chappots hingehen zu Aktionen, die mit Agents und Agenten ausgeführt werden können, gut.

  
9:18  
Daniel, Ich habe eine Frage, aber wenn wir uns die linke Seite anschauen, also wenn wir nur mit einem AI Agenten zu tun haben, es ist momentan nicht so, dass dieses Setup heute etabliert ist, weil mit AI Agent, was wir auch darunter verstehen, dieses Thema Zielverfolgung und das autonome Handeln und die Entscheidungsfähigkeit.

  
9:45  
Oder habt wie wie sieht ihr das? Ist die linke Seite aus eurer Sicht etabliert, sieht ihr das heutzutage Unternehmen ein Single Agents mehr oder weniger einfach umgesetzt haben?

  
10:02  
Absolut also die linke Seite ist so, wo wir herkommen und die rechte Seite zeigt, wo die Reise hingeht, wo die Industrie und die AI Community @lorage hingehen, dass wir also hingehen zu einer Welt, wo wir sehr viel Spezialisierung sehen werden über die einzelnen Agenten hinweg, weil mit diesem einzelnen Agenten hier auf der linken Seite kommen wir willkommen.

  
10:26  
Ein bisschen ein Stück weit, aber nicht wirklich weit. Und deswegen sehen wir auf Spezialisierungen in Wirtschaften und genau das Gleiche passiert jetzt gerade mit mit EI Agenten, dass wir versuchen in eine ganze, in ganze Teams von hochspezialisierten EI Agenten zu greifen und dass wir.

  
10:45  
As we had an app for anything around dos were gong to have an agent for anything that we need und deswegen ganze Teams von AI Agenten greifen können, die wissen, wie sie miteinander zusammenarbeiten, um komplexere Aufgaben miteinander zu lösen, ja.

  
11:04  
Und da geht die Reise hin und IBM war dabei und hat solche Lösungen bereits in in Produktion getragen und unsere Kunden genießen jetzt die, die die Vorteile davon Mhm Dankeschön, die Wissenschaft und die.

  
11:21  
Empirische Evidenz, die wir sehen, ist auch sehr klar, dass wir von der rechten Seite wahnsinnige Performance approvement sehen. Und das liegt an 3 verschiedenen Gründen. Einmal, weil wir, weil jeder Agent spezialisiert ist, zweitens, weil wir ein Problem sehr viel holistischer betrachten und angehen, können wir davor eben aus einer technischen Business in einer ethischen Perspektive und drittens, weil sich diese Agenten selber kreuz checken können, sodass.

  
11:50  
Der auch gut vom einen Agent durch den anderen Agenten überprüft wird. Und all diese, all diese Faktoren in Kombination führen dazu, dass wir sehr viel bessere Resultate und Task Compinition Rates erreichen können, dann von und, und das ist sozusagen von der tiefen Perspektive, es gibt noch 2 weitere Dimensionen von Breite und Höhe, wenn ich das mir von der breiten Perspektive anschaue, dann ist es heute möglich viel.

  
12:18  
Breitere Prozessketten zu automatisieren. End to End und das liegt daran, weil Language Models so große Fähigkeiten haben, sie sind multimodal, wir können autonom das Internet durchsuchen, wir können mit den strukturierten Datenbanken sprechen, das ist alles möglich.

  
12:36  
Und wir, wir, wir können in in enterprise.it Systeme greifen und mit den Daten kommunizieren und arbeiten und schließlich von einer höheren Perspektive können wir governance und und Monitoring haben, wo wir diese Systeme auch wirklich steuern können, wo wir Enterprise grade, Filters und God Rails implementieren können, sodass die Agenten nicht einfach beispielsweise Discount.

  
13:01  
Ausgeben on we half of the Company was sie nicht machen sollen, aber das nur ganz kurz. Also die Reise geht auf die rechte Seite, aber viele Unternehmen sind noch auf der linken Seite und ich möchte euch gerne ein Beispiel sagen, wo wir das sehr erfolgreich etabliert haben.

  
13:21  
IBM hat auch selber eine ganze Plattform, wo wir motoragentensysteme bauen und die eine platt Applikation die ich euch zeigen werde ist ist eine spezifische Applikation die auf dieser Plattform lebt.

  
13:35  
Und die Plattform hat 3 verschiedene horizontale Layers, eine für deren Products and Lay House. Dann haben wir in der Mitte hier die Multi Agenten Systeme und wie wir die Orchestrieren und dann zum Schluss und top haben wir das Frontend und user Interface for AI und genau und dann vertikal haben wir Applikationen die sich durch alle die 3 Layers greifen und die eine die ich euch vorstellen werde ist ist regulate.

  
14:03  
Weil da geht es um Regulatory Reporting und die Frage ist, wieso ist das ein wahnsinnig vielversprechender V und Use Case für Agent to KI und und cherit to KI more generally der Grund ist, dass Regulation sehr textintensiv ist und es ist genau der Ort, wo Large Language Models sehr stark sind. Regulationen sind üblicherweise auch sehr.

  
14:31  
Administrativally Costly und deswegen ein Bereich, wo unsere Kunden viel Geld und Ressourcen sparen können und dann zu guter Letzt ist sind Regulationen hier um zu bestehen und und die Führen tatsächlich dazu, dass dass wir sehen, dass die Regulierungen eher steigen über die Zeit, wie sinken.

  
14:56  
Und wir waren dabei und haben solche Lösungen bereits in Produktion getragen. Fully agentic AI Designs, wo das Regulator Reporting an ein an mich Agenten outgesourct haben und ich werde euch gleich zeigen wie wir das gemacht haben.

  
15:11  
Folgendes um jetzt hier aber noch vorab euer Interesse zu wecken für Regulatory Reporting und wieso so ein interessanter Use Cases für Gentic AI möchte ich euch gerne den Business Impact zeigen, den wir hier sehen und hier auf der linken Seite seht ihr den Animal Time and Cospirden, den unsere Kunden haben, wenn die solche Regulatory Reports schreiben, stellt euch vor, ihr habt 50 regulatory authors die über

  
15:39  
3 Monate lang an einem Gewissen, an einem bestimmten Regulatory Report arbeiten. Was wir sehen in der Industrie ist, dass diese Kosten um 95% bis zu 95% reduziert werden können. Somewaring the range of seventyp to ninety five Prozent with a eye und.

  
15:58  
In diesem Fall haben keine Firing Rounds stattgefunden. Die Company als Ganzes war aber viel produktiver, weil die Leute, die waren wurden einfach realocated und konnten dann ihre Arbeit in einem anderen Department fortsetzen.

  
16:16  
Aber es konnte wirklich reduziert werden, massiv. Wir haben statt statt 3 Monate arbeiten nicht 50 Leute, sondern nur noch ne Handvoll Leute, ungefähr 5 Leute an dem gleichen Regulatory Report und sie produzieren den nicht innerhalb von 3 Monaten, sondern in wenigen Tagen oder Wochen, also die die die Cost and Efficiency Games sind massiv und dann das.

  
16:40  
Gleiche sind wir hier auch für diesen Use Case bezüglich den Ertragssteigerungen, weil wir unseren Kunden geholfen haben, rund 100 Tage schneller am Markt zu sein. Und wenn ich als Unternehmen mein Produkt 100 Tage früher am Markt verkaufen kann und pro Tag über den europäischen Markt hinweg mein Produkt für 1000000 oder 5000000 verkaufen kann, dann sprechen wir schnell von dreistelligen Millionenbeträgen, die wir dazu gewinnen.

  
17:10  
An an additional revenues gut, das ist die Business Seite, weshalb das so interessant ist und weshalb sich sich sich die AI Investments hier um ein Zigfaches ausgezahlt haben. Schon nach dem ersten Product Release um wir das danach für mehrere Produkte nutzen können.

  
17:29  
So, jetzt regulatory Reporting. Wie sieht das aus? Wir haben möglicherweise mehrere Module, die wir es einreichen müssen, und das heißt, unsere Kunden setzen auf 10 tausenden Seiten von Text, von Powerpoints und Excel Sheets, die sie irgendwie in eine Form Gießen würden müssen, die der Regulator von Ihnen verlangt und der Regulator verlangt eine gewisse.

  
17:51  
Struktur, verschiedene Sections, Subsections und so weiter und wir schauen uns an in dem konkreten Falle, wie wir hier beispielsweise hier einen von diesen Moduls und spezifische Sub sections hier generieren können. Mit unserer Applikation und High Level. Wie das funktioniert, ist es so, dass wir die ganzen Inputs konsumieren, dann eine sehr supestizierte Retriever Augmented Generation Pipeline haben und das dann an einem Multi Agenten System geben, wo die Agenten alle.

  
18:21  
Zugang haben zur Regulierung und dann entsprechend für die entsprechende Section ein Outbook generieren. Und das wird hier die Lösung, wird hier angesteuert, mehrheitlich durch die Azure und What's Next Infrastruktur Unbenutzen mehrere Lorge Language Models, die autonom miteinander zusammenarbeiten von Open AI Metamystro und hogging Face und damit möchte ich auch gerne gleich in die eigentliche Demo eintauchen.

  
18:49  
Und das ist hier eine fulifunktionale Applikation, die ihr seht, die auf der Plattform lebt, die ich vorhin gerade vorgestellt habe. Und wir haben hier die verschiedenen Sections, die wir gerne generieren würden, und ich zeige euch jetzt, wie wir das machen können. Ich habe das alles schon vorgeladen, damit wir nicht warten müssen, bis die bis die Outpodes generiert werden, und zwar möchte ich jetzt hier als author regulatory author möchte ich hier eine bestimmte Section.

  
19:19  
Von diesem Report generieren, was ich jetzt als allererstes mache, ist, ich kann die Input Daten hier hochladen und und dann dem Lorge Language Model sagen welche Inputs konsumiert werden sollen. Das sind üblicherweise Dokumente UPS, die so die sehr sehr lange sind, die so ausschauen, ja haben sehr viel Text, die haben Bilder, Tabellen und so weiter ja.

  
19:49  
Das ist hier, ah, jetzt kommt's ja, ah sorry, kannst du ein bisschen, OK, jetzt kommt ich kann auch schauen, OK also.

  
20:04  
Und der Regulator? Der sagt mir tatsächlich sehr konkret hier, das sind die Regulatory Guidelines, wo der Regulator sagt was er gerne hätte und wie die Section genau ausschauen soll. Das heißt hier wird angegeben schreibt der Regulator was ich über was ich in der entsprechenden Section bitte schreiben soll, das ist jetzt hier ein Beispiel in einem Pharmakontext, der lässt sich aber genauso gut übertragen auf jede andere Industrie und dann würde ich das.

  
20:34  
Dann geben wir oder oder Grounden die Large Language Models in diese Regulierung und geben den Agenten Zugang dazu. Und was dann passiert ist.

  
20:45  
Wenn ich das modeagenten System starte, dann seht ihr hier tatsächlich, wie die einzelnen Agenten miteinander interagieren und das heißt, es geht zuerst habe ich eine Input Message, dann geht's zu einem Chatmanager und jetzt kommt's zu einem Writing Agent, der zuerst ein sehr guten und soliden initialen Drawft von dieser Section quasi produziert und dann habe ich 2 Prüfagenten, die einerseits prüfen für Vollständigkeit.

  
21:13  
Spricht dieser blaue Writing Agent über alles, was der Regulator von uns will und zweitens habe ich einen Source Revue Agent, der nicht für Vollständigkeit prüft, sondern für Korrektheit und was der blaue Writing Agent hier produziert hat, das heißt dieser Agent schaut zurück auf die Inputs und schaut, ob der blaue Agent das korrekt zusammengefasst hat oder nicht und wenn nicht, dann gibt dieser Agent hier. Dieser Prüfagent gibt Feedback und sagt dem blauen Agenten, Hey, du musst es umschreiben.

  
21:43  
Du hast ihren Fehler gemacht, Korrigier das bitte und so Iterieren die in in multiple Loops, bis entweder die beiden Agenten wie hier zufrieden sind mit dem Output oder bis wir eine maximal Anzahl an an Iterationen erfüllt haben und geben dann entsprechend final den entsprechenden Output zurück. Ja dann.

  
22:12  
Und bekomme das hier nach wenigen Minuten zurück, wenn ich das hier als Mensch alles hätte schreiben müssen, hätte es mich mindestens einen ganzen Tag gekostet, weil ich hätte diese 80 bis 100 Dokumenten lange Input Dokuments hätte ich zuerst studieren müssen, hätte mir dann nachlesen müssen, was der Regulator genau von mir möchte und hätte mich dann an die Arbeit machen müssen, die ganze Subsection hier abzufassen und und einzutippen und das Ganze zusammen.

  
22:42  
Zusammenzufassen. Während hier Agenten mit einem super soliden Drawed zurückkommen, an uns nach 2 bis 3 Minuten, und das ist ein Game Changer für viele von unseren Kunden.

  
22:58  
Wir haben dieses System fundamental mit einem Human in The Loop designt. Das heißt, hier hat er menschliche Regulatory Author, hat Zugang, die entsprechende Section gleich zu editieren. Wir können auch zurückgehen und sagen, wir möchten gerne zusätzliche Dokumente hochladen oder unsere einzelnen Agenten adaptieren, ein anderes Modell aussuchen für den Agenten und können das alles anpassen plus.

  
23:28  
Ist ich kann entsprechende Tabellen hinzufügen, die ich gerne dabei hätte. Hier kann ich die Dazufügen und und hochladen und einfügen in den Text, die wurden aus den Input Dokumenten erkannt und so weiter also es ist fundamental Engineered with the human in the loop.

  
23:52  
Dass wir das Review können, aber dass der Mensch sehr, sehr viel schneller ist, um um genau das zu tun, weil die Menschen, die wissen genau was, was, was die Inputs waren, um die, die hier einfließen und und können das dann entsprechend korrigieren. Gut jetzt.

  
24:09  
Ultimativ möchte ich als Unternehmen aber den Wert von dieser Möglichkeiten. Die Channel Bcfi bietet @Scale abschöpfen. Das heißt, ich möchte mindestens über 3 verschiedene Achsen die Lösung skalieren. Ich möchte nicht nur diese 34 sections hier generieren können, sondern wenn ich noch mal zurück gehe, hier hingehe, dann möchte ich gerne.

  
24:37  
Da möchte ich gerne alles actions von diesem bestimmten Modul generieren können. Ich möchte gerne über alle verschiedene Module hinweg Content generieren können, plus ich möchte gerne die Lösung skalieren können zu regulatory Reporting Beyond just sustain Scientific Reporting, aber eben auch Financial Reporting, All Reporting, Sustainability, Reporting und so weiter Adrian wird euch nachher noch einen anderen Use Case erläutern, wo wir genau das was.

  
25:07  
Vorhaben hier jetzt um diese dieser Skalierung hier Rechnung zu tragen, haben wir das System hier mit diesem Skalierung Gedanken implementiert und was wir fundamental gemacht haben ist, wir erlauben das System auf ehemaligen Submission Reports zu trainieren. Das heißt ich kann.

  
25:33  
Ehemalige Annual Report zum Beispiel, Inputs und Outputs, Reinfüttern und die Maschine lernt danach autonom, wie sie sich prompt muss, damit wir Outputs generieren, die nahe kommen an unsere ehemaligen Submission Reports for Annual Reporting oder eben andere Submission Reports.

  
25:54  
Und das ist hier, wo die wo die Item Lösung so sehr unsere Kunden überzeugt, weil das erlaubt denen das ganze Regulatory Authoring mit einer Lösung hier zu beantworten, wie mit 20 verschiedenen highly specialized.

  
26:09  
Venders zusammenzuarbeiten, um diesen Regulatory Reports zu zu generieren. Und wenn wir hier eintauchen, kann ich euch kurz zeigen, wie das geht. Das heißt, ihr könnt hier verschiedene Input Output pairs hochladen, wie solche wie wie solche Regulatory Reports wie die Aussehen, ihr habt hier die Inputs und hier habt ihr entsprechenden Section specific output wo die Maschine danach lernt wie wir diesen Output.

  
26:36  
Generieren können, basieren auf diesen Inputs und, und das ist der Trainingsmechanismus, den wir hier implementiert haben, um hier das vielleicht kurz zu fassen und und zu abstrahieren, was wir gemacht haben, zum Beispiel um euch einen Proofpoint zu geben für die Skalierbarkeit von so einer Lösung, ist folgendes, Wir haben hier einen neuen Use Case, nicht was ich euch davor gezeigt habe für Clinical Study Reports, sondern hier ist.

  
27:05  
Generieren wir die Highlights of the Prescribing Informations noch mal ein Pharma Use Case, aber es soll nur die Skalierbarkeit zeigen von von unserer Lösung und was wir hier gemacht haben ist, wir haben hier die die agentic AI Engine auf 3 verschiedenen Produkten trainiert. Ja wie wir also Inputs in Outputs.

  
27:27  
Komprimieren, was die Struktur ist und so weiter was der Regulator gerne möchte und haben dieses Training in die Agentica I Engine destilliert um dann zu testen wie gut das jetzt auf einem neuenprodukt.de funktioniert, das wir nicht verwendet haben um zu testen. Und wenn wir das machen haben wir grundsätzlich 2 Fragen. Also erstens möchten wir das Vergleichen mit einem hell out Human Output den wir schon.

  
27:55  
Genutzt haben oder haben aber nicht genutzt haben um zu trainieren und haben hier wirklich 2 Fragen. Einerseits möchten wir wissen, welchen Anteil von dem Human Output kann der AI Output abdecken, also was ist die Coverage von dem Human Output und zum zweiten Fragen wir uns wie factually Accurate der AI Output Server tatsächlich ist. Und noch mal wir wir haben hier die Challenge.

  
28:23  
Und nur Small Data Sets. Ja, wir haben nur 3 Beispiele und möchten die Agent AI Engine gerne so trainieren, dass das funktioniert und zum zweiten haben wir das jetzt hier für dieses Beispiel nur in in 23 Tagen gemacht, wo wir die Rekalibrierung und Datenaufbereitung und so weiter angefertigt haben um genau das zu tun, dass wir eine neue Zusammenfassung quasi schreiben können von diesen für dieses Produkt d.

  
28:51  
Ja, und die Resultate sind wie folgt erstens für die erste Frage bezüglich Coverage schafft es unsere AI Engine 90% vom Human Oput abzudecken, das heißt die AI Engine kommt zurück mit dem Oput der 90% vom Content im Human Oput abdeckt und das heißt nicht, dass die AI das in 10% der Fälle falsch gemacht hat, sondern das heißt nur, dass die AI sich entschieden hat, 10% des Contents im Human Oput.

  
29:21  
Anders zusammenzufassen, wie der Mensch, und das ist sehr ähnlich, wie wenn wir die quasi diese Aufgabe an 2 Menschen erteilt hätten, dann würden wir auch nicht erwarten, dass die beiden Menschen mit einem 100% Overlapping Report zurückkommen würden, sondern wir würden leichte Unterschiede zwischen diesen beiden Reports von den beiden Menschen erwarten. Es ist genau die gleiche Story hier mit AI und dann zum zweiten, wenn wir um um uns um Factual aqueracy kümmern, dann.

  
29:51  
Dann schafft es die AI Engine hier Content zu produzieren. Der 95% akkurat ist und ihr seht hier das Color Coding mit Grün. War das korrekt und hier die orangenen Stellen wo es nicht ganz korrekt war und das ist, weshalb wir immer noch ein Human in der Loop haben möchten in all unseren agentic Workflows.

  
30:14  
Und das ist wirklich auch, wo die, wo die, wo, die die Welt in AI im Moment steht, wer fundamentaly eine Co Pilot Mode Not in ein Auto Pilot Mode und das ist sehr vergleichbar zu Self Driving Cars, die funktionieren gut wenn wir hier in in in Kalifornien auf auf Highways fahren, aber es wird schwierig wenn wir in Deutschland oder in der Schweiz über Passstraßen fahren müssen mit einem mit einem Fully Autopilot funktioniert noch nicht und das ist

  
30:44  
auch dort, wo die Welt in der AI steht und damit möchte ich hier schließen und übergeben an Archian für den nächsten Use Case. Vielen dank Daniel, Es wurden im Chat einige Fragen gestellt und 2 Fragen wurden mehrfach gestellt.

  
31:00  
Vielleicht könntest du bezogen zu dem Case noch mal was sagen zum Thema Evaluation. Wie sorgt ihr dafür, dass das Thema Halluzination nicht vorkommt oder minimiert wird und die zweite Frage, die auch häufig vorkam, wie ihr für den jeweiligen News Case, die die passenden GPT Modelle auswählt, anhand einer bestimmten Logik oder einfach ja durchtesten?

  
31:24  
OK, beantworte gerne kurz die beiden Fragen, erstens bezüglich der Reduzierung von Halluzinationen. Was wir sehen ist, dass agentic AI uns enorm helfen kann damit und es gibt mehrere Ansätze, die wir verfolgt haben, einer von den Hauptansätzen ist der, dass wir in das Fact Checking greifen, von von verschiedenen Agenten, das heißt?

  
31:48  
Der eine Agent, der prüft tatsächlich gegenüber den Inputs, die wir eingegeben haben, ob das jetzt factually Consistant ist mit den Inputs, die wir konsumiert haben, oder ob der Salalam, die da Fakten halluziniert hat oder nicht. Und das hilft tatsächlich, und das empirische Evidenz auch sehr klar, dass uns das hilft.

  
32:09  
Halluzinationen zu reduzieren. Noch mal, es hilft zu reduzieren, aber wir können die Halluzinationen noch nicht zu 100% vollkommen eliminieren und deswegen haben wir immer noch ein human in The Loop.

  
32:24  
Und dann zur zweiten Frage, welche Modelle wir verwenden, um die entsprechenden Use Cases zu entwickeln. Wir orientieren uns da an die gängigen Leaderboards, wo wir sehen, welche Modelle für welche Aufgabe bestmöglich geeignet sind und wir arbeiten auch sehr häufig zusammen mit mit unseren Kunden, wo wir sehen in was für Modelle wir überhaupt greifen können. Ist das überhaupt eine Wahl, dass wir in das Bestmögliche ein Tropic Model greifen, ja oder Nein, wenn nicht, nehmen wir das Nächstbeste möglich.

  
32:54  
Modell, das auf dem Leaderboard erscheint und dann auch, dass wir gerade mit der starken Open Source Community mit unseren Kunden zusammenarbeiten, um die Modelle auf ihren eigenen Datenverein zu tun. Vielen Dank gut, ich lass es da verstehen, weil während Arian seine Zeit auflegt, noch noch eine Frage Dani, die du vielleicht beantworten kannst. Also A schreiben die GPTS ihre Prompts selbst.

  
33:20  
Und ist es wirklich ein Training im Sinne von einem Feintuning oder ist es eher fusured Learning, was hier verwendet wird? Das waren noch so 2 Sachen die die aufkommen, hier greifen wir in Technologien, wo wir das prompt Engineering von den LMS tatsächlich automatisiert haben und wir lernen anhand von den Input Output Pairs, wie wir gute Outputs generieren können, die sehr nah an die Training und Reference exemples herankommen.

  
33:55  
Wunderbar dann Adrian. Ja, vielen Dank, danke Daniel auch tolle Präsentation 23 Sätze noch zu mir ich bin Adrian Wellhausen, bin Data Scientist bei der IBM seit inzwischen fast 4 Jahren wo ich sage die meiste Zeit davon konnte ich inzwischen schon fast mit generative A auch verbringen und zuletzt oder nicht nur zuletzt aber bereits seit einiger Zeit auch schon mit tatsächlich eher Agents.

  
34:24  
Und da auf der technischen Ebene beim Implementieren, aber auch vom Solutioning und bei Use Case Creation. Und ich freue mich einen Use Case einmal mitgebracht haben zu haben, den ich einmal vorstellen möchte und der hoffentlich ganz besonders relevant ist für ihre Industrie, könnte ich ein kurzes Zeichen haben, ob wir meinen Bildschirm sehen können. Ja, super.

  
34:51  
Okay also in meinem Beispiel soll es konkret darum gehen, die Agenten im Energiesektor einzusetzen und da konkret bei der Erstellung von Antragsdokumenten, wenn sie gerne bestimmen, also wir müssen eine neue Leitung bauen, vielleicht ein neues Kraftwerk, einen neuen Windpark errichten und im Zuge dessen ist es auch nötig, einfach umfangreiche Genehmigungsverfahren zu durchlaufen oder Planfeststellungsverfahren und im Zuge dessen.

  
35:20  
Müssen wir als allererstes mal einen relativ umfangreichen Antrag schreiben, wo einfach sehr, sehr viele verschiedene Dokumente zusammenkommen, die dann bei der Behörde eingereicht werden müssen und zu erstellen solcher Anträge, das bindet in der Regel ziemlich viele Ressourcen und dauert auch relativ lange und genau hier können KI Agenten helfen und darauf möchte ich heute eingehen.

  
35:43  
Genau, ich habe hier einmal eine kleine Liste mitgebracht mit typischen Herausforderungen, die tendenziell damit verbunden sind, mit so mit Erstellung von Antragsdokumenten, die ist natürlich nicht vollzählig, aber vielleicht kommt die ein oder andere Herausforderung ihnen auch bekannt vor. Auf der rechten Seite habe ich mal ein Beispiel von ihnen auch mitgebracht, genau um solche Dokumente kann es sich zum Beispiel handeln, ja, so mit einem Erläuterungsbericht beispielsweise als Teil eines Planfeststellungsantrags und.

  
36:11  
Und bei der Erstellung sind sie natürlich mit verschiedenen Herausforderungen konfrontiert. Typischerweise gibt es relativ viele komplexe regulatorische Anforderungen sowohl auf Bundesebene Länder oder Kommunenebene, die sie berücksichtigen müssen, da müssen sie identifizieren, welche sind eigentlich für sie relevant, welches ist vielleicht die aktuelle Fassung davon und wird diese oder ist alles, was sie schreiben damit auch konform.

  
36:40  
Sind sie in Verbindung mit vielen Stakeholdern, zum Beispiel auch Gutachtern, die verschiedenen Dokumente vielleicht auch für sie mit produzieren, die sie mitberücksichtigen, die sie zu koordinieren haben, aber wo sie auch die Dokumente hinterher koordinieren müssen und wo auf der einen Seite natürlich die Frage ist, wie geht man mit so einer großen Summe an Dokumenten und dem Umfang von vielleicht besonders großen Dokumenten um, aber auf der anderen Seite auch, wo werden die eigentlich abgespeichert, wie zugänglich sind die und wie können diese gefunden werden?

  
37:10  
Und wenn wir vielleicht noch mal Richtung tatsächliche Erstellung von beispielsweise einem Erläuterungsbericht gucken. Anforderungen und Herausforderungen, die man hier haben kann, ist zum Beispiel, dass man über mehrere Kapitel hinweg auch innerhalb eines Kapitels, aber auch über Kapitel hinweg durchs ganze Dokument Konsistenz hat, also Konsistenz in der Sprache, in der Struktur.

  
37:31  
Da sollten keine Widersprüche drin stehen und hinterher möchte ich natürlich ein ein Dokument, was ich abgeben kann bei der entsprechenden Behörde, was natürlich richtig ist und was dann hinterher auch angenommen wird und in Summe natürlich, um es noch mal einmal hier abzurunden. All das ist natürlich mit extrem manuellem Aufwand verbunden und mit langen Erstellzeiten.

  
38:01  
Genau also wie können KI Agenten dabei helfen? Ich habe mal verschiedene Bereiche skizziert hier, bei denen KI Agenten tatsächlich helfen können, teilweise haben wir das auch schon jetzt gehört in Daniels Präsentation, also wir können automatisch helfen, zum Beispiel mit einem Brack System relevante Dokumente zu finden, aber nicht nur die Dokumente wie jetzt ein Umweltgutachten oder Lagepläne, sondern auch die tatsächlichen Informationen selbst wenn das sehr sehr lange.

  
38:29  
Dokumente sind, wo die Information drin steht, auf der auf der linken Seite unten Analyse und Qualitätsprüfung der Inputs, Dokumente. Wir haben wirklich eine Vielzahl von Input Dokumenten in diesem Zusammenhang, die eine Rolle spielt und wichtig für uns ist natürlich auch zu wissen, insbesondere wenn sie vielleicht nicht von uns persönlich stammen, sondern vielleicht auch von einem Dienstleister sind ja ich vollständig und.

  
38:53  
Und gibt es Widersprüche in den Dokumenten, gibt es vielleicht unterschiedliche Versionen und welche muss ich eigentlich verwenden und auf der anderen Seite natürlich, ich hatte es vorhin schon kurz angesprochen, wir haben gesetzliche Normen, wir haben technische Normen, die berücksichtigt werden müssen, auch da muss ich natürlich darauf achten, habe ich das die neueste Version zur Verfügung.

  
39:17  
Auf der rechten Seite Richtung Generierung. Vieles davon wurde vorhin auch bereits angesprochen. Ja, also natürlich, wir können automatisch Text erstellen und generieren basierend auf unseren Input Dokumenten, die ich eben genannt habe, aber auch vielleicht haben Sie Textbausteine, die sie wiederverwenden, ja oder eben entsprechende technische Normen und Gesetze und wir können auf diese natürlich auch referenzieren, auch das ist in diesen Dokumenten normalerweise wichtig.

  
39:45  
Und lassen Sie mir noch 2 Sachen hier nennen. Das eine ist zum Beispiel, diese Entscheidung darüber tatsächlich auch. Was muss tatsächlich generiert werden, also welche Kapitel sind tatsächlich notwendig? Ich mach mal ein Beispiel, wenn ich zum Beispiel eine.

  
40:02  
Einen erneuerungsbau hab oder eine eine, eine Verstärkung nur und nicht ein kompletten Neubau ist es vielleicht nicht nötig, noch mal eine komplette Umweltprüfung vorzunehmen und in dem Fall müssen Agenten auch feststellen können, OK, also Stichwort Negativfeststellung dieses Kapitel ist in dem Fall nicht oder in anderer Form zu generieren und unten rechts, das möchte ich jetzt auch noch mal angesprochen haben, Prüfung des generierten Textes ganz wichtig also.

  
40:32  
Die Normen gesetzliche Technische sind die eingehalten. Dann hatte ich noch mal gesagt Konsistenzprüfung fachlich, stilistisch auch sprachlich und werden zum Beispiel auch Begriffe einheitlich verwendet, ja, also Terminologie wie kann sowas konkret aussehen? Ich gebe mal ein konkretes Beispiel, das ist ein simplifiziertes Beispiel, aber das wird so in der Praxis auch bereits angewendet.

  
40:59  
So ein typischer Agenten Workflow kann wie folgt aussehen. Also hier haben wir ein Team auf 6 Agenten und diese Agenten kommen natürlich mit unterschiedlichen Fähigkeiten zusammen. Haben Sie das Ziel ein Kapitel in diesem Erläuterungsbericht zu erstellen und dieses Kapitel, also hier geht es in den Naturschutz und in diesen diese 6 Agenten bestehen aus dem Orchestrierungsagent der Agent kümmert sich quasi darum zu sagen okay wer ist denn dieser Sprecher?

  
41:29  
Und ja, koordiniert quasi die Konversation zwischen den Agenten. Wir haben den Suchagent, der tatsächlich die Dokumente und Informationen für uns sucht und findet, wir haben den Generierungsagent, der tatsächlich Text produziert, und dann haben wir 2 Prüfungsagenten, den Gesetzesprüfungsagenten und den Widerspruch prüfungsagenten und zuletzt noch einen Agenten, der für uns auch ein Output Format generiert, in dem Fall jetzt in Word, wenn wir das einmal.

  
41:57  
Wir uns angucken, wie das quasi in einem Flow aussieht, dann hätten wir hier auf der linken Seite einen Trigger, ob das jetzt ein User ist, der zum Beispiel sagt, Erstelle den Kapitel des Naturschutz, oder OB das von einem Tool automatisiert gesteuert wird, wenn zum Beispiel alle Kapitel auf einmal generiert werden müssen, ist natürlich flexibel, aber es gibt quasi einen Anstoß und von dort aus wird dann die Konversation geleitet von den Orchestrierungsagenten.

  
42:24  
Und wir sehen hier also als erstes würde der Suchagent hingehen, würde die relevanten Dokumente finden, die wir brauchen, sobald er die gefunden hat, würde er die gefundenen Dokumente weitergeben und der Generierungsagent macht sich an die Arbeit auf Basis dieser gefundenen und relevanten Dokumente für das Naturschutzkapitel und dieser generierte Text wird dann an den nächsten Agenten weitergegeben, in dem Fall hier der Widerspruchsagent.

  
42:50  
Der noch mal prüft und das referenziert noch mal, auf was Daniel eben gesagt hatte. Diese, auch diese Factual Correctness, bestehen Widersprüche zwischen dem generierten Text und wir sehen es hier unten an der gestrichelten Linie noch mal zu den tatsächlichen Daten inputdaten und wenn, wenn quasi hier eine Diskrepanz besteht, würde man dieses Feedback zurückgeben und den Generierungsagenten sagen, bitte mach dich noch mal in die Arbeit.

  
43:16  
Alternativ wird es weitergegeben. Der Gesetzesprüfungsorgan hat jetzt Zugriff auf die aktuellen Gesetze und kann sich diese ziehen und zuletzt wird das Wort generiert. Ich habe mal so eine.

  
43:31  
Zum beispielhaften Flow mitgebracht. Ich würde hier einmal versuchen, schnell durchzugehen, in der Zeit also wie gesagt, zunächst wird die Suche oder wird das die Generierung angestoßen, das heißt, der Orchestrierungsagent sagt Bitte das Kapitel Naturschutz für den Erläuterungsbericht, in dem Fall zum Windpark in Stuttgart erstellen, Wir hätten ein suchagent, er findet 2 Dokumente, faunagutachten und Biotopkartierung und.

  
43:59  
Danach macht sich der Generierungsagent an die Arbeit und er sagt jetzt im im Umfeld des Windparks wurden keine artenschutzrechtlich relevanten Arten festgestellt. Laut Gutachten sind keine geschützten Biotope betroffen, Ausgleichsmaßnahmen sind nicht erforderlich, das geht weiter an den Widerspruchsagent und dieser stellt jetzt aber tatsächlich fest, hier ist ein Widerstand im Faunagutachten sind Fledermaus vollkommen dokumentiert, im Text aber nicht. Also wir haben hier eine aktuelle Differenz.

  
44:27  
Und in dem Fall würde jetzt der Orchestrierungsagent quasi nicht entscheiden. Ich gebe es weiter an den nächsten Agenten, sondern noch mal zurück an den Generierungsagent es ist eine Nachbesserung nötig, das Fledermaus vorkommen muss quasi adressiert werden und das wird dann quasi umgeschrieben mit auf Basis dieses Feedbacks noch mal mit den Input Dokumenten und im nächsten Fall korrigiert würde hier stehen.

  
44:50  
Im Umfeld des Windparks wurden Fledermaus vollkommen festgestellt. Ein Abschaltkonzept für aktivitätsreiche Nächte wird umgesetzt und so weiter also wie gesagt ein simplifiziertes Beispiel, aber so könnte es aussehen und am nächsten Zuge würde dann quasi der Widerspruchsprüfungsagent grünes Licht geben, würde sagen kein Widerspruch gefunden, alle Aussagen stimmen mit dem bereitgestellten Gutachten überein.

  
45:13  
In dem Fall würde der Orchestrierungsagent sagen, alles in Ordnung. Nächster Sprecher muss nicht mehr zurückgeführt werden, sondern der nächste in der Reihenfolge ist dran. Es ist der Gesetzesprüfungsagent, der macht sich an die Arbeit, sagt in dem Fall auch, dass alles konform ist gemäß dem Bundesnaturschutzgesetz, auch hier alles in Ordnung von der Bewertung her, vom Orchestrierungsagent und am Ende generieren wir ein Word Dokument, was in dem Fall jetzt zum Beispiel heruntergeladen werden kann abschließend.

  
45:42  
Noch ein Zielbild, was ich Ihnen zeigen möchte, wieso eine Lösung dann aussehen kann. Tatsächlich, wir haben jetzt nur von einem Kapitel gesprochen, aber sie sind ja interessiert, dann einen ganzen Erläuterungsbericht zu schreiben und wir haben jetzt hier eine Darstellung, also es gibt sowohl User Inputs als auch Aufgaben die die KI übernimmt und dann Ergebnisse und wir würden zum Beispiel als erstes mal Input Dokument relevante Hochladen können und den jeweiligen Kapiteln zuweisen können.

  
46:12  
Ja, das heißt, manche Dokumente sind vielleicht auch relevant für mehrere Kapitel, aber es würde quasi eine gewisse Ordnung geben. Dann hätten wir 3 Kapitel. In diesem Beispiel würden die Input Dokumente nach Relevanz dort einordnen, dann können wir eine schon bereits KI gesteuerte Vorprüfung der Qualität der Input Daten vornehmen, das heißt, man könnte zum Beispiel sagen, manche Dokumente fallen hier durch in der Vorprüfung, weil zum Beispiel eine Vollständigkeit nicht gegeben ist. Bei verschiedenen Input Dokumenten.

  
46:41  
Und ja, das würde ihnen dann quasi auch angezeigt werden und im nächsten Schritt gibt es eine Konfiguration. Jetzt könnte man sagen, OK, wir haben noch nicht alle Dokumente für Kapitel 3. Wir machen erstmal Kapitel 1 und 2 und dort nehmen wir auch eine ausgewählte Input Dokumente für die Generation zur Verfügung, weil wir haben ja gesehen in Schritt 3 ein oder 2 Dokumente, wir haben vielleicht auch die Qualitätsprüfung nicht bestanden.

  
47:07  
So würde ich das konfigurieren und würde dann quasi meine Agenten losschicken. Wir sehen hier die Fähigkeiten, die wir vorhin schon mal genannt haben, die sich an die Arbeit machen und dann sukzessive diese Kapitel erarbeiten und generieren, das Ergebnis ist dann in dem Fall zum Beispiel hier ein Word Dokument, wir haben hier Word gewählt, weil darin können sie einfach wieder arbeiten, das ist ein Format, was sie sofort wieder in die Hand nehmen können und manuell auch noch mal prüfen können, auch vielleicht noch mal. Stichwort human in the loop.

  
47:37  
Wir sind aber noch nicht ganz am Ende von diesem Workflow. Was jetzt passieren kann, ist, dass sie noch mal sagen, die Formatierung stimmen noch nicht 100% das können da von der KI übernommen werden und sie können das an oder abnehmen ablehnen und in einem letzten Schritt kommt noch mal eine Prüfung KI is it touch und am Ende hätte man ein verifiziertes Word Dokument, warum gibt es hier noch mal eine zweite Prüfung?

  
48:01  
Wenn sie jetzt quasi im Schritt in dem ersten Schritt, wo sie ein Word Dokument haben, manuelle Edits machen und Anpassungen machen, dann möchten Sie vielleicht noch nicht noch mal neu generieren, möchten aber immer noch sagen, wie sieht die Prüfung jetzt aus, bin ich immer noch konform mit meinen formalen stilistischen Vorgaben oder mit gemäß den Gesetzen oder hat sich vielleicht auch was geändert?

  
48:23  
Und das kann ihnen dann quasi hier geheihlightet werden. Hier einmal zum Beispiel mit Rot und Grün und Indikation dafür geben. Jetzt haben sie 2 Möglichkeiten, entweder sie machen noch mal manuelle Bearbeitungen und können dann einfach noch mal weiter prüfen oder sie machen tatsächlich den kompletten Cycle einmal zu und sagen, ich würde noch mal anfangen mit einer Generation von von von Anfang an, vielleicht auch mit einem anderen Kapitel, weil zum Beispiel ich andere Quelldokumente habe oder sich darin was verändert hat.

  
48:55  
Ich würde es mal dabei belassen. In der letzten Folie sind nur noch mal der Mehrwert da, aber ich glaube der ist bereits klar geworden aus der vorherigen Präsentation und sie finden es auch noch mal im Nachgang in der in den Slides vielen dank Adrian eine Frage wurde gestellt wie lange in der Regel so ein Projekt dauert, also von der Anforderungsanalyse bis zur Umsetzung.

  
49:22  
Die Implementierung eines solchen Tools, ja ja, also wie bei vielen KI Projekten auch, das kommt immer ein bisschen drauf an. Wir können dann natürlich mit Erfahrungswerten arbeiten, aber es lohnt sich oft natürlich mit einem MVP einmal zu starten oder schnell Mehrwert zu schaffen und zu zeigen im Team und im Fachbereich, dass so was funktioniert und aber auch ein bisschen herauszufinden, wie die das Team vielleicht damit arbeiten möchte und ich glaube, das ist gut erreichbar in.

  
49:51  
33 bis 6 Monaten vielen Dank für die Einschätzung genau, wir würden noch einen kurzen Blick vielleicht auf das Thema Vertrieb setzen und würden so ein bisschen, ich glaube Regulatorik und wie das grundsätzlich funktioniert haben wir verstanden. Vielleicht zeigen wir noch mal einen Case, der so ein bisschen stärker in in Toolnutzung geht, der auch, sage ich mal mehr an der Kundenschnittstelle ist.

  
50:21  
Dani, vielleicht kannst du das zusammenfassen, dann können wir am Ende noch mal 23 Sätze sagen. Wie kann man starten, wie kann man anfangen, wo eignet sich so was und genau fragen gerne weiterhin im Chat sehr gerne. Vielen Dank Björn, Wir schauen uns hier eine Customer Self Service Lösung an, die wir für einen global tätigen Haushaltsgerätehersteller entwickelt haben und.

  
50:50  
Das Spannende war, die haben letztes Jahr experimentiert mit älteren Lösungen, wo die wo die Konversationen im im Chatbot der auf der Kundenwebseite sitzt sehr stark all devired war und und vordefiniert, was wir für Antworten geben, auf welche Frage und das war, das hat einfach der IBM es nicht erlaubt.

  
51:20  
Wirklich ein tolles Kundenerlebnis hier zu ermöglichen, weil das ist auch unser Incentive, weil die Verträge in dem konkreten Falle waren so ausgelegt, dass wir atgom based.

  
51:32  
Insentiviert sind, das heißt je eine bessere Customer Service Solution. Wir entwickeln umso umso Better ist Solution für unsere Kunden und umso besser ist es für IBM, also sind die die Anreize optimal hier gesetzt und deswegen ist der verantwortliche Partner damals auf mich zugekommen und habe mich gefragt, was können wir machen in dem Bereich.

  
52:02  
Ich mit der gentic AI und was wir hier gebaut haben ist wirklich um auch die Frage hier von die die vorher kam an Adrian zu beantworten. Wir haben innerhalb von 8 Wochen auf ein Chatbot Lösung auf der Customer Website komplett auf ein Fully gentic AI Design umgestellt und.

  
52:26  
Wir haben ein Chatbot mit einem holistischen Ansatz, wo wir alle Anfragen über alle Produkte und Informationen auf der Webseite beantworten können, wo wir in 3, ich sag es gleich in 3 unterschiedliche Suchmechanismen greifen können, die wir aufgestellt haben. Wir gehen über solche hardwired Konversationen hinweg und haben adaptive, flüssige, Kontextuell bewusste Konversationen, die sehr natürlich sind mit.

  
52:57  
JGPT powered like of an Experience, wo wir auch viele Multiturning Konversationen haben und haben eine ganze Reihe an Technologien hier reingepackt mit Smart Orchestrations, wo wir zu diesem neuen Credo das Android Corpothy ausgegeben Hab für.

  
53:21  
Large language models as an Operating Systems wo wir den Stateful Flow für Smart Rating greifen, wo wir parallelisierte Ausführungen von Multi Agenten Systemen haben, das heißt, Meta Agenten arbeiten autonom in parallel an gewissen Aufgaben und führen die danach wieder zusammen, wo wir Tool Calling haben und in zum Beispiel Bing Search greifen, wo wir in Elalems as Churches greifen für erneut dieses Fact Checking, dass wir.

  
53:51  
Das wir gerne nutzen möchten, wo wir rekursive Suchmechanismen haben. Das heißt wenn wir feststellen, hey wir haben es im ersten Ron nicht gefunden, gehen wir zurück und suchen nochmals. Wir haben Active Memory Management über die ganze Lösung hinweg und und Self Healing Capabilities und haben fundamental eine skalierbare Architektur über verschiedene Märkte, Brands und und sprachen aufgesetzt und was wir damit erreicht haben.

  
54:22  
War folgendes. Wir haben einerseits unsere Key Containment Matrix mit diesem Fully Agent AI Design um 80% verbessert und vor allen Dingen, und das ist sehr wichtig, wollte der Kunde die Lösung skalieren über verschiedene Märkte hinweg und was wir geschafft haben ist, dass wir das um um die die Zeit umzuskalieren um 75% reduzieren konnten, das heißt es dauert nicht mehr 3 Monate.

  
54:51  
Wie es wir in den in den entsprechenden Markt skalieren können, sondern wir brauchen nur noch 3 Wochen, um einen neuen Markt zu adaptieren und die Lösung in den neuen Markt zu tragen. Und das sind die Business Benefits und wenn wir uns noch kurz unter die Haube schauen, wie das aussieht, dann.

  
55:12  
Sieht das Reforgt aus, also wir? Wir haben hier zum Beispiel verschiedene Fragetypen, die wir einzeln dann klassifizieren können, und das geht dann in einen receptionist Agent, der sicherstellt, dass mal eine Mindestinformation vorhanden ist, die wir benötigen, um die Frage sinnvoll zu beantworten, weil in in vielen Fällen kommen, die kommen die Kunden einfach und schreiben in den Chatbot Kühlschrank, und dann weißt du aber nicht, sind die.

  
55:39  
Irgendwie interessiert an einem Kauf von einem Kühlschrank. Es geht es darum, dass irgendwie der Kühlschrank, den sie haben von uns kaputt ist und sie gerne wissen würden, wie sie, wie sie ihn reparieren können und so weiter also the Reception estation das wie da um so initial.

  
55:55  
The what the why the how the when and Where zu verstehen von dem spezifischen Intent, den die Kunden haben möchten. Und sobald wir den haben, dann steuern wir das hier in sehr kontrollierter Art und Weise die einzelnen Curies durch verschiedene Retriever mechanisms.

  
56:15  
Wo wir eben online Search haben, dass wir auf Client native Content only reduzieren können, weil wir wollen nicht, dass wir irgendwelche newspapers Artikels oder irgendwelche Blogspots da mit Einfangen durch die Onlinesuche, sondern nur Client native Content. Das wäre jetzt bei euch ENBW Native Content only.

  
56:40  
Und können dann in in strukturierte Daten greifen. Für Agentic Retriever, Augmented Generation und und das Lieben unsere Kunden, wir können auch einen FAQ Type of Style vordefinierte Antworten anfertigen, dass zum Beispiel für Promotions und Discounts wollen wir nicht, dass ein Large Language Model sehr kreativ wird und irgendwelche Discounts ausgibt.

  
57:05  
Für die die Firma danach Liabolis, sondern da wollen wir vordefinierte Antworten ausgeben, damit genau das nicht passiert und und wir dann sagen, OK, unsere Discounts findet ihr auf folgender Webseite von uns und könnt ihr dort nachschauen gehen und da haben wir auch über die ganze Prozesskette hier hinweg haben wir Enterprise gerade Filters und Gore Trails, damit wir zum Beispiel auch die Produkte hier nicht vergleichen gegenüber.

  
57:34  
Produkte von der Konkurrenz und all das haben wir in 8 Wochen implementiert und die Lösung ist jetzt live mit unseren Kunden und sie genießen die Vorteile, die ich zuvor erwähnt habe. Genau das ganz kurz und jetzt nehmen wir gerne Fragen auf, die ihr dazu habt.

  
58:01  
Genau. Also ich glaub wir sind schon am Ende der Zeit, wahrscheinlich deshalb verständlich, wenn einige da sind. Ich glaub wir sind noch hier, haben uns sehr gefreut, dass wir heute hier sein durften und wenn da fragen sind oder im Nachgang jemand sagt Mensch Ich hab ein Prozess, der wird sich dafür eignen kann glaub ich ihnen gerne den Kontakt auch herstellen und machen wir sehr gerne ja genau ich glaub eine Frage gab's noch oder eine Wortmeldung.

  
58:30  
Eine Hand war sehr kurz hoch, Fernanda, bitte ja, also war nicht meine Hand, aber ich, ich habe ich habe eine Frage trotzdem, wie ist das mit also technisch mit der Implementierung, also nutzt ihr da Python oder nutzt ihr keine Ahnung NNAN oder wie also wie läuft das auch mit den Modellen also manche Modellen sind Open Source habe ich gesehen in dem Bild von der Präsentation genau also.

  
58:59  
Ja genau, nimm die Frage sehr gerne von einer eigenen Consulting Perspektive.