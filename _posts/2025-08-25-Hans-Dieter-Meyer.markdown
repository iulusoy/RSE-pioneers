---
title: "RSE pioneers - Pioniere des Forschungssoftware-Engineerings: Hans-Dieter Meyer"
excerpt: "Quantum dynamics researcher and developer of the Heidelberg MCTDH software package."
classes: wide
date: 2025-08-25
categories: interview
tags: 
  - theoretical-chemistry
  - quantum-dynamics
  - MCTDH
  - research-software
  - open-source
header:
  overlay_filter: 0.5
  overlay_color: "#0d2476ff"
meyer_gallery:
  - url: /assets/images/meyer-portrait.jpg
    image_path: /01-Dieter-Meyer/dieter.jpg
    alt: "Professor Hans-Dieter Meyer"
    title: "Professor Hans-Dieter Meyer"
  - url: /assets/images/mctdh-software.png
    image_path: /01-Dieter-Meyer/MCTDH.png
    alt: "MCTDH Software Interface"
    title: "MCTDH Software Interface"
  - url: /assets/images/heidelberg-lab.jpg
    image_path: /assets/images/heidelberg-lab.jpg
    alt: "Theoretical Chemistry Lab at Heidelberg"
    title: "Theoretical Chemistry Lab at Heidelberg"
---

Die computergestützte Forschung hat mittlerweile fast alle Fachbereiche ergriffen, und Forschende vor Herausforderungen in der Anwendung und der Entwicklung von Forschungssoftware gestellt. Mit der KI-Revolution steht bereits die nächste Welle an Umwälzungen bevor.
Einige Fachbereiche hat die Digitalisierung des Forachungsprozesses in den letzten 20 Jahren jedoch wenig verändert: Insbesondere die Fachbereiche, die schon immer computergestützt geforscht haben. So zum Beispiel in der theoretischen Chemie: Hier haben Wissenschaftler "schon immer" (seit den 1970er Jahren) Computerprogramme entwickeln und in der Forschung zum Einsatz gebracht, mit allem was dazu gehört - z.B. dem Erlernen von Programmiersprachen, Compilern und Profilern. So entstanden über die Jahre hinweg einige große Programmpackete wie [GAMESS](https://www.ameslab.gov/gamess-open-source-quantum-chemistry-software), [Gaussian](https://gaussian.com/), [Molpro](https://www.molpro.net/), und [andere](https://en.wikipedia.org/wiki/Category:Computational_chemistry_software) - fundamentale Bausteine für die Forschung und Forschungsinfrastrukturen, ohne die viele Erkenntnisse nicht möglich gewesen wären.

Wie haben diese ersten RSEs die Forschung vorangetrieben, welche Faktoren haben Erfolg und Verbreitung von Forschungssoftware beeinflusst? Was sind Unterschiede von heute zu damals? Mit diesen Fragen befasst sich RSE Pioneers.

## Zur Person

Hans-Dieter Meyer studierte Diplom-Physik in Göttingen und schloss seine Doktorarbeit an der Universität Göttingen bei J.P. Toennies in 1978 zu dem Thema "Formation of dimers in rare gas beams from nozzles" ab. Im Anschluss ging er als DFG-geförderter Postdoc zur University of California, Berkeley, USA, wo er bei W. H. (Bill) Miller sich weiterhin mit der Simulation von Streuprozessen befasste. Nach dem Aufenthalt in Berkeley kehrte Dieter nach Göttingen zurück und schloss sich 1980 dem Lehrstuhl für Theoretische Chemie der Universität Heidelberg an (Gruppe von Lorenz Cederbaum). In 1991 habilitierte Dieter zum Thema "Stationäre und zeitabhängige Behandlung molekularer Streuprozesse” und war danach Hochschuldozent, Privatdozent, und ist seit 2005 Apl. Professor an der Universität Heidelberg.

Hans-Dieter Meyer ist der Hauptverantwortliche, Entwickler und langjähriger Maintainer der Open-Source Research Software “Heidelberg-MCTDH” (Multi-Configuration Time-Dependent Hartree). [MCTDH][MCTDH] ist ein hocheffizienter Algorithmus zur Lösung der zeitabhängigen Schrödingergleichung, und ist in Fortran geschrieben (verschiedene Fortran-Dialekte, hinzu kommen Teile in C und Python). Der Algorithmus ist in [mehreren Publikationen][mctdh-refs] und einem [Buch][MCTDH-book] beschrieben, und das Software-Paket, bestehend aus verschiedenen Programmen, wurde etwa 550-mal heruntergeladen. In der Quantendynamik-Community ist MCTDH berühmt für seine Effizienz und hohe Genauigkeit in der Lösung von Wellenpaket-Dynamik-Problemen. Es finden regelmäßig [Workshops und Lehrveranstaltungen zu MCTDH][MCTDH-summer-school] statt. Darüberhinaus entstand die ["High-Dimensional Quantum Dynamics" Konferenzreihe][HDQD-conferences], und es gibt weitere (variierte) Implementierungen des MCTDH Algorithmus in anderen Programmen (Uwe Manthe (Bielefeld), Graham Worth (University College London, [“Quantics”][Quantics]), Haobin Wang (Denver)). Die Publikationen, welche MCTDH vorgestellt haben, sind insgesamt über 5.000 Mal zitiert, die Heidelberg-MCTDH Homepage listet über 300 Publikationen unter Nutzung von MCTDH auf. MCTDH hat daher fundamental zu dem Bereich der Quantendynamik beigetragen und unzählige Forschungsprojekte und Forscherkarrieren geprägt. Ohne die Entwicklung des Algorithmus, aber insbesondere des Software-Paketes, welches den Algorithmus zugänglich gemacht hat, sowie der Betreuung der Nutzer, wäre die Forschungslandschaft um einiges ärmer, und [viele Einsichten hätten nicht gewonnen werden können][MCTDH-highlight]. 

Hans-Dieter Meyer hat laut Google Scholar 358 Forschungsbeiträge veröffentlicht (ResearchGate: 316, Web of Science: 285), die 27.244-mal zitiert wurden (ResearchGate: 22.448, Web of Science: 19.739) (h-Index 75 (ResearchGate: h-Index 68, Web of Science: h-Index 64)).

## Die Anfänge
Hans-Dieter Meyer begann während seiner Doktorarbeit computergestützt zu forschen, damals noch auf Lochkarten und mit Hilfe kleiner Programme zur Datenauswertung, hauptsächlich in Fortran. Das Programmieren hat er sich selber beigebracht, "durchs Abgucken". Anfangs war das Programmieren und Debuggen von Programmen noch deutlich aufwändiger: Erst mit der Anschaffung der ersten Bildschirme und eigener Rechner in den Forschungsgruppen war es möglich, direkter zu Programmieren und Fehler sofort zu korrigieren. All dies war Teil der täglichen Arbeit und integraler Teil der eigenen Forschung.

Anfang der 90er Jahre begann dann die Arbeit an MCTDH: Mit der Entwicklung der Methode und des Algorithmus. Diese bilden zwei Seiten des gleichen Inhaltes ab: Zum einen die mathematische Beschreibung, Näherung und mathematische Validierung des Ansatzes; zum anderen die numerische Repräsentation des Ansatzes (z.B. [Matrixdarstellung](https://doi.org/10.1007/BF01328531)), numerische Transformationen (z.B. [Matrix-Operationen](https://www.netlib.org/lapack/#_presentation)) und Algorithmen (z.B. [Integratoren zur Lösung partieller Differenzialgleichungen](https://numerical.recipes/)). Nach der initialen Implementation der Methode wurde das Programm erweitert und professionalisiert (Anheben des technologischen Reifegrads über den Prototyp hinaus).

## Öffentlichstellung der Software zur allgemeinen Nutzung

<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part1_open_source.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

Nach Erreichen eines höheren Reifegrades der Software war die Freigabe der Software an die Öffentlichkeit ein großer Meilenstein:

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Damals hatten wir auch noch nicht daran gedacht, das Programm öffentlich zu machen. Das kam erst später. Ich weiß gar nicht mehr genau wann, aber das muss auch Ende der 90er oder Anfang 2000 gewesen sein. Wir haben dann diskutiert, ob wir den MCTDH Code öffentlich machen sollen. Das war eine längere Diskussion, das war auch eine schwierige Entscheidung. [...] Aber es war natürlich die einzig richtige Entscheidung.</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Nur dadurch, dass wir das Open Source gemacht haben und den anderen zugänglich gemacht haben und das Programm auch so geschrieben haben, dass es für Leute, die nicht so ganz tief drin sind, wirklich nutzbar ist, hat MCTDH die Verbreitung erfahren.</i> 
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte1_open_source.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i>Sonst wäre es ein kleines Ding nebenher gewesen. Es ist zu kompliziert. Man kann nicht einen Doktoranden sagen, mach das mal, das funktioniert nicht. Man muss einen längeren Atem haben. Den hat man nur, wenn man sich damit verbunden fühlt."</i>
</div>

**IU:** Es ist oft das Sentiment unter den Forschenden, ich habe das geschrieben, das ist meins, ich möchte das nicht öffentlich machen, weil dann nutzen das andere und klauen mir die Ergebnisse. Was würdest du jemandem sagen, oder, was hat euch dazu bewogen, das dann doch freizugeben?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Diese Bedenken hatten wir vielleicht auch, aber das ist altes Denken. Man sollte die Programme freigeben, damit sie nutzbar sind. Es macht ja keinen Sinn, dass jeder das Rad immer neu erfindet und ähnliche Programme schreibt. Das wird deutlich, wenn man an solche Bibliotheken wie LAPACK denkt. LAPACK ist wirklich eine wunderbare Sache. Sehr stark benutzt. Das haben Leute geschrieben, die haben sich die Mühe gemacht und werden jetzt acknowledged und ziert, aber wenn man das nicht freigegeben hätte, so dass nur die eigene Universität diese schönen Programme nutzen kann, das hätte ja nicht so viel Sinn gegeben. Ich glaube, da renne ich inzwischen offene Türen ein. Das war zu der Zeit, als wir uns in den 90er-Jahren entschieden haben, anders. Aber jetzt renne ich da offene Türen ein. Ich glaube, die Leute sehen ein, man sollte die Sachen öffentlich machen."</i> 
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte2_open_source2.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

## RSE Praktiken

<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part2_RSE_practices.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

**IU:** Du hast jetzt die Programmierung und Softwareentwicklung über die Jahre natürlich verfolgt, und wenn du an verschiedene Phasen zurückdenkst, wie siehst du die Wichtigkeit von Programmierung und Softwareentwicklung, zum Beispiel während deiner Doktorarbeit, später als ihr MCTDH releast habt und jetzt in der Forschung?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Das hängt ein bisschen davon ab, wo und wie man forscht. Aber für uns war das natürlich immer essentiell. Theoretische Chemie ist immer sehr programmierlastig. Die Dinge, die man analytisch lösen kann, das haben die Generationen vor uns gelöst. Wir sind sehr darauf angewiesen, das numerisch zu machen. Entweder muss man dann die Programme selber schreiben, das haben wir dann getan. Oder, und dazu haben wir auch beigetragen, man benutzt fertige Programme. Das ist in der Quantenchemie natürlich noch viel mehr verbreitet als in der Dynamik. Aber in der Dynamik gibt es jetzt auch viele Programme, SHARC zum Beispiel für Surface Hopping und MCTDH und andere Pakete. Wir fördern damit einen Trend, den ich gar nicht so gerne mag, nämlich dass junge Doktoranden sagen, ich nehme einfach die fertigen Pakete und rechne damit und mache schöne Ergebnisse und kann ein Paper schreiben, aber habe mir nie die Finger schmutzig gemacht mit Programmieren. Das ist die andere Seite, wenn man das öffentlich macht, aber das ist halt so. Unser Arbeitsgebiet ist sehr computerlastig. Man muss mit Computern umgehen können, man sollte programmieren können und Programme weiterentwickeln. </i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Es ist ja so, dass man immer größere Systeme lösen kann. Das liegt natürlich daran, dass die Computer immer leistungsfähiger werden. Das ist enorm, was in den letzten 20 Jahren passiert ist. Auf was für kleinen Maschinen wir damals gerechnet haben. Aber es liegt auch an den Algorithmen. Die Algorithmen sind sehr viel besser geworden. Man muss an beiden arbeiten. Man kann nicht einfach da sitzen und warten, dass die nächste Computergeneration groß genug ist, um die Probleme zu lösen. Man muss die Algorithmen entsprechend entwickeln und erfinden, und da sind ja enorme Beiträge geleistet worden. MCTDH hat da selber einen großen Beitrag geleistet.</i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte3_algorithms.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i>Dass wir jetzt die Dynamik von Molekülen mit 50 Freiheitsgraden oder so quantenmechanisch berechnen können, das wäre vor 20 Jahren schwer vorstellbar gewesen.<sup>[1]</sup> Das sieht man auch daran, dass gewisse Formate im Output erweitert werden mussten. Als das Programm geschrieben wurde, konnten wir uns nicht vorstellen, dass wir über 100 Freiheitsgrade haben werden. Es wurden nur zwei Digits ausgedruckt. Wir hatten vielleicht 5 Freiheitsgrade, später mal 12 oder so, aber dass wir über 100 gehen, das war jenseits unseres Vorstellungsvermögens. Wir mussten die Formate ändern, damit da nicht Sterne ausgedruckt werden. Und solche Sachen, daran sieht man wie groß der Fortschritt ist, wir konnten es uns einfach nicht vorstellen."</i>
</div>

**IU:** Diese zwei Drehschrauben, also einmal algorithmisch, sieht man ja bei MCTDH wie bei dem Schritt zu ML-MCTDH. Aber dann auch in der Nutzung der Hardware.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Parallelisierung zum Beispiel."</i></div>

**IU:** Mit der Hardware haben sich vielleicht auch die wichtigsten Fähigkeiten geändert, die man braucht zum Programmieren, oder wie siehst du das.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich habe ja noch Programmieren im alten Stiel gelernt, und das habe ich mir schwer abgewöhnen müssen, z.B. das man nicht zu viel Memory verbraucht, dass man arrays, nachdem die gebraucht wurden, wieder verwendet. Das ist natürlich auch sehr fehlerträchtig. Das sollte man vermeiden. Heute ist Memory überhaupt kein Problem mehr. Das ist meistens massig vorhanden. Der ganze Stil des Programmierens hat sich natürlich geändert. Man programmiert heute ein bisschen anders als es früher war. Wir machen nicht unbedingt Objektprogrammierung. Aber in der Richtung ist vieles anders. Die Programmierspanne von Fortran 90 ist etwas anders als Fortran 77, da hat sich viel geändert. Das ist natürlich auch ein Problem für MCTDH. Es ist ja relativ alt. Es gibt noch sehr viele Code, der in Fortran 77 geschrieben ist. Das ist auch nicht änderbar. Niemand will das. Das ist eine zu große Masse. Das bleibt dann. Da muss man sehen, dass man das gut vereint und das alles gut laufen kann."</i>
</div>
**IU:** Es tritt vielleicht auch Lesbarkeit mehr in den Vordergrund, weil mehr wiederverwendet wird.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, genau. Mehr Kommentare reinschreiben."</i></div>
**IU:** Ihr habt ja für MCTDH dann auch Versionskontrolle und Tests genutzt und Dokumentation geschrieben, zum Beispiel. Wie seid ihr darauf gekommen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Zunächst haben wir natürlich sozusagen wild vor uns her programmiert. Wir haben dann ‘99 die erste Versionskontrolle eingeführt. Das war PRCS, ich weiss nicht ob das jemand kennt. Dann wurde uns das aber zu umständlich und zu alt und wir haben dann 2010 Subversion eingeführt. Inzwischen nehmen viele Leute Git. Aber ich bin mit Subversion, mit SVN, ganz zufrieden und das kann eigentlich alles, was ich brauche. Das war natürlich auch ein wichtiger Schritt, dass man das jetzt mal zurückverfolgen konnte was wann geändert worden ist. Vor allem, weil mehrere Leute damals programmiert haben. Eine Versionskontrolle ist unglaublich hilfreich, weil man wieder zurückgehen kann und sehen kann, was da gemacht worden ist, wo der Fehler eingebaut worden ist, falls es einen gab."</i></div>
**IU:** Und die Tests?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Wir haben eine Testroutine geschrieben. Ich glaube, es gibt so 50 Inputs. Die werden dann abgearbeitet. Aber es ist eigentlich zu wenig. Mit den Inputvariablen kann man MCTDH unheimlich fein steuern. Es ist halt ein sehr generelles Programm zur Lösung der Schrödinger Gleichung unterscheidbarer Teilchen. Man kann unheimlich viele verschiedene Dinge damit machen. Insofern gibt es immer wieder Probleme, weil Leute etwas ausprobiert haben, woran wir nie gedacht haben. Und dann in Schwierigkeiten geraten. Insofern lerne ich viel von den Nutzern. Die schreiben mir dann eine Email, und dann sehe ich ein, da müssen wir was ändern, da sollten wir was ändern. Das ist sehr schön. Ganz zu Beginn hatte ich mal gehofft, dass die Leute einen Beitrag leisten, vielleicht irgendwie eine Auswertroutine schreiben. Aber das ist eigentlich nie passiert. Sie kommen immer nur mit Complaints wie “es funktioniert nicht gut genug” oder “da müsste man etwas machen” und dann müssen wir halt was machen. Das andere Forscher etwas zum MCTDH code beitragen, die Hoffnung hat sich leider kaum ergeben."</i></div>
**IU:** Darauf werde ich nochmal zurückkommen. MCTDH lässt sich aber auch sehr einfach kompilieren auf allen möglichen Hardwares.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, das läuft auf einem Laptop bis hin zu Supercomputern."</i></div>
**IU:** Habt ihr eine Strategie verfolgt, dass ihr es überall ausgetestet habt, oder ist das mit der Zeit gewachsen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Das ist mit der Zeit gewachsen. Linux ist eine wunderbare Sache. Linux läuft auf allen Rechnern. Gott sei Dank läuft es auch auf Apple Computern. Es ist zwar nicht Linux, aber ein Unix-System. Da muss man ein bisschen anpassen. Wenn man einen Apple Laptop hat, läuft MCTDH da auch. Wenn man einen Windows-Rechner hat, sollte man Linux installieren wenn man MCTDH nutzen möchte. Und auf den Hochleistungs-Rechnern läuft in der Regel immer Linux. Insofern war da eigentlich wenig zu tun. Wir testen immer alles mit den GNU-Compilern."</i></div>
**IU:** Ihr habt MCTDH nutzbar gemacht und unter Versionskontrolle gestellt, usw. Ihr habt praktisch beste Praxis angewandt, obwohl es den Begriff an sich noch nicht gab. Hast du das nach außen hin mal diskutiert? Oder war das überhaupt ein Thema mit anderen Forschenden oder auch in der Gruppe? Dass andere gesagt haben, warum macht ihr das? Oder wir wollen das nicht machen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Zu Beginn haben wir das lange diskutiert, bevor wir es gemacht haben. Aber danach war die Entscheidung ja da. Ich kann das auch nur anderen wieder empfehlen, dies zu tun. Das ist die einzige Möglichkeit, dass das die Arbeit nicht irgendwie untergeht. Es gibt unheimlich viel Software, die irgendwann mal geschrieben und dann vergessen wird. Man möchte die vielleicht gerne nutzen, aber dann ist der Doktorand, der sie geschrieben hat, nicht mehr da. Das ist vielleicht ein Punkt, den ich auch mal hervorheben will.</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i> Wenn man das öffentlich machen will, muss man auch eine gute Dokumentation schreiben. Und das ist lästig, das macht keinem so richtig viel Spaß. Programmieren macht oft Spaß, aber Dokumentation schreiben etwas weniger. Aber das ist unglaublich wichtig. 
</i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte4_documentation.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i>
Gerade wenn es dann so komplex wird wie MCTDH. Ich gucke selber in die Dokumentation, weil ich vergessen habe, wie genau lautet das keyword, um diese oder jene Funktion einzuschalten. Eine gute Dokumentation ist ganz essentiell. Ich glaube, dass viel Software nicht nutzbar ist, liegt daran, dass sie nicht ausreichend gut dokumentiert ist."</i></div>
**IU:** Und mit der Dokumentation, wer hat angefangen, die zu schreiben?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Inzwischen gibt es viele Tools, die wir aber gar nicht benutzt haben, weil es die Tools noch gar nicht gab. Wir schreiben das alles in HTML. Und dann haben wir noch andere Dinge geschrieben. Ein User’s Guide gibt es noch, der ist in LaTeX geschrieben. Und es gibt auch noch eine sogenannte Lab Session. Das ist ein Tutorial, mit dem man verschiedene Inputs ausprobieren kann und dann lernen kann, MCTDH zu benutzen. Aber das sind mehr so Handreichungen, um MCTDH zu nutzen und es zu lernen. Die HTML-Dokumentation ist in der täglichen Arbeit sehr hilfreich, wenn man genau wissen will, wie muss der Input aussehen, wenn ich das und das machen möchte."</i></div>

[¹] Die Behandlung von Modellen wie Spin-Boson, vibronic-coupling Hamiltonian, generalized Henon-Heiles etc. ist sehr viel einfacher. Pyrazin mit seinen 24 Freiheitsgraden konnten wir schon 1999 lösen und heutzutage sind Modelle mit mehreren 100 Feiheitsgraden lösbar.

## Wissenschaftliche Durchbrüche durch MCTDH
<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part3_MCTDH_breakthroughs.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** Gibt es Personen, die dich in der Entwicklung von Forschungssoftware beeinflusst haben? Gab es irgendwo bestimmte Momente oder Wendepunkte, Personen, die dir geholfen haben, eine bestimmte Strategie zu verfolgen, so etwas in der Art?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, ich hatte Glück, dass Graham Worth relativ früh, das war ‘94, zu meiner Arbeitsgruppe hinzu kam. Er hatte viel Erfahrung mit Programmieren. Wir haben eigentlich viel von ihm profitiert. Er hat das Ganze ein bisschen mehr professionalisiert, würde ich mal sagen. Er war dann hier Postdoc bis Ende 2000. Dem bin ich zu Dank verpflichtet. Ich habe von ihm auch einige Programmiertipps gelernt. Und dann Frank Otto, der war ein Doktorand, das war so ein Computerfreak. Der hat ja schon auf Ataris oder so als Schüler rumprogrammiert. Der hat uns auch bei einigen Dingen geholfen, so irgendwelche komplizierten Skripte geschrieben oder solche Sachen. Wenn man Mitarbeiter hat, die mehr können als man selbst, ist das sehr schön. Und sonst vom Programmieren so herausragend, da ist Haobin Wang zu nennen, der ML entwickelt hat. Nicht bei uns, in den Vereinigten Staaten. Ich war 2001 dort zu einer Geburtstagsfeier von Bill Miller. Dort habe ich Haobin Wang kennengelernt. Und der hatte angefangen, Multilayer MCTDH (ML) zu entwickeln. Wir haben das dann viel diskutiert, weil wir ähnliche Ideen hatten. Wir hatten das Cascading genannt. Aber wir haben da nie wirklich was gemacht. Das erschien uns einfach zu komplex. Und wir sagten, wenn wir uns da jetzt ransetzen und das programmieren, und das funktioniert nicht, dann machen wir uns sehr viel Arbeit für nichts. Aber Haobin Wang hat das einfach gemacht. Und das hat wunderbar funktioniert. Und dann haben wir das alle nachgemacht. Insofern ist er mein Hero."</i></div>
**IU:**Und als Wendepunkt, das kam ja jetzt schon ein paar Mal hoch, war die Öffentlichmachung von MCTDH. Aber gab es noch irgendwelche anderen Punkte, an denen ihr die Richtung geändert habt?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Eigentlich nicht so sehr. ML, das ist Multilayer MCTDH, ist für größere Systeme ein wichtiger Schritt nach vorne. Das Heidelberger ML hat im wesentlichen Oriol Vendrell programmiert. Und wir hatten auch keinen großen Plan. Die Probleme kamen auf uns und zu und wir haben sie dann versucht zu lösen. Wir haben versucht, es immer weiter besser zu machen. [...] Was in den letzten Jahren eine starke, wichtige  Entwicklung war, war das Umschreiben vom allgemeinen Potentialprogramm in die sogenannte Sum-of-Products-Form. [...] Man kann das Potential in eine kompaktere Form bringen, in die sogenannte CPD-Form auch bekannt unter den Namen CANDECOMP oder Parallel Factors. Da hat Markus Schröder einen riesigen Beitrag geleistet, denn jetzt haben wir ein Programm haben, MCCPD, Monte Carlo CPD, was allgemeine Potentialflächen ind sum-of-products Format bringt. Die Quantenchemiker stellen der wissenschaftlichen Gemeinschaft Programme zur Verfügung, da gibt man Koordinaten vor und sie returnen die potentielle (Born-Oppenheimer) Energie. Das heißt, sie haben ein Potential-Fit generiert, aber das ist ein allgemeiner Fit und diesen refitten wir im auf diese Sum-of-Products Form. Das war jetzt ein ganz großer Schritt, weil wir damit wirklich große Systeme behandeln können. Das Letzte, was wir in Zusammenarbeit mit Fabien Gatti und anderen gemacht haben, war Wasserstoff auf einer Graphitfläche und da haben wir mehrere Graphitatome mitgenommen, die sich dann bewegen können und die Energie transferieren können. Und das war ein ganz großer Schritt, denn dies führte zu 75 Freiheitsgraden. Und dann die Fläche mit 75 Freiheitsgraden zu refitten, das hätten wir vor ein paar Jahren noch für nicht denkbar gehalten. [...]
Ein anderer wichtiger Punkt, wiederum nicht direkt MCTDH aber für MCTDH sehr wichtig, ist die Herleitung des Operators der kinetischen Energie. Wenn man so kleine Systeme wie Wasser oder HONO oder so behandelt, da kann man die kinetische Energie per Hand herleiten und programmieren. Aber wenn die Systeme größer werden wird es schwierig. Wir wollen ja nicht so etwas wie Normalkoordinaten nehmen, dann ist alles simpel, sondern es ist sehr, sehr wichtig, dass die Koordinaten den natürlichen Bewegungen folgen oder die natürlichen Bewegungen gut beschreiben. [...] Und dann wird die kinetische Energie unfassbar kompliziert. Glücklicherweise ist dann in Zusammenarbeit mit David Lauvergnat und Fabien Gatti ein Programm entstanden, das heißt Tana, und das berechnet diese kinetische Energie analytisch und schreibt sie dann in einem Format, das man direkt in MCTDH einlesen kann. Ohne das hätten wir auch die großen Systeme nicht mehr machen können. Wir haben damals, 2007, das Spektrum des protonierten Wasser-Dimers, also des Zundel-Kations, berechnet. Das war ein großer Durchbruch. Im Zundel-Kation hält ein Proton zwei Wassermoleküle zusammen. Es gibt Bewegungen großer Amplitude in einem sehr anharmonischen Potential. Damals haben wir noch mit Fabien Gatti zusammen, also er hat das gemacht, die kinetische Energie sozusagen per Hand erstellt, mit Überprüfung durch numerische Verfahren (Tnum). Der kinetische Operator ist in einer sum-of-products Form mit etwa 150 Termen dargestellt. Das war eine lange Arbeit, aber es war möglich. Aber für Moleküle, die wir kürzlich berechnet haben, wie das Eigenkation (33D), das wäre gar nicht mehr möglich gewesen. Für den refit des Potentials (mit MCCPD) haben wir 2048 Terme in der sum-of-products Form benutzt, die Darstellung der kinetischen Energie benötigte fast 2500 Terme. Das kann man nicht mehr per Hand machen. Das ist ganz essentiell. Das sind also so Dinge, die parallel zu MCTDH laufen, aber für MCTDH absolut essentiell sind. Diese Entwicklungen sind in den letzten Jahren entstanden und haben uns natürlich sehr geholfen. Damit können wir diese großen Systeme berechnen. [...]"</i></div>
**IU:** Das zeigt ja beispielhaft auch, wie man sich nicht darauf verlassen kann, dass Computer besser werden und man rechnet einfach größere Systeme. Man braucht eben auch, also das Problem ändert sich, die Darstellung ändert sich und die muss abgebildet werden.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Man braucht eine Entwicklung der Algorithmen, ganz sicher. Und an viele Algorithmen denkt man vorher gar nicht. Erst wenn das Problem da ist und so groß wird, dass es wirklich nagt, dann fängt man an, überhaupt über neue Algorithmen nachzudenken. Insofern bin ich auch glücklich, dass MCTDH, das ist ja inzwischen, also 1990 haben wir angefangen, das ist ja 35 Jahre alt, das ist ja älter als mancher Zuhörer dieses Podcasts, dass es immer noch lebt. Denn ich war mir immer bewusst, irgendwann kommt jemand mit einer ganz neuen Idee und man macht das ganz anders und es geht viel schöner und besser. Aber MCTDH hat sich gehalten. Natürlich weil wir es immer weiterentwickelt haben mit ML und so, was ein sehr wichtiger Schritt war. Aber es ist immer noch eine sehr gute Methode und kann immer noch mithalten und ist immer noch ganz, ganz vorne dabei."</i></div>

## Entwicklung von Forschungssoftware im akademischen Umfeld
<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part4_academic_environment.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** Wenn du jetzt so daran denkst, das ist ja eine Entwicklung von Forschungssoftware in der Forschungslandschaft und du hast ja erwähnt, du hast ja Doktoranden gehabt, die daran gearbeitet haben und so weiter. Wo siehst du kritische Punkte in der Entwicklung von Forschungssoftware im universitären Umfeld?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, ein kritischer Punkt ist die Finanzierung. Die DFG finanziert sowas nicht, sondern sie finanziert nur wissenschaftliche Forschung und wenn man dazu vielleicht ein bisschen Programmierentwicklung machen kann, dann kann man das ja machen, aber man kann nicht in einen Antrag schreiben, ein Programm zu entwickeln oder so."</i><small>[Anmerkung: Ein DFG Antrag von Dieter wurde aus diesem Grund abgelehnt].</small> <i>"Das funktioniert nicht. Und das ist anders in England. Graham Worth hat Gelder bekommen, extra für Programmentwicklung. Er hat dann einen Fork gemacht vom Heidelberger MCTDH, nennt es QUANTICS und da hat er speziell Geld dafür bekommen, das zu entwickeln. So etwas fehlt in Deutschland. Das war für mich immer ein Krampf. Man musste immer ein wissenschaftliches Projekt haben und man wollte aber eigentlich Programmentwicklung machen. Wir wollten natürlich auch Anwendungen machen. Natürlich, das auch. Wir machen ja die Entwicklung nicht nur so ins Blaue hinein. Wir machen es um Anwendungen durchführen zu können. Aber um es in einem DFG-Antrag durchzukriegen, muss man es umgekehrt schreiben. Man muss es so schreiben, dass die Anwendung im Vordergrund steht und die Entwicklung, die läuft dann so nebenher. Aber dazu ist Softwareentwicklung zu wichtig. Und ich hoffe, dass sich da mal ein bisschen was ändert."</i></div> 
**IU:** Und dann habt ihr praktisch neue Fragestellungen bearbeitet und dabei auch ein bisschen Programmwartung übernommen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, natürlich. Zu Beginn haben wir angefangen mit H+H<sub>2</sub>-Streuung und solche Sachen. Und das haben wir in den Vordergrund gestellt und dafür auch schöne Papers geschrieben. Im Laufe dieser Arbeiten wurde MCTDH entwickelt. Aber die Anträge liefen natürlich immer über das Projekt, das untersucht worden ist."</i></div> 
**IU:** Und abgesehen davon, dass man ja auch Geld braucht, um die Leute zu finanzieren, dass sie die Software entwickeln, ist es ja auch so, dass daraus nicht direkt immer ein Paper entsteht. Wie siehst du das, wie kann man diese Beiträge würdigen oder ist das in der Vergangenheit gewürdigt worden, wenn Doktoranden Beiträge geleistet haben?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, wie gesagt, das Geld gibt es nur für die Forschung, die dann rausgekommen ist, dass da noch irgendwas berechnet worden ist, ein Wirkungsquerschnitt oder ein Spektrum oder so weiter. Und die eigentliche Programmentwicklung, die wird so nicht gewürdigt. Ich meine, ich würdige sie natürlich, aber vom Geldgeber her nicht so sehr. Und das ist der Punkt, den ich kritisiere, dass man da mehr flexibel sein muss."</i></div>
**IU:** Das hat ja vielleicht auch Einfluss auf die Karriere der Doktoranden, wenn die halt die Zeit investieren, dann wird das nicht angerechnet.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, ja, ich hatte mal einen Postdoc, der kam und sagte, er möchte eigentlich nicht so gerne Programmentwicklung machen, er brauche ja Papers für seine Karriere. Das habe ich eingesehen, dann haben wir mit ihm schöne Sachen gemacht. Das ist dann so. Also solche Argumente kommen schon und das habe ich in dem Sinne auch unterstützt. Bei Doktoranden ist es einfacher. Ein Doktorand, der muss eine Doktorarbeit schreiben, aber der denkt vielleicht noch nicht so sehr an seine Karriere in dem Moment."</i></div>
**IU:** MCTDH hat ja einige Publikationen, die dann auch zitiert werden sollen, wenn man das Programm nutzt. Denkst du, das ist ein guter Weg, um diese Beiträge zu würdigen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, ich glaube, ich sehe keinen anderen. Es war ja auch ein langer Weg. Inzwischen ist es sehr bekannt und alle Leute sagen, das ist eine sehr gute Methode und kennen es und highlighten es. Aber zu Beginn war das schwierig. Es war den Leuten doch sehr fremd. Und ich weiß, unser erster wirklich großer Durchbruch war Pyrazin. Das ist ein Vibronic Coupling-System mit 24 Freiheitsgraden. Um es vielleicht auszuführen: Es gibt zwei Arten von Problemen. Das eine sind diese Modelle, wie Vibronic Coupling-Modelle und so, die sind automatisch in Sum-of-Products Form. Insofern eignen sie sich sehr. Und dann gibt es die wirklichen Moleküle, deren Potentialenergieflächen ab initio berechnet worden sind, wo wir dann den Schritt machen müssen, das Potential in Sum-of-Products auszudrücken.</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Und das Pyrazin war so ein Modell, ein Vibronic Coupling-Modell, und das konnten wir 1999 lösen. Das ist lange her. Und wir hatten gedacht, das ist so ein großer Durchbruch. Aber es hat relativ wenig Resonanz ergeben, denn wir waren einfach zu weit vorne. Die anderen Leute machten zwei oder drei Freiheitsgrade, und wir machten 24. Das haben die nicht so ganz richtig verstanden, gedacht das ist sowas ganz Spezielles, das sind harmonische Oszillatoren und so. Aber das ist Vibronic Coupling. Das ist sehr, sehr, sehr anharmonisch. Von den Autoren ist niemand eingeladen worden, mal zu einem Vortrag darüber, in den folgenden zwei Jahren oder so. Später ist unsere Arbeit sehr anerkannt worden. Pyrazin ist ein Standardmodell geworden, um andere Methoden zu testen. Viele semi-klassische Methoden versuchen Pyrazin zu lösen, ja, das hat sich stark geändert. Aber das ist mir immer noch sehr in Erinnerung, als wir Pyrazin gelöst haben, hatten wir gedacht haben, jetzt kriegen wir großen Applaus. Nichts. Die Anerkennung kam mit Verzögerung. </i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte5_breakthrough.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i> Sie kam mit deutlicher Verzögerung. Ein anderer großer Durchbruch war das Zundel-Kation, weil das wirklich ein echtes Molekül ist, nicht ein Modell. Mit 15 Freiheitsgraden, das war auch zu dem Zeitpunkt weit besser, mehr als andere Leute konnten. Wir konnten das wirklich vollständig analysieren und lösen. Das war ein großer Schritt. Da haben wir auch viel Anerkennung bekommen. Das war noch alles vor ML, das war mit MCTDH gemacht worden. Das hat groß zur Anerkennung und zur Akzeptanz von MCTDH geführt. Inzwischen ist das alles natürlich kein Problem mehr. Aber im Beginn schon."</i></div>

<div style="display: flex; align-items: center; margin: 1rem 0;">
<img src="/01-Dieter-Meyer/zundel_molden.png" alt="Das Zundel-Kation." style="width: 50%; height: auto; margin-right: 1rem;">
<div style="flex: 1; font-style: italic; color: #666;">Im Zundel-Kation hält ein Proton zwei Wassermoleküle zusammen. Es gibt Bewegungen großer Amplitude in einem sehr anharmonischen Potential, und der kinetische Operator ist in einer sum-of-products Form mit etwa 150 Termen dargestellt.</div>
</div>

## Entstehen einer Community
<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part5_community.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** MCTDH wird ja auch durch viele Menschen genutzt in der Forschung. Die basieren dann ihre Forschung wieder auf der Verfügbarkeit und Nutzbarkeit von MCTDH. Siehst du da kritische Punkte? Eine Nutzer-Community zu haben in der Forschungslandschaft? 
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Nein, es ist eigentlich sehr schön. Es ist klar, dass Leute das MCTDH-Programm runterladen und nutzen. Und dann vielleicht wieder anderen Problemen zuwenden, das ist der Lauf der Dinge. Sie machen das nicht unbedingt ihr ganzes Forscherleben wie ich es in den letzten Jahren gemacht habe, sondern sie haben ein bestimmtes Problem, wenden da MCTDH an. Dann machen sie vielleicht was anderes. Manche bleiben dabei, benutzen MCTDH kontinuierlich für fast alle ihre Sachen. Das ist unterschiedlich. Ich kriege auch manchmal eine E-Mail von irgendeinem Studenten vielleicht aus China oder so, der MCTDH haben will. Da habe ich dann schon große Bedenken, dass das was wird. Wenn jemand das alleine machen will, das ist zu komplex, wenn man kein Umfeld hat. Wenn sozusagen der Professor sagt, mach das mal. Dann muss es schon ein sehr, sehr guter Student sein, dass er es schafft. Dann höre ich auch nie wieder was davon. Man muss schon ein Umfeld haben, wenn jemand aus dem Quantenchemie-Umfeld kommt und sagt, jetzt machen wir mal Dynamik. Das ist eine andere Denkweise. Quantendynamik, auch die Zeitabhängigkeit. Ich stelle immer wieder fest, dass das den Leuten schwer fällt. Es gibt Leute, die denken sehr in Eigenzuständen und jetzt sollen sie in Wellenpacketen denken. Wenn man so ein Einzelkämpfer ist, ist das schwer. Man braucht schon eine gewisse Umgebung und eine Unterstützung. Dann kann das gut gehen. Ein anderer Punkt, der mir gerade dabei einfällt, wir machen es dieses Jahr wieder, und wir haben es vor zwei Jahren gemacht: Eine MCTDH-Summer-School. Und, letztes Mal hat einer der Schüler Kritik geäußert, MCTDH ist zu kompliziert. Das ist nicht wahr, die Quantendynamik ist kompliziert. MCTDH versucht es so einfach zu machen wie möglich. Aber Quantendynamik ist kompliziert. Einfach Trajektorien rechnen ist schon einfacher, das sehe ich ein. Da kriegt man vielleicht schnell ein Paper. Man rechnet ein paar Haufen Trajektorien und analysiert das ein bisschen. Aber Quantendynamik, die volle Quantenmechanik, ist kompliziert, das ist klar. Da muss man sich reinhängen. </i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i> Auch wenn einem durch das MCTDH-Projekt die Programmierung abgenommen worden ist, die intellektuelle Leistung, sich damit zu beschäftigen, die kann einem niemand abnehmen. Die muss man dann bringen."</i></div>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte6_understanding.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** Also die Nutzer müssen schon auch verstehen, was da passiert, worauf sie es anwenden können und dafür reicht dann einfache Dokumentation nicht aus. Man muss auch in die Methode einsteigen, in dem Paper. Deswegen gibt es auch das Buch. Vielleicht, das ist so das eine, dass sie den Bereich verstehen. Aber dann gibt es vielleicht in der Anwendung wieder Fragen, wie schreibe ich jetzt das Operator-File? Was muss ich da tun? Da bekommt ihr sicherlich auch viele Nutzer-Anfragen mit Fragen zur Unterstützung.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, ja. Ich kriege manchmal einen Input und raufe mir dann die Haare. Aber im Großen und Ganzen ist es gar nicht so kompliziert, auch das Operator-File. Wir haben ein extra ASCII-File, in das man reinschreibt, wie der Operator aussieht, wie der Hamiltonian auszusehen hat. Das kann man über diese Sum-of-Products Struktur ziemlich gut definieren. Es gibt eine ganze Library von Operatoren, die man dann einbinden kann. Erste Ableitung, zweite Ableitung, irgendwelche Funktionen usw. Das kann man, glaube ich, ganz gut lernen. Wenn man das Input-File schreibt, muss man eine gewisse Vorstellung haben über verschiedene Punkte haben, z.B. wie eine Basis funktioniert.  Manchmal funktioniert was nicht, weil z.B. die Gitterpunkte viel zu grob gewählt sind. Dann gibt es gar keine Konvergenz in der primitiven Basis. Dann kann gar nichts funktionieren. Dann ist es nicht ein Fehler von MCTDH, sondern ist es wirklich ein Inputfehler. Ich kriege manchmal Anfragen und einen Input und warum funktioniert das nicht. Dann versuche ich zu helfen."</i></div>
**IU:** Das kostet dich ja auch wieder Zeit.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Das kostet mich wieder Zeit, aber ich bin ja pensioniert und habe die Zeit."</i></div>
**IU:** Von daher können sich diese Nutzer dann auch wirklich glücklich schätzen. Weil es schwierig ist, die Zeit zu finden und Support zu leisten. Im Prinzip kann man das auch über Forschungsprojekte gar nicht finanzieren.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Genau. Das ist wieder dieser Punkt, den wir schon besprochen haben. Dass da die DFG vielleicht mal ein bisschen die Politik ändert."</i></div>
**IU:** Natürlich ist die Methode viel verbreitet worden und viel angewandt worden. Du hast ja auch schon angesprochen, dass die Nutzer zwar keinen Code zurück beigetragen haben, aber dadurch, dass sie Fehler gefunden haben, sie durchaus dazu beigetragen haben.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich habe viel gelernt von den Nutzern. Einerseits, weil sie auf Fehler aufmerksam gemacht haben oder Fragen gestellt haben, die klargemacht haben, dass der Input oder die Dokumentation ein bisschen missverständlich war. Dass man das so verstehen kann, wie der Nutzer das verstanden hat, aber ich das gar nicht so gemeint habe. Und dass man dann da ein bisschen oder auch ins Programm noch irgendwelche Fehlermeldungen einbaut. Man macht einen Input, der unsinnig ist und dann soll MCTDH das vielleicht entdecken und sagen, das ist eine nicht erlaubte Kombination von Dingen. Ich habe dann oft eine Fehlermeldung eingebaut, die das Programm stoppt und auf den fehlerhaften Input hinweist. Insofern lerne ich immer viel von den Nutzern."</i></div>
**IU:** Und du hast ja auch angesprochen, ihr habt ja auch schon eine Summer School gemacht und planen jetzt wieder eine. Wie ist die Idee entstanden, die Summer School zu machen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich glaube, die kam von Oriol. Ich weiß nicht genau, irgendwie kam die Idee auf, das sollten wir mal machen. Und das haben wir dann vor zwei Jahren gemacht, das war sehr schön. Und wir machen sie dieses Jahr wieder, Ende Juli. Und ich glaube, die Deadline ist abgelaufen, man kann sich nicht mehr bewerben, aber es kommen so etwa 50 Leute. Und wir machen sie etwas konzentrierter. Die erste Summer School war ein bisschen breiter, da haben wir auch Leute von MCTDHB und MCTDHF dazu genommen. Also MCTDH ist ein Programm zur Lösung der Schrödinger-Gleichung für unterscheidbare Teilchen und kann somit die Molekulardynamik lösen. Aber dann gibt es natürlich auch identische Teilchen, also Fermionen wie Elektronen, oder Bosonen. Die Bosonenforschung ist ja ein Schwerpunkt in der Physik, also ultrakalte Physik usw. Und da haben Leute Programme geschrieben, die diese Symmetrien einbauen. In der letzten summer-school gab es  eine Session, MCTDHB und MCTDHF, aber die haben wir jetzt rausgenommen. Wir wollen uns mehr auf das eigentliche MCTDH konzentrieren. Gleicherweise haten wir damals noch einen Vortrag über Tensor Trains und DMRG und solche Sachen, die mit MCTDH verwandt ist. Auch das nehmen wir jetzt raus. Diese Summer School ist mehr auf die Anwendung von MCTDH konzentriert und dass  die Teilnehmer lernen, MCTDH zu benutzen und dann wieder stöhnen können, wie kompliziert das ist. Das hat mich sehr amüsiert."</i></div>
**IU**: Und ihr habt aber auch eine Konferenzserie.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, wir haben die High Dimensional Quantum Dynamics Serie, HDQD, die finded im Prinzip alle zwei Jahre statt. Die Thematik der Konferenz ist natürlich nicht allein auf MCTDH ausgerichtet, sondern eben auf High Dimensional Quantum Dynamics. Aber MCTDH hatte natürlich immer eine sehr starke Bedeutung, eine sehr starke Betonung. Zu Beginn hatte ich diese Konferenz-Reihe organisiert. Inzwischen mache ich das nicht mehr, inzwischen macht das ein Committee. Zu Beginn war ich das alleine, ich habe immer versucht  jemanden zu finden, der die HDQD ausrichtet. Und es war zu Beginn schwierig. Später hat sich das geändert, dann kamen die Leute zu mir und wollten eine HDQD ausrichten. Und inzwischen ist es relativ etabliert. Und es gibt ein Committee, das jetzt entscheidet, wer die Konferenz ausrichtet. Die vorletzte HDQD war in Groningen, die habe ich noch zugeteilt. Und die allerletzte war in Hamburg, 2024. Und die nächste wird, glaube ich, in Spanien sein. Also in 2026 wird es dann wieder eine HDQD geben, alle zwei Jahre."</i></div>
**IU:** Und wie viele Teilnehmer habt ihr da im Moment?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "So 150 vielleicht. Wir haben klein angefangen, mit etwa 50 Teilnehmern. Die erste Konferenz war 2005 in Leiden mit Geert-Jan Kroes. Der hat mal einen Sabbatical hier in Heidelberg gemacht. Er kam zu mir und sagte, er würde gerne mal eine Konferenz organisieren, ob ich da mitmachen wollte. Ich hasse Organisation. Eine Konferenz hätte ich von mir aus nicht gemacht. Aber er hat die in Leiden im sogenannten Lorentz-Center gemacht. Das heißt, die eigentliche Organisation ist dort gemacht worden. Da hatte ich nichts mit zu tun. Ich hatte nur mit der wissenschaftlichen Organisation zu tun, Auswahl der Speakers, Aufstellung des Programms usw. Das habe ich natürlich gerne gemacht. Und dann haben Geert-Jan Kroes und ich die HDQD ins Leben gerufen. Und das war ein großer Erfolg, die Leute waren so begeistert, es war eine Konferenz, die war mehr aufs Technische fokussiert. Was sind die Methoden, um High Dimensional Quantum Dynamics zu lösen? Vom Stil eine andere Konferenz. Und die Leute waren so begeistert, dass sie gesagt haben, das machen wir wieder. Und dann habe ich versucht, das alle zwei Jahre zu organisieren, was mir nicht immer gelungen ist. Sie fiel dann mal aus, und so waren es mal drei Jahre zur nächsten HDQD, und wegen Covid auch einmal vier. Aber ich habe immer jemanden gefunden, der eine HDQD organisiert, und zwar in Montpellier, Birmingham,  Mittelwihr, Rostock,  Lille und Groningen. Jetzt ist es mehr organisiert, der Stil hat sich auch geändert, ein bisschen zu meinem Bedauern. Aber es war so eine Konferenz on the point. Es war wirklich mehr von und für Leute, die Programme entwickeln. Und jetzt ist es doch mehr eine allgemeine Konferenz. Sie unterscheidet sich nicht mehr so stark von anderen Konferenzen. So ist der Lauf der Dinge. Es ist auch größer geworden. Wir hatten 50, jetzt steuern wir mehr auf die 150, 200 oder so zu. Es ist eine ganz normale Konferenz geworden. Aber der Schwerpunkt High Dimensional Quantum Dynamics ist geblieben."</i></div>
**IU:** Also habt ihr da so eine Community, die ist gewachsen, und ...
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, das entscheidet jetzt das Steering Committee, ich bin gar nicht mehr dabei."</i></div>
**IU:** Also das Profil hat sich ein bisschen geändert von wirklich Entwicklung hin zu Anwendung vielleicht?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, mehr zur Anwendung und ein bisschen breiter. Wir haben jetzt auch semiklassisches und so. Aber ich kann sie sehr empfehlen. HDQD ist wirklich eine sehr schöne Konferenz."</i></div>

## Ausblick
<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part6_future.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** Und euer Code ist ja jetzt über die Jahre gewachsen. Du meintest, es sind jetzt 35 Jahre. Und gibt es da bestimmte Herausforderungen, die schwierig sind anzugehen, wenn man so einen Code hat, der über die Jahre entwickelt wird?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, natürlich. Dadurch, dass der Code so alt ist, Teile sehr alt sind, wäre es schön, sozusagen von Scratch neu zu schreiben. Aber das ist unmöglich. Wir haben die Manpower auch nicht. Ich hatte ja früher drei, vier Leute, die MCTDH entwickelt haben. Inzwischen bin ich mit Markus Schröder praktisch alleine. Ich habe ja niemanden mehr. Ich bin ja pensioniert. Wir machen also nicht mehr so viel Entwicklung wie zu Beginn. Das ist ja auch nicht mehr so nötig. Im gewissen Sinne ist MCTDH ja auch abgeschlossen. Wir machen nur Erweiterungen, die uns jetzt so auf den Fingern brennen. Diese Potentialerweiterung war sehr, sehr wichtig. Inzwischen arbeitet Markus ein bisschen an einem Programm, um Eigenzustände zu berechnen. Da gibt es das Improved Relaxation. Aber er möchte zu größeren Systemen gehen, wo Improved Relaxation nicht mehr funktioniert. Ein bisschen Entwicklung gibt es noch, aber nicht mehr so wie in den Anfangsjahren, wo drei, vier Leute hauptsächlich daran gearbeitet haben. Ich beantworte hin und wieder mal eine Nutzeranfrage, aber machen tu ich nicht mehr so viel."</i></div>
**IU:** Du meintest ja auch schon, dass viele, die MCTDH nutzen oder vielleicht auch in der Gruppe daran arbeiten oder damit arbeiten, nicht wirklich an dem Programm selber arbeiten.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, um das Programm selber kümmern sich hauptsächlich nur noch Markus Schröder und ich."</i></div>
**IU:** Aber dann gibt es natürlich Compiler, die sich ändern, die Hardware ändert sich.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Genau. Von der Seite gibt es immer mal wieder Bedarf. Aber das sind natürlich Kleinigkeiten. Es kommt ein neuer Compiler, und plötzlich funktioniert es nicht. Dann muss man den Befehl raussuchen, der den neuen zusätzlichen Check abschaltet. Und compiliert geht es wieder. Und solche Sachen, Kleinigkeiten passieren immer."</i></div>
**IU:** Wenn man jetzt an die Programmiersprache selber, also Fortran, denkt, ist es ja auch eine Programmiersprache, die sehr genutzt wurde, also besonders in der Chemie, in der theoretischen Physik auch, für diese Probleme. Aber heute nicht mehr so viel.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, Fortan ist, glaube ich, das Beste, was man benutzen kann für number crunching. Und natürlich, die modernere Sprache ist C++, die kann natürlich auch viel mehr, aber das viel mehr braucht man in der Regel nicht. Zumindest nicht, wenn man solche Dinge macht wie wir. C++ hat einen großen Vorteil. Viele Leute fangen jetzt an mit Python. Und man kann das natürlich auch mischen. Python ist wunderbar, es ist sehr einfach, es ist sehr mächtig, aber leider sehr langsam. Man könnte jetzt Programme schreiben, wo der ganze Input und alles Mögliche auf Python läuft und dann das number crunching ausgelagert wird an eine höhere Sprache. Und da eignet sich dann C++ besser, weil es die gleiche Datenstruktur wie Python hat. Und das wäre mit Fortran etwas komplizierter. Das ist etwas bedauerlich, dass die Python-Leute sich an C++ orientiert haben und nicht an Fortran. Insofern kann gut sein, dass die Zukunft stark darin liegt, dass man so eine Mischung von Python und C++ programmiert."</i></div>   
**IU:** Aber an sich hat Fortran ja in dem Bereich Quantendynamik oder Quantenmechanik sehr viel beigetragen.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, sehr viel beigetragen. Es gibt sehr viel in Fortran geschriebene Software. Und mit 90 und den höheren 2003 und was es jetzt gibt, ist Fortran auch sehr viel stärker geworden. Es ist sehr viel flexibler und kann viel mehr. Ich bin mit Fortran ganz glücklich. Aber das muss jeder selber entscheiden. Ich hänge vielleicht auch an der Tradition. Ich bin mit Fortran groß geworden. So ist es halt."</i></div>
**IU:** Gibt es Pläne in der nahen Zukunft, außer der Summer School, mit MCTDH?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Nein, wir werden weiter möglichst große Systeme studieren, so weit wir können. Wir haben hier in der Gruppe von Oriol Vendrell eine gewisse Tradition, protonierte Wassercluster zu untersuchen. Der letzte und größte Wassercluster den wir untersucht haben ist das Extended Zundel Kation, das ist ein Zundel mit noch vier Wassern drumherum. Das sind 51 Freiheitsgrade. Das ist schon ziemlich groß. Und in dieser Richtung werden wir sicher weitergehen. Wir berechnen die Absorptionsspektren der Cluster. Das ist die Anwendung. Und von der Programmentwicklung, da sehe ich im Moment nichts, was spektakulär ist, aber das kann natürlich kommen. Wenn wir auf ein Problem stoßen für das wir eine neue zusätzliche Entwicklung brauen, dann würde man die auch leisten, so weit es möglich ist. Man ist ja immer problem-driven. Man bekommt ein Problem, man setzt sich ja nicht hin und denkt sich etwas Großartiges aus, sondern die Probleme kommen und man versucht sie zu lösen."</i></div>
**IU:** Ja, dann bedanke ich mich bei dir.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, schönen Dank für das Gespräch, es war schön. Dankeschön. Und hoffentlich trägst es dazu bei, weitere MCTDH-User anzulocken."</i></div>
**IU:** Ja, bestimmt.

<!-- <script>
document.addEventListener('DOMContentLoaded', function() {
    const audioElements = document.querySelectorAll('audio');
    
    audioElements.forEach(function(audio) {
        audio.addEventListener('play', function() {
            // Pause all other audio elements when this one starts playing
            audioElements.forEach(function(otherAudio) {
                if (otherAudio !== audio) {
                    otherAudio.pause();
                }
            });
        });
    });
});
</script> -->

## Key Topics Covered

- Early experiences with programming in theoretical chemistry
- Development and open-source release of MCTDH
- Challenges in funding research software development
- The importance of documentation and community support
- Evolution of computational methods and hardware

## Full Interview Resources

### Complete Transcript
**[Read Full Interview Transcript](/interview-hans-dieter-meyer-de)**

### Audio Interview

**[🎧 Listen to Full Interview on Buzzsprout](https://www.buzzsprout.com/2531619/episodes/17727894)**

*Full audio interview (German) - conducted on May 8, 2025*

<iframe src="https://www.buzzsprout.com/2531619/episodes/17727894/player" width="100%" height="200" frameborder="0" scrolling="no"></iframe>

### Related Images

<div class="gallery">
  <div class="gallery-item">
    <img src="/01-Dieter-Meyer/dieter.jpg" alt="Professor Hans-Dieter Meyer" title="Professor Hans-Dieter Meyer">
    <div class="gallery-item">
    <img src="/01-Dieter-Meyer/MCTDH.png" alt="MCTDH stats" title="MCTDH package tech stats">
  </div>
  </div>
</div>

*Images from Professor Meyer's career and the MCTDH project.*

**Autoren von MCTHD**: Michael Beck, Andreas Jäckle, Graham Worth, Hans-Dieter Meyer  
**Contributors zu MCTHD**: Marie-Catherine Heitz, Stephan Wefing, Uwe Manthe, Suren Sukiasyan, Andreas Raab, Masahiro Ehara, Christoph Cattarius, Fabien Gatti, Frank Otto, Mathias Nest, Michael R. Brill, Oriol Vendrell, Markus Schröder, Daniel Pelaez-Ruiz, Phillip S. Thomas, Ying-Chih Chiang, Keyvan Sadri, David Mendive-Tapia

### Related links
[MCTDH]: http://mctdh.uni-hd.de/ "The Heidelberg MCTDH program package"
[MCTDH-refs]: http://mctdh.uni-hd.de/ "References for the Heidelberg MCTDH program package"
[MCTDH-book]: https://www.wiley-vch.de/de/fachgebiete/naturwissenschaften/multidimensional-quantum-dynamics-978-3-527-32018-9 "H.-D. Meyer, F. Gatti, and G. A. Worth, Eds., Multidimensional Quantum Dynamics: MCTDH Theory and Applications, Wiley-VCH, Weinheim, 2009, ISBN  978-3-527-32018-9"
[MCTDH-summer-school]: https://www.mctdh-school.uni-heidelberg.de/ "MCTDH Summer School"
[HDQD-conferences]: https://qdn.cnrs.fr/?page_id=44 "High-dimensional Quantum Dynamics Conferences"
[Quantics]: https://www2.chem.ucl.ac.uk/worthgrp/quantics/doc/index.html "The Quantics program package"
[MCTDH-highlight]: https://doi.org/10.1002/cphc.201600662 "The Importance of Vibronic Coupling for Efficient Reverse Intersystem Crossing in Thermally Activated Delayed Fluorescence Molecules"
---

*This interview is part of the RSE Pioneers project, documenting the contributions of early research software engineers who laid the foundation for modern computational research.*

**Interview Details:**
- **Date:** May 8, 2025
- **Duration:** 60 minutes
- **Language:** German
- **Location:** Heidelberg
