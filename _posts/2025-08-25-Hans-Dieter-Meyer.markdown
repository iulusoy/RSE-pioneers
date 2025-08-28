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
  <source src="/01-Dieter-Meyer/part1_open_source.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

Nach Erreichen eines höheren Reifegrades der Software war die Freigabe der Software an die Öffentlichkeit ein großer Meilenstein:
<audio controls style="width: 100%; margin: 0.5rem 0 1rem 0;">
  <source src="/01-Dieter-Meyer/soundbyte1_open_source.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<div style="padding: 1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>"Damals hatten wir auch noch nicht daran gedacht, das Programm öffentlich zu machen. Das kam erst später. Ich weiß gar nicht mehr genau wann, aber das muss auch Ende der 90er oder Anfang 2000 gewesen sein. Wir haben dann diskutiert, ob wir den MCTDH Code öffentlich machen sollen. Das war eine längere Diskussion, das war auch eine schwierige Entscheidung. [...] Aber es war natürlich die einzig richtige Entscheidung.</i>
<div style="padding: 1rem; margin: 1rem -1rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Nur dadurch, dass wir das Open Source gemacht haben und den anderen zugänglich gemacht haben und das Programm auch so geschrieben haben, dass es für Leute, die nicht so ganz tief drin sind, wirklich nutzbar ist, hat MCTDH die Verbreitung erfahren.</i> 
</div>
<i>Sonst wäre es ein kleines Ding nebenher gewesen. Es ist zu kompliziert. Man kann nicht einen Doktoranden sagen, mach das mal, das funktioniert nicht. Man muss einen längeren Atem haben. Den hat man nur, wenn man sich damit verbunden fühlt."</i>
</div>

**Frage:** Es ist oft das Sentiment unter den Forschenden, ich habe das geschrieben, das ist meins, ich möchte das nicht öffentlich machen, weil dann nutzen das andere und klauen mir die Ergebnisse. Was würdest du jemandem sagen, oder, was hat euch dazu bewogen, das dann doch freizugeben?
<audio controls style="width: 100%; margin: 0.5rem 0 1rem 0;">
  <source src="/01-Dieter-Meyer/soundbyte2_open_source2.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

<div style="padding: 1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>"Diese Bedenken hatten wir vielleicht auch, aber das ist altes Denken. Man sollte die Programme freigeben, damit sie nutzbar sind. Es macht ja keinen Sinn, dass jeder das Rad immer neu erfindet und ähnliche Programme schreibt. Das wird deutlich, wenn man an solche Bibliotheken wie LAPACK denkt. LAPACK ist wirklich eine wunderbare Sache. Sehr stark benutzt. Das haben Leute geschrieben, die haben sich die Mühe gemacht und werden jetzt acknowledged und ziert, aber wenn man das nicht freigegeben hätte, so dass nur die eigene Universität diese schönen Programme nutzen kann, das hätte ja nicht so viel Sinn gegeben. Ich glaube, da renne ich inzwischen offene Türen ein. Das war zu der Zeit, als wir uns in den 90er-Jahren entschieden haben, anders. Aber jetzt renne ich da offene Türen ein. Ich glaube, die Leute sehen ein, man sollte die Sachen öffentlich machen."</i> 
</div>

## RSE Praktiken


*Du hast jetzt die Programmierung und Softwareentwicklung über die Jahre natürlich verfolgt, und wenn du an verschiedene Phasen zurückdenkst, wie siehst du die Wichtigkeit von Programmierung und Softwareentwicklung, zum Beispiel während deiner Doktorarbeit, später als ihr MCTDH releast habt und jetzt in der Forschung?*   
Das hängt ein bisschen davon ab, wo und wie man forscht. Aber für uns war das natürlich immer essentiell. Theoretische Chemie ist immer sehr programmierlastig. Die Dinge, die man analytisch lösen kann, das haben die Generationen vor uns gelöst. Wir sind sehr darauf angewiesen, das numerisch zu machen. Entweder muss man dann die Programme selber schreiben, das haben wir dann getan. Oder, und dazu haben wir auch beigetragen, man benutzt fertige Programme. Das ist in der Quantenchemie natürlich noch viel mehr verbreitet als in der Dynamik. Aber in der Dynamik gibt es jetzt auch viele Programme, SHARC zum Beispiel für Surface Hopping und MCTDH und andere Pakete. Wir fördern damit einen Trend, den ich gar nicht so gerne mag, nämlich dass junge Doktoranden sagen, ich nehme einfach die fertigen Pakete und rechne damit und mache schöne Ergebnisse und kann ein Paper schreiben, aber habe mir nie die Finger schmutzig gemacht mit Programmieren. Das ist die andere Seite, wenn man das öffentlich macht, aber das ist halt so. Unser Arbeitsgebiet ist sehr computerlastig. Man muss mit Computern umgehen können, man sollte programmieren können und Programme weiterentwickeln. Es ist ja so, dass man immer größere Systeme lösen kann. Das liegt natürlich daran, dass die Computer immer leistungsfähiger werden. Das ist enorm, was in den letzten 20 Jahren passiert ist. Auf was für kleinen Maschinen wir damals gerechnet haben. Aber es liegt auch an den Algorithmen. Die Algorithmen sind sehr viel besser geworden. Man muss an beiden arbeiten. Man kann nicht einfach da sitzen und warten, dass die nächste Computergeneration groß genug ist, um die Probleme zu lösen. Man muss die Algorithmen entsprechend entwickeln und erfinden, und da sind ja enorme Beiträge geleistet worden. MCTDH hat da selber einen großen Beitrag geleistet. Dass wir jetzt die Dynamik von Molekülen mit 50 Freiheitsgraden oder so quantenmechanisch berechnen können, das wäre vor 20 Jahren schwer vorstellbar gewesen. [^1] Das sieht man auch daran, dass gewisse Formate im Output erweitert werden mussten. Als das Programm geschrieben wurde, konnten wir uns nicht vorstellen, dass wir über 100 Freiheitsgrade haben werden. Es wurden nur zwei Digits ausgedruckt. Wir hatten vielleicht 5 Freiheitsgrade, später mal 12 oder so, aber dass wir über 100 gehen, das war jenseits unseres Vorstellungsvermögens. Wir mussten die Formate ändern, damit da nicht Sterne ausgedruckt werden. Und solche Sachen, daran sieht man wie groß der Fortschritt ist, wir konnten es uns einfach nicht vorstellen.   
*Diese zwei Drehschrauben, also einmal algorithmisch, sieht man ja bei MCTDH wie bei dem Schritt zu ML-MCTDH. Aber dann auch in der Nutzung der Hardware.*   
Parallelisierung zum Beispiel.   
*Mit der Hardware haben sich vielleicht auch die wichtigsten Fähigkeiten geändert, die man braucht zum Programmieren, oder wie siehst du das.*  
Ich habe ja noch Programmieren im alten Stiel gelernt, und das habe ich mir schwer abgewöhnen müssen, z.B. das man nicht zu viel Memory verbraucht, dass man arrays, nachdem die gebraucht wurden, wieder verwendet. Das ist natürlich auch sehr fehlerträchtig. Das sollte man vermeiden. Heute ist Memory überhaupt kein Problem mehr. Das ist meistens massig vorhanden. Der ganze Stil des Programmierens hat sich natürlich geändert. Man programmiert heute ein bisschen anders als es früher war. Wir machen nicht unbedingt Objektprogrammierung. Aber in der Richtung ist vieles anders. Die Programmierspanne von Fortran 90 ist etwas anders als Fortran 77, da hat sich viel geändert. Das ist natürlich auch ein Problem für MCTDH. Es ist ja relativ alt. Es gibt noch sehr viele Code, der in Fortran 77 geschrieben ist. Das ist auch nicht änderbar. Niemand will das. Das ist eine zu große Masse. Das bleibt dann. Da muss man sehen, dass man das gut vereint und das alles gut laufen kann.   
*Es tritt vielleicht auch Lesbarkeit mehr in den Vordergrund, weil mehr wiederverwendet wird.*   
Ja, genau. Mehr Kommentare reinschreiben.   
*Ihr habt ja für MCTDH dann auch Versionskontrolle und Tests genutzt und Dokumentation geschrieben, zum Beispiel. Wie seid ihr darauf gekommen?*   
Zunächst haben wir natürlich sozusagen wild vor uns her programmiert. Wir haben dann ‘99 die erste Versionskontrolle eingeführt. Das war PRCS, ich weiss nicht ob das jemand kennt. Dann wurde uns das aber zu umständlich und zu alt und wir haben dann 2010 Subversion eingeführt. Inzwischen nehmen viele Leute Git. Aber ich bin mit Subversion, mit SVN, ganz zufrieden und das kann eigentlich alles, was ich brauche. Das war natürlich auch ein wichtiger Schritt, dass man das jetzt mal zurückverfolgen konnte was wann geändert worden ist. Vor allem, weil mehrere Leute damals programmiert haben. Eine Versionskontrolle ist unglaublich hilfreich, weil man wieder zurückgehen kann und sehen kann, was da gemacht worden ist, wo der Fehler eingebaut worden ist, falls es einen gab.   
*Und die Tests?*   
Wir haben eine Testroutine geschrieben. Ich glaube, es gibt so 50 Inputs. Die werden dann abgearbeitet. Aber es ist eigentlich zu wenig. Mit den Inputvariablen kann man MCTDH unheimlich fein steuern. Es ist halt ein sehr generelles Programm zur Lösung der Schrödinger Gleichung unterscheidbarer Teilchen. Man kann unheimlich viele verschiedene Dinge damit machen. Insofern gibt es immer wieder Probleme, weil Leute etwas ausprobiert haben, woran wir nie gedacht haben. Und dann in Schwierigkeiten geraten. Insofern lerne ich viel von den Nutzern. Die schreiben mir dann eine Email, und dann sehe ich ein, da müssen wir was ändern, da sollten wir was ändern. Das ist sehr schön. Ganz zu Beginn hatte ich mal gehofft, dass die Leute einen Beitrag leisten, vielleicht irgendwie eine Auswertroutine schreiben. Aber das ist eigentlich nie passiert. Sie kommen immer nur mit Complaints wie “es funktioniert nicht gut genug” oder “da müsste man etwas machen” und dann müssen wir halt was machen. Das andere Forscher etwas zum MCTDH code beitragen, die Hoffnung hat sich leider kaum ergeben.   
*Darauf werde ich nochmal zurückkommen. MCTDH lässt sich aber auch sehr einfach kompilieren auf allen möglichen Hardwares.*   
Ja, das läuft auf einem Laptop bis hin zu Supercomputern.   
*Habt ihr eine Strategie verfolgt, dass ihr es überall ausgetestet habt, oder ist das mit der Zeit gewachsen?*   
Das ist mit der Zeit gewachsen. Linux ist eine wunderbare Sache. Linux läuft auf allen Rechnern. Gott sei Dank läuft es auch auf Apple Computern. Es ist zwar nicht Linux, aber ein Unix-System. Da muss man ein bisschen anpassen. Wenn man einen Apple Laptop hat, läuft MCTDH da auch. Wenn man einen Windows-Rechner hat, sollte man Linux installieren wenn man MCTDH nutzen möchte. Und auf den Hochleistungs-Rechnern läuft in der Regel  immer Linux. Insofern war da eigentlich wenig zu tun. Wir testen immer alles mit den GNU-Compilern. 

*Ihr habt MCTDH nutzbar gemacht und unter Versionskontrolle gestellt, usw. Ihr habt praktisch beste Praxis angewandt, obwohl es den Begriff an sich noch nicht gab. Hast du das nach außen hin mal diskutiert? Oder war das überhaupt ein Thema mit anderen Forschenden oder auch in der Gruppe? Dass andere gesagt haben, warum macht ihr das? Oder wir wollen das nicht machen?*   
Zu Beginn haben wir das lange diskutiert, bevor wir es gemacht haben. Aber danach war die Entscheidung ja da. Ich kann das auch nur anderen wieder empfehlen, dies zu tun. Das ist die einzige Möglichkeit, dass das die Arbeit nicht irgendwie untergeht. Es gibt unheimlich viel Software, die irgendwann mal geschrieben und dann vergessen wird. Man möchte die vielleicht gerne nutzen, aber dann ist der Doktorand, der sie geschrieben hat, nicht mehr da. Das ist vielleicht ein Punkt, den ich auch mal hervorheben will. Wenn man das öffentlich machen will, muss man auch eine gute Dokumentation schreiben. Und das ist lästig, das macht keinem so richtig viel Spaß. Programmieren macht oft Spaß, aber Dokumentation schreiben etwas weniger. Aber das ist unglaublich wichtig. Gerade wenn es dann so komplex wird wie MCTDH. Ich gucke selber in die Dokumentation, weil ich vergessen habe, wie genau lautet das keyword, um diese oder jene Funktion einzuschalten. Eine gute Dokumentation ist ganz essentiell. Ich glaube, dass viel Software nicht nutzbar ist, liegt daran, dass sie nicht ausreichend gut dokumentiert ist.   
*Und mit der Dokumentation, wer hat angefangen, die zu schreiben?*   
Inzwischen gibt es viele Tools, die wir aber gar nicht benutzt haben, weil es die Tools noch gar nicht gab. Wir schreiben das alles in HTML. Und dann haben wir noch andere Dinge geschrieben. Ein User’s Guide gibt es noch, der ist in LaTeX geschrieben. Und es gibt auch noch eine sogenannte Lab Session. Das ist ein Tutorial, mit dem man verschiedene Inputs ausprobieren kann und dann lernen kann, MCTDH zu benutzen. Aber das sind mehr so Handreichungen, um MCTDH zu nutzen und es zu lernen. Die HTML-Dokumentation ist in der täglichen Arbeit sehr hilfreich, wenn man genau wissen will, wie muss der Input aussehen, wenn ich das und das machen möchte.   

[¹] Die Behandlung von Modellen wie Spin-Boson, vibronic-coupling Hamiltonian, generalized Henon-Heiles etc. ist sehr viel einfacher. Pyrazin mit seinen 24 Freiheitsgraden konnten wir schon 1999 lösen und heutzutage sind Modelle mit mehreren 100 Feiheitsgraden lösbar.



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


## Audio Highlights

**[🎧 Listen to Interview Highlights on Buzzsprout](https://www.buzzsprout.com/2531619/episodes/17727894)**

*Listen to key moments from our conversation with Professor Meyer.*

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
