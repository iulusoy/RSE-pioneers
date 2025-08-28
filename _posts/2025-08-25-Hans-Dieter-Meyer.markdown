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

<script>
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
</script>


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
