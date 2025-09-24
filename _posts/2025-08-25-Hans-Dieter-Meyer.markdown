---
title: "RSE pioneers - Pioniere des Forschungssoftware-Engineerings: Hans-Dieter Meyer"
excerpt: "Quantum dynamics researcher and developer of the Heidelberg MCTDH software package."
date: 2025-08-25
author: Inga Ulusoy
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
gallery:
  - url: https://www.pci.uni-heidelberg.de/tc/dieter.html
    image_path: /assets/images/dieter.jpg
    alt: "Professor Hans-Dieter Meyer"
    title: "Professor Hans-Dieter Meyer"
  - url: https://www.pci.uni-heidelberg.de/tc/mctdh.html
    image_path: /assets/images/MCTDH.png
    alt: "MCTDH Software Interface"
    title: "MCTDH Software Interface"
  - url: /assets/images/MCTDH-ship.jpg
    image_path: /assets/images/MCTDH-ship.jpg
    alt: "The MCTDH ship, steered by Dieter. Non-smokers clearly achieve better scientific results than do people who smoke. While Oriol is on the lookout, Frank Otto is busy programming."
    title: "The MCTDH ship, steered by Dieter. Non-smokers clearly achieve better scientific results than do people who smoke. While Oriol is on the lookout, Frank Otto is busy programming."
  - url: https://www.pci.uni-heidelberg.de/tc/index.html
    image_path: /assets/images/uni-hd-logo.png
    alt: "Theoretical Chemistry group at Heidelberg University"
    title: "Theoretical Chemistry Lab at Heidelberg"
toc: true
toc_label: "Interview Abschnitte"
toc_sticky: true
---

<style>
/* Reduce left sidebar margin */
.sidebar,
.toc {
  left: 0 !important;
  margin-left: 0 !important;
  padding-left: 0.5rem !important;
}

/* If you want the main content to move further left as well */
.page__container,
.page {
  padding-left: 1rem !important;
  max-width: 1600px !important;
}

/* On very large screens, keep sidebar close to the edge */
@media (min-width: 1200px) {
  .sidebar,
  .toc {
    left: 0 !important;
    margin-left: 0 !important;
    padding-left: 0.5rem !important;
  }
  .page__container,
  .page {
    max-width: 1800px !important;
    padding-left: 1rem !important;
  }
}

/* Prevent column layout switch at 1600px and above */
@media (min-width: 1600px) {
  .layout--single .page__container,
  .layout--single .page,
  .page__container,
  .page {
    max-width: 1400px !important;
    width: calc(100% - 300px) !important;
    margin-left: 280px !important;
    margin-right: auto !important;
    padding-left: 1rem !important;
    padding-right: 1rem !important;
  }
  
  /* Keep sidebar on the left - positioned to not block content */
  .sidebar {
    position: absolute !important;
    left: auto !important;
    top: auto !important;
    width: 250px !important;
    max-width: 250px !important;
    margin-left: 0 !important;
    padding-left: 0.5rem !important;
    z-index: 1 !important;
  }
  
  /* Keep TOC on the right side */
  .toc {
    position: sticky !important;
    top: 2rem !important;
    left: auto !important;
    right: 1rem !important;
    width: 200px !important;
    max-width: 200px !important;
    margin-left: auto !important;
    z-index: 5 !important;
  }
}
/* Custom styling for the Minimal Mistakes TOC */
.toc {
  background-color: #f8f9fa;
  border: 1px solid #dee2e6;
}

.toc .nav__title {
  color: #0d2476ff !important;
  background-color: transparent;
  font-weight: bold;
}

.toc .nav__list a {
  color: #333;
  transition: background-color 0.2s;
}

.toc .nav__list a:hover {
  background-color: #0d2476ff;
  color: white;
}

.toc .nav__list .active a {
  background-color: #0d2476ff;
  color: white;
}

/* Hide header link symbol for main title (h1) */
h1 .header-link {
  display: none !important;
}

/* Gallery styling for clickable images */
.gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin: 20px 0;
}

.gallery-item {
    flex: 1;
    min-width: 300px;
    text-align: center;
}

.gallery-item a {
    display: block;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    border-radius: 8px;
    overflow: hidden;
    text-decoration: none;
}

.gallery-item a:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(13, 36, 118, 0.3);
}

.gallery-item img {
    width: 100%;
    height: auto;
    display: block;
    transition: opacity 0.3s ease;
}

.gallery-item a:hover img {
    opacity: 0.9;
}

/* Add cursor pointer for clickable images */
.gallery-item a {
    cursor: pointer;
}

/* Audio section styling */
.audio-section {
    background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
    border: 2px solid #0d2476ff;
    border-radius: 12px;
    padding: 25px;
    margin: 25px 0;
    box-shadow: 0 4px 15px rgba(13, 36, 118, 0.15);
}

.audio-info h4 {
    color: #0d2476ff;
    margin-top: 0;
    margin-bottom: 15px;
    font-size: 1.2em;
}

.audio-info p {
    margin: 8px 0;
    color: #495057;
}

.audio-links {
    margin: 20px 0;
    text-align: center;
}

.audio-button {
    display: inline-block;
    background: #0d2476ff;
    color: white !important;
    padding: 12px 24px;
    text-decoration: none !important;
    border-radius: 8px;
    font-weight: bold;
    transition: all 0.3s ease;
    box-shadow: 0 2px 8px rgba(13, 36, 118, 0.3);
}

.audio-button:hover {
    background: #1a4bc7;
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(13, 36, 118, 0.4);
    color: white !important;
}

.audio-note {
    margin-top: 15px;
    padding-top: 15px;
    border-top: 1px solid #dee2e6;
}

.audio-note p {
    font-size: 0.9em;
    color: #6c757d;
    font-style: italic;
    margin: 0;
}
.mm-labels {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  margin-bottom: 1.5rem;
}
.mm-label {
  font-size: 0.95em;
  font-weight: 500;
}
.mm-category {
  background: #0d2476ff;
  color: #fff;
}
.mm-tag {
  background: #e9ecef;
  color: #0d2476ff;
}
</style>

<!-- Place this after the front matter and before your main content -->

{% if page.categories or page.tags %}
<div class="mm-labels" style="margin-bottom: 1.5rem;">
  {% if page.categories %}
    <span class="mm-label mm-category" style="background:#0d2476ff; color:#fff; border-radius:4px; padding:2px 8px; margin-right:8px;">
      {{ page.categories | join: ', ' }}
    </span>
  {% endif %}
  {% if page.tags %}
    {% for tag in page.tags %}
      <span class="mm-label mm-tag" style="background:#e9ecef; color:#0d2476ff; border-radius:4px; padding:2px 8px; margin-right:4px;">
        {{ tag }}
      </span>
    {% endfor %}
  {% endif %}
</div>
{% endif %}

  <div style="margin: 20px 0;">
    <a href="{{ site.baseurl }}/interview/2025/08/25/Hans-Dieter-Meyer-en.html" class="audio-button" style="display: inline-block; background: #0d2476ff; color: white !important; padding: 12px 24px; text-decoration: none !important; border-radius: 8px; font-weight: bold; transition: all 0.3s ease; box-shadow: 0 2px 8px rgba(13, 36, 118, 0.3);">
      🇬🇧 Read English Interview
    </a>
  </div>

Die computergestützte Forschung hat mittlerweile fast alle Fachbereiche ergriffen, und Forschende vor Herausforderungen in der Anwendung und der Entwicklung von Forschungssoftware gestellt. Mit der KI-Revolution steht bereits die nächste Welle an Umwälzungen bevor.
Einige Fachbereiche sind von der Digitalisierung des Forschungsprozesses weniger stark beeinflußt worden: Insbesondere die Fachbereiche, die bereits computergestützt geforscht haben. So zum Beispiel in der theoretischen Chemie: Hier haben Wissenschaftler "schon immer" Computerprogramme entwickelt und in der Forschung zum Einsatz gebracht, mit allem was dazu gehört - z.B. dem Erlernen von Programmiersprachen, Compilern und Profilern. So entstanden über die Jahre hinweg viele große Programmpackete wie [GAMESS](https://www.ameslab.gov/gamess-open-source-quantum-chemistry-software), [Gaussian](https://gaussian.com/), [Molpro](https://www.molpro.net/), und [andere](https://en.wikipedia.org/wiki/Category:Computational_chemistry_software) - fundamentale Bausteine für die Forschung, ohne die viele Erkenntnisse nicht möglich gewesen wären.

Wie haben diese ersten RSEs die Forschung vorangetrieben, welche Faktoren haben Erfolg und Verbreitung von Forschungssoftware beeinflusst? Was sind Unterschiede von heute zu damals? Mit diesen Fragen befasst sich RSE Pioneers.

## Zur Person

Hans-Dieter Meyer studierte Physik in Göttingen und schloss seine Doktorarbeit an der Universität Göttingen bei J.P. Toennies in 1978 zu dem Thema "Formation of dimers in rare gas beams from nozzles" ab. Im Anschluss ging er als DFG-geförderter Postdoc zur University of California, Berkeley, USA, wo er bei W. H. (Bill) Miller sich weiterhin mit der Simulation von Streuprozessen befasste. Nach dem Aufenthalt in Berkeley kehrte Dieter nach Göttingen zurück und schloss sich 1980 dem Lehrstuhl für Theoretische Chemie der Universität Heidelberg an (Gruppe von Lorenz Cederbaum). In 1991 habilitierte Dieter zum Thema "Stationäre und zeitabhängige Behandlung molekularer Streuprozesse” und war danach Hochschuldozent, Privatdozent, und ist seit 2005 Apl. Professor an der Universität Heidelberg.

Hans-Dieter Meyer ist der Hauptverantwortliche, Entwickler und langjähriger Maintainer der Open-Source Research Software “Heidelberg-MCTDH” (Multi-Configuration Time-Dependent Hartree). [MCTDH][MCTDH] ist ein hocheffizienter Algorithmus zur Lösung der zeitabhängigen Schrödingergleichung, und ist in Fortran geschrieben (verschiedene Fortran-Dialekte, hinzu kommen Teile in C und Python). Der Algorithmus ist in [mehreren Publikationen][mctdh-refs] und einem [Buch][MCTDH-book] beschrieben, und das Software-Paket, bestehend aus verschiedenen Programmen, wurde etwa 550-mal heruntergeladen. In der Quantendynamik-Community ist MCTDH berühmt für seine Effizienz und hohe Genauigkeit in der Lösung von Wellenpaket-Dynamik-Problemen. Die Publikationen, welche MCTDH vorgestellt haben, sind insgesamt über 5.000 Mal zitiert, die Heidelberg-MCTDH Homepage listet über 300 Publikationen welche MCTDH nutzen. MCTDH hat daher fundamental zur Forschung in der Quantendynamik beigetragen und Forschungsprojekte sowie Forscherkarrieren geprägt. Ohne die Entwicklung des Algorithmus, aber insbesondere des Software-Paketes, welches den Algorithmus zugänglich gemacht hat, sowie der Betreuung der Nutzer, wäre die Forschungslandschaft um einiges ärmer, und [viele Einsichten hätten nicht gewonnen werden können][MCTDH-highlight]. 

Hans-Dieter Meyer hat laut Google Scholar 358 Forschungsbeiträge veröffentlicht (ResearchGate: 316, Web of Science: 285), die 27.244-mal zitiert wurden (ResearchGate: 22.448, Web of Science: 19.739) (h-Index 75 (ResearchGate: h-Index 68, Web of Science: h-Index 64)).

## Die Anfänge
Hans-Dieter Meyer begann während seiner Doktorarbeit computergestützt zu forschen, damals noch auf Lochkarten und mit Hilfe kleiner Programme zur Datenauswertung, hauptsächlich in Fortran. Das Programmieren hat er sich selber beigebracht, "durchs Abgucken". Anfangs war das Programmieren und Debuggen von Programmen noch deutlich aufwändiger: Erst mit der Anschaffung der ersten Bildschirme und eigener Rechner in den Forschungsgruppen war es möglich, direkter zu Programmieren und Fehler sofort zu korrigieren. All dies war alltäglich und integraler Bestandteil der eigenen Forschung.

Anfang der 90er Jahre begann dann die Arbeit an MCTDH mit der Entwicklung der Methode und des Algorithmus. Diese bilden zwei Seiten des gleichen Inhaltes ab: Zum einen die mathematische Beschreibung, Näherung und Verifizierung des Ansatzes; zum anderen die numerische Repräsentation des Ansatzes. Durch die Implementation wird der Ansatz durch einen Vergleich mit exakt lösbaren Modellen und experimentellen Daten sowohl verifiziert als auch validiert. Nach der initialen Implementierung der Methode wurde das Programm erweitert und professionalisiert (Anheben des technologischen Reifegrads über den Prototyp hinaus).

## Öffentlichstellung der Software zur allgemeinen Nutzung

<div style="background-color: #f8f9fa; border: 1px solid #dee2e6; border-radius: 0.375rem; padding: 1rem; margin: 1rem 0; font-size: 0.9rem;">
<strong>🎧 Diesen Abschnitt als Audio hören:</strong>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/part1_open_source.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

Nach Erreichen eines höheren Reifegrades der Software war die Freigabe an die Öffentlichkeit ein großer Meilenstein:

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Zunächst hatten wir noch nicht daran gedacht, das Programm öffentlich zu machen. Das kam erst später, ich weiß gar nicht mehr genau wann, Ende der 90er oder Anfang 2000. Das war eine längere Diskussion, und auch eine schwierige Entscheidung. [...] Aber es war natürlich die einzig richtige Entscheidung.</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Nur dadurch, dass wir das Open Source gemacht haben und den anderen zugänglich gemacht haben und das Programm auch so geschrieben haben, dass es für Leute, die nicht so ganz tief drin sind, wirklich nutzbar ist, hat MCTDH die Verbreitung erfahren.</i> 
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte1_open_source.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i>Sonst wäre es ein kleines Ding nebenher gewesen. Es ist zu kompliziert. Man kann nicht einem Doktoranden sagen, mach das mal, das funktioniert nicht. Man muss einen längeren Atem haben. Den hat man nur, wenn man sich damit verbunden fühlt."</i>
</div>

**IU:** Es ist oft das Sentiment unter den Forschenden, "ich habe das geschrieben, das ist meins, ich möchte das nicht öffentlich machen, weil dann nutzen das andere und klauen mir die Ergebnisse". Was würdest du jemandem sagen, oder, was hat euch dazu bewogen, das dann doch freizugeben?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Diese Bedenken hatten wir vielleicht auch, aber das ist altes Denken. Man sollte die Programme freigeben, damit sie nutzbar sind. Es macht ja keinen Sinn, dass jeder das Rad immer neu erfindet und ähnliche Programme schreibt. Das wird deutlich, wenn man an solche Bibliotheken wie LAPACK denkt. Das haben Leute geschrieben, die haben sich die Mühe gemacht und werden jetzt acknowledged und zitiert, aber wenn man das nicht freigegeben hätte, so dass nur die eigene Universität diese schönen Programme nutzen kann, das hätte ja nicht so viel Sinn gegeben. Ich glaube, da renne ich inzwischen offene Türen ein. Das war zu der Zeit, als wir uns in den 90er-Jahren entschieden haben, anders. Ich glaube, die Leute sehen mittlerweile ein, man sollte die Sachen öffentlich machen."</i> 
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
<i>HDM: "Das hängt ein bisschen davon ab, wo und wie man forscht. Aber für uns war das natürlich immer essentiell. Theoretische Chemie ist immer sehr programmierlastig. Die Dinge, die man analytisch lösen kann, die haben die Generationen vor uns gelöst. Wir sind sehr darauf angewiesen, das numerisch zu machen. Entweder muss man dann die Programme selber schreiben, das haben wir dann getan. Oder, und dazu haben wir auch beigetragen, man benutzt fertige Programme. Das ist in der Quantenchemie natürlich noch viel mehr verbreitet als in der Dynamik. Wir fördern damit einen Trend, den ich gar nicht so gerne mag, nämlich dass junge Doktoranden sagen, ich nehme einfach die fertigen Pakete und rechne damit und mache schöne Ergebnisse und kann ein Paper schreiben, aber habe mir nie die Finger schmutzig gemacht mit Programmieren. Das ist die andere Seite, wenn man das öffentlich macht, aber das ist halt so. Unser Arbeitsgebiet ist sehr computerlastig. Man muss mit Computern umgehen können, man sollte programmieren können und Programme weiterentwickeln. </i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Es ist ja so, dass man immer größere Systeme lösen kann. Das liegt natürlich daran, dass die Computer immer leistungsfähiger werden. Das ist enorm, was in den letzten 20 Jahren passiert ist. Aber es liegt auch an den Algorithmen. Die Algorithmen sind sehr viel besser geworden. Man muss an beiden arbeiten, man kann nicht einfach da sitzen und warten, dass die nächste Computergeneration groß genug ist, um die Probleme zu lösen. Man muss die Algorithmen entsprechend entwickeln und erfinden, und da sind enorme Beiträge geleistet worden. MCTDH hat da selber einen großen Beitrag geleistet.</i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte3_algorithms.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i>Dass wir jetzt die Dynamik von Molekülen mit 50 Freiheitsgraden oder so quantenmechanisch berechnen können, das wäre vor 20 Jahren schwer vorstellbar gewesen.<sup>[1]</sup> Das sieht man auch daran, dass gewisse Formate im Output erweitert werden mussten. Als das Programm geschrieben wurde, konnten wir uns nicht vorstellen, dass wir über 100 Freiheitsgrade haben werden. Es wurden nur zwei Digits ausgedruckt. Wir hatten vielleicht 5 Freiheitsgrade, später mal 12 oder so, aber dass wir über 100 gehen, das war jenseits unseres Vorstellungsvermögens. Wir mussten die Formate ändern, damit da nicht Sterne ausgedruckt werden. Und solche Sachen, daran sieht man wie groß der Fortschritt ist."</i>
</div>

**IU:** Diese zwei Drehschrauben, algorithmisch und hardware, sieht man ja bei MCTDH wie bei dem Schritt zu ML-MCTDH. Aber dann auch in der Nutzung der Hardware.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Parallelisierung zum Beispiel."</i></div>

**IU:** Mit der Hardware haben sich vielleicht auch die wichtigsten Fähigkeiten geändert, die man braucht zum Programmieren, oder wie siehst du das?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich habe ja noch Programmieren im alten Stil gelernt, und das habe ich mir schwer abgewöhnen müssen, z.B. das man nicht zu viel Memory verbraucht, dass man arrays, nachdem die gebraucht wurden, wieder verwendet. Das ist natürlich auch sehr fehlerträchtig und das sollte man vermeiden. Heute ist Memory überhaupt kein Problem mehr. Der ganze Stil des Programmierens hat sich natürlich geändert. Die Programmierspanne von Fortran 90 ist etwas anders als Fortran 77, da hat sich viel geändert. Das ist natürlich auch ein Problem für MCTDH, es ist ja relativ alt. Es gibt noch sehr viele Code, der in Fortran 77 geschrieben ist. Das ist auch nicht änderbar. Das ist eine zu große Masse, das bleibt dann. Da muss man sehen, dass man das gut vereint und das alles gut laufen kann."</i>
</div>
**IU:** Es tritt vielleicht auch Lesbarkeit mehr in den Vordergrund, weil mehr Routinen wiederverwendet werden.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, genau. Mehr Kommentare reinschreiben."</i></div>
**IU:** Ihr habt ja für MCTDH dann auch Versionskontrolle und Tests genutzt und Dokumentation geschrieben, zum Beispiel. Wie seid ihr darauf gekommen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Zunächst haben wir natürlich sozusagen wild vor uns her programmiert. Wir haben dann ‘99 die erste Versionskontrolle eingeführt. Das war PRCS, ich weiss nicht ob das jemand kennt. Dann wurde uns das aber zu umständlich und zu alt und wir haben dann 2010 Subversion eingeführt. Inzwischen nehmen viele Leute Git. Aber ich bin mit Subversion, mit SVN, ganz zufrieden und das kann eigentlich alles, was ich brauche. Das war natürlich auch ein wichtiger Schritt, dass man das jetzt mal zurückverfolgen konnte was wann geändert worden ist. Vor allem, weil mehrere Leute damals programmiert haben."</i></div>
**IU:** Und die Tests?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Wir haben eine Testroutine geschrieben. Ich glaube, es gibt so 50 Inputs, die werden dann abgearbeitet. Aber es ist eigentlich zu wenig. Mit den Inputvariablen kann man MCTDH unheimlich fein steuern. Es ist halt ein sehr generelles Programm zur Lösung der Schrödingergleichung unterscheidbarer Teilchen. Man kann unheimlich viele verschiedene Dinge damit machen. Insofern gibt es immer wieder Probleme, weil Leute etwas ausprobiert haben, woran wir nie gedacht haben und dann in Schwierigkeiten geraten. Insofern lerne ich viel von den Nutzern. Die schreiben mir dann eine Email, und dann sehe ich ein, da müssen wir was ändern, da sollten wir was ändern. Das ist sehr schön. Ganz zu Beginn hatte ich mal gehofft, dass die Leute einen Beitrag leisten, vielleicht irgendwie eine Auswertroutine schreiben. Aber das ist eigentlich nie passiert."</i></div>
**IU:** Darauf werde ich nochmal zurückkommen. MCTDH lässt sich aber auch sehr einfach kompilieren auf aller möglicher Hardware.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, das läuft auf einem Laptop bis hin zu Supercomputern."</i></div>
**IU:** Habt ihr eine Strategie verfolgt, dass ihr es überall ausgetestet habt, oder ist das mit der Zeit gewachsen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Das ist mit der Zeit gewachsen. Linux ist eine wunderbare Sache. Linux läuft auf allen Rechnern. Gott sei Dank läuft es auch auf Apple Computern. Es ist zwar nicht Linux, aber ein Unix-System. Da muss man ein bisschen anpassen. Wenn man einen Apple Laptop hat, läuft MCTDH da auch. Wenn man einen Windows-Rechner hat, sollte man Linux installieren wenn man MCTDH nutzen möchte. Und auf den Hochleistungs-Rechnern läuft in der Regel immer Linux. Insofern war da eigentlich wenig zu tun. Wir testen immer alles mit den GNU-Compilern."</i></div>
**IU:** Ihr habt MCTDH nutzbar gemacht und unter Versionskontrolle gestellt, usw., also ihr habt beste Praxis angewandt, obwohl es den Begriff an sich noch nicht gab. Hast du das nach außen hin mal diskutiert? Oder war das überhaupt ein Thema mit anderen Forschenden oder auch in der Gruppe? Dass andere gesagt haben, warum macht ihr das? Oder wir wollen das nicht machen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Zu Beginn haben wir das lange diskutiert, bevor wir es gemacht haben. Aber danach war die Entscheidung ja da. Ich kann das auch nur anderen wieder empfehlen, dies zu tun. Das ist die einzige Möglichkeit, dass die Arbeit nicht irgendwie untergeht. Es gibt unheimlich viel Software, die irgendwann mal geschrieben und dann vergessen wird. Man möchte die vielleicht gerne nutzen, aber dann ist der Doktorand, der sie geschrieben hat, nicht mehr da. Das ist vielleicht ein Punkt, den ich auch mal hervorheben will.</i>
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
<i>HDM: "Ich hatte Glück, dass Graham Worth relativ früh, das war ‘94, zu meiner Arbeitsgruppe hinzu kam. Er hatte viel Erfahrung mit Programmieren, wir haben eigentlich viel von ihm profitiert. Er hat das Ganze ein bisschen mehr professionalisiert. Er war dann hier Postdoc bis Ende 2000. Dem bin ich zu Dank verpflichtet. Und dann Frank Otto, der war ein Doktorand, der hat ja schon auf Ataris oder so als Schüler rumprogrammiert. Der hat uns auch bei einigen Dingen geholfen. Wenn man Mitarbeiter hat, die mehr können als man selbst, ist das sehr schön. Und sonst vom Programmieren so herausragend, da ist Haobin Wang zu nennen, der ML (Multilayer) entwickelt hat. Nicht bei uns, in den Vereinigten Staaten. Ich war 2001 dort zu einer Geburtstagsfeier von Bill Miller. Dort habe ich Haobin Wang kennengelernt. Und der hatte angefangen, Multilayer MCTDH zu entwickeln. Wir haben das dann viel diskutiert, weil wir ähnliche Ideen hatten. Wir hatten das Cascading genannt. Aber wir haben da nie wirklich was gemacht. Das erschien uns einfach zu komplex. Und wir sagten, wenn wir uns da jetzt ransetzen und das programmieren, und das funktioniert nicht, dann machen wir uns sehr viel Arbeit für nichts. Aber Haobin Wang hat das einfach gemacht. Und das hat wunderbar funktioniert. Und dann haben wir das alle nachgemacht. Insofern ist er mein Hero."</i></div>
**IU:** Und ein Wendepunkt, das kam ja jetzt schon ein paar Mal hoch, war die Öffentlichmachung von MCTDH. Aber gab es noch irgendwelche anderen Punkte, an denen ihr die Richtung geändert habt?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Eigentlich nicht so sehr. ML, das ist Multilayer MCTDH, ist für größere Systeme ein wichtiger Schritt nach vorne. Das Heidelberger ML hat im wesentlichen Oriol Vendrell programmiert. Und wir hatten auch keinen großen Plan. Die Probleme kamen auf uns und zu und wir haben sie dann versucht zu lösen. Wir haben versucht, es immer weiter besser zu machen. [...] Was in den letzten Jahren eine starke, wichtige  Entwicklung war, war das Umschreiben vom allgemeinen Potentialprogramm in die sogenannte Sum-of-Products-Form. [...] Man kann das Potential in eine kompaktere Form bringen, in die sogenannte CPD-Form auch bekannt unter den Namen CANDECOMP oder Parallel Factors. Da hat Markus Schröder einen riesigen Beitrag geleistet, denn jetzt haben wir ein Programm, MCCPD, Monte Carlo CPD, was allgemeine Potentialflächen ins sum-of-products Format bringt. Die Quantenchemiker stellen der wissenschaftlichen Gemeinschaft Programme zur Verfügung, da gibt man Koordinaten vor und sie returnen die potentielle (Born-Oppenheimer) Energie. Das heißt, sie haben einen Potential-Fit generiert, aber das ist ein allgemeiner Fit und diesen refitten wir auf diese Sum-of-Products Form. Das Letzte, was wir in Zusammenarbeit mit Fabien Gatti und anderen gemacht haben, war Wasserstoff auf einer Graphitfläche und da haben wir mehrere Graphitatome mitgenommen, die sich dann bewegen können und die Energie transferieren können. Und das war ein ganz großer Schritt, denn dies führte zu 75 Freiheitsgraden. Und dann die Fläche mit 75 Freiheitsgraden zu refitten, das hätten wir vor ein paar Jahren noch für nicht denkbar gehalten. [...]
Ein anderer wichtiger Punkt, wiederum nicht direkt MCTDH aber für MCTDH sehr wichtig, ist die Herleitung des Operators der kinetischen Energie. Wenn man so kleine Systeme wie Wasser oder HONO oder so behandelt, da kann man die kinetische Energie per Hand herleiten und programmieren. Aber wenn die Systeme größer werden wird es schwierig. Wir wollen ja nicht so etwas wie Normalkoordinaten nehmen, dann ist alles simpel, sondern es ist sehr, sehr wichtig, dass die Koordinaten den natürlichen Bewegungen folgen oder die natürlichen Bewegungen gut beschreiben. [...] Und dann wird die kinetische Energie unfassbar kompliziert. Glücklicherweise ist dann in Zusammenarbeit mit David Lauvergnat und Fabien Gatti ein Programm entstanden, das heißt Tana, und das berechnet diese kinetische Energie analytisch und schreibt sie dann in einem Format, das man direkt in MCTDH einlesen kann. Ohne das hätten wir auch die großen Systeme nicht mehr machen können. Wir haben damals, 2007, das Spektrum des protonierten Wasser-Dimers, also des Zundel-Kations, berechnet. Das war ein großer Durchbruch. Im Zundel-Kation hält ein Proton zwei Wassermoleküle zusammen. Es gibt Bewegungen großer Amplitude in einem sehr anharmonischen Potential. Damals haben wir noch mit Fabien Gatti zusammen, also er hat das gemacht, die kinetische Energie sozusagen per Hand erstellt, mit Überprüfung durch numerische Verfahren (Tnum). Der kinetische Operator ist in einer sum-of-products Form mit etwa 150 Termen dargestellt. Das war eine lange Arbeit, aber es war möglich. Aber für Moleküle, die wir kürzlich berechnet haben, wie das Eigenkation (33D), das wäre gar nicht mehr möglich gewesen. Für den refit des Potentials (mit MCCPD) haben wir 2048 Terme in der sum-of-products Form benutzt, die Darstellung der kinetischen Energie benötigte fast 2500 Terme. Das kann man nicht mehr per Hand machen. Das sind also so Dinge, die parallel zu MCTDH laufen, aber für MCTDH absolut essentiell sind. Diese Entwicklungen sind in den letzten Jahren entstanden und haben uns natürlich sehr geholfen. Damit können wir diese großen Systeme berechnen. [...]"</i></div>
**IU:** Das zeigt ja auch beispielhaft, wie man sich nicht darauf verlassen kann, dass Computer besser werden und man einfach größere Systeme rechnet. Das Problem ändert sich, die Darstellung ändert sich und die muss abgebildet werden.
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
**IU:** Wenn du jetzt daran denkst, das ist ja eine Entwicklung von Forschungssoftware in der Forschungslandschaft und du hast ja erwähnt, du hast Doktoranden gehabt, die daran gearbeitet haben und so weiter. Wo siehst du kritische Punkte in der Entwicklung von Forschungssoftware im universitären Umfeld?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ein kritischer Punkt ist die Finanzierung. Die DFG finanziert sowas nicht [Anmerkung: Mittlerweile hat sich bei der DFG ein Schritt in die Richtung der Förderung von Forschungssoftware-Entwicklung getan.], sondern sie finanziert nur wissenschaftliche Forschung und wenn man dazu vielleicht ein bisschen Programmierentwicklung machen will, dann kann man das ja machen, aber man kann nicht in einen Antrag schreiben, ein Programm zu entwickeln oder so."</i><small>[Anmerkung: Ein DFG Antrag von Dieter wurde aus diesem Grund abgelehnt].</small> <i>"Das funktioniert nicht. Und das ist anders in England. Graham Worth hat Gelder bekommen, extra für Programmentwicklung. Er hat dann einen Fork gemacht vom Heidelberger MCTDH, nennt es QUANTICS und da hat er speziell Geld dafür bekommen, das zu entwickeln. So etwas fehlt in Deutschland. Das war für mich immer ein Krampf. Man musste immer ein wissenschaftliches Projekt haben und man wollte aber eigentlich Programmentwicklung machen. Wir wollten natürlich auch Anwendungen machen. Wir machen ja die Entwicklung nicht nur so ins Blaue hinein, sondern um Anwendungen durchführen zu können. Aber um es in einem DFG-Antrag durchzukriegen, muss man es umgekehrt schreiben. Man muss es so schreiben, dass die Anwendung im Vordergrund steht und die Entwicklung, die läuft dann so nebenher. Aber dazu ist Softwareentwicklung zu wichtig. Und ich hoffe, dass sich da mal ein bisschen was ändert."</i></div> 
**IU:** Und dann habt ihr praktisch neue Fragestellungen bearbeitet und dabei auch ein bisschen Programmwartung übernommen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, natürlich. Zu Beginn haben wir angefangen mit H+H<sub>2</sub>-Streuung und solche Sachen. Und das haben wir in den Vordergrund gestellt und dafür auch schöne Papers geschrieben. Im Laufe dieser Arbeiten wurde MCTDH entwickelt. Aber die Anträge liefen natürlich immer über das Projekt, das untersucht worden ist."</i></div> 
**IU:** Und abgesehen davon, dass man ja auch Geld braucht, um die Leute zu finanzieren, dass sie die Software entwickeln, ist es ja auch so, dass daraus nicht direkt immer ein Paper entsteht. Wie siehst du das, wie kann man diese Beiträge würdigen oder ist das in der Vergangenheit gewürdigt worden, wenn Doktoranden Beiträge geleistet haben?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Wie gesagt, das Geld gibt es nur für die Forschung, die dann rausgekommen ist, dass da noch irgendwas berechnet worden ist, ein Wirkungsquerschnitt oder ein Spektrum oder so weiter. Und die eigentliche Programmentwicklung, die wird so nicht gewürdigt. Ich meine, ich würdige sie natürlich, aber vom Geldgeber her nicht so sehr. Und das ist der Punkt, den ich kritisiere, dass man da mehr flexibel sein muss."</i></div>
**IU:** Das hat ja vielleicht auch Einfluss auf die Karriere der Doktoranden, wenn die halt die Zeit investieren, dann wird das nicht angerechnet.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich hatte mal einen Postdoc, der kam und sagte, er möchte eigentlich nicht so gerne Programmentwicklung machen, er brauche ja Papers für seine Karriere. Das habe ich eingesehen, dann haben wir mit ihm schöne Sachen gemacht. Das ist dann so. Also solche Argumente kommen schon und das habe ich in dem Sinne auch unterstützt. Bei Doktoranden ist es einfacher. Ein Doktorand, der muss eine Doktorarbeit schreiben, aber der denkt vielleicht noch nicht so sehr an seine Karriere in dem Moment."</i></div>
**IU:** MCTDH hat ja einige Publikationen, die dann auch zitiert werden sollen, wenn man das Programm nutzt. Denkst du, das ist ein guter Weg, um diese Beiträge zu würdigen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich sehe keinen anderen. Es war ja auch ein langer Weg. Inzwischen ist es sehr bekannt und alle Leute sagen, das ist eine sehr gute Methode und kennen es und highlighten es. Aber zu Beginn war das schwierig. Es war den Leuten doch sehr fremd. Und ich weiß, unser erster wirklich großer Durchbruch war Pyrazin. [...]</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Das Pyrazin konnten wir 1999 lösen. Das ist lange her. Und wir hatten gedacht, das ist so ein großer Durchbruch. Aber es hat relativ wenig Resonanz ergeben, denn wir waren einfach zu weit vorne. Die anderen Leute machten zwei oder drei Freiheitsgrade, und wir machten 24. Das haben die nicht so ganz richtig verstanden, gedacht das ist sowas ganz Spezielles. Von den Autoren ist niemand eingeladen worden, mal zu einem Vortrag darüber, in den folgenden zwei Jahren oder so. Später ist unsere Arbeit sehr anerkannt worden. Pyrazin ist ein Standardmodell geworden, um andere Methoden zu testen. Viele semi-klassische Methoden versuchen Pyrazin zu lösen, ja, das hat sich stark geändert. Aber das ist mir immer noch sehr in Erinnerung, als wir Pyrazin gelöst haben, hatten wir gedacht haben, jetzt kriegen wir großen Applaus. Nichts. Die Anerkennung kam mit Verzögerung. </i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte5_breakthrough.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<i> Ein anderer großer Durchbruch war das Zundel-Kation, weil das wirklich ein echtes Molekül ist, nicht ein Modell. Mit 15 Freiheitsgraden, das war auch zu dem Zeitpunkt weit besser, mehr als andere Leute konnten. Wir konnten das wirklich vollständig analysieren und lösen. Da haben wir auch viel Anerkennung bekommen. Inzwischen ist das alles natürlich kein Problem mehr. Aber im Beginn schon."</i></div>

<div style="display: flex; align-items: center; margin: 1rem 0;">
<img src="{{ '/assets/images/zundel_molden.png' | relative_url }}" alt="Das Zundel-Kation." style="width: 50%; height: auto; margin-right: 1rem;">
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
**IU:** MCTDH wird ja auch durch viele Forschende genutzt, die dann ihre Forschung wieder auf der Verfügbarkeit und Nutzbarkeit von MCTDH basieren. Siehst du da kritische Punkte? Eine Nutzer-Community zu haben in der Forschungslandschaft? 
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Nein, es ist eigentlich sehr schön. Es ist klar, dass Leute das MCTDH-Programm runterladen und nutzen. Und sich dann vielleicht wieder anderen Problemen zuwenden, das ist der Lauf der Dinge. Sie machen das nicht unbedingt ihr ganzes Forscherleben wie ich es in den letzten Jahren gemacht habe, sondern sie haben ein bestimmtes Problem, wenden da MCTDH an. Dann machen sie vielleicht was anderes. Manche bleiben dabei, benutzen MCTDH kontinuierlich für fast alle ihre Sachen. Das ist unterschiedlich. Ich kriege auch manchmal eine E-Mail von irgendeinem Studenten vielleicht aus China oder so, der MCTDH haben will. Da habe ich dann schon große Bedenken, dass das was wird. Wenn jemand das alleine machen will, das ist zu komplex, wenn man kein Umfeld hat. Wenn sozusagen der Professor sagt, mach das mal. Dann muss es schon ein sehr, sehr guter Student sein, dass er es schafft. Dann höre ich auch nie wieder was davon. Man muss schon ein Umfeld haben, wenn jemand aus dem Quantenchemie-Umfeld kommt und sagt, jetzt machen wir mal Dynamik. Das ist eine andere Denkweise, die Zeitabhängigkeit. Ich stelle immer wieder fest, dass das den Leuten schwer fällt. Es gibt Leute, die denken sehr in Eigenzuständen und jetzt sollen sie in Wellenpaketen denken. Wenn man so ein Einzelkämpfer ist, ist das schwer. Man braucht schon eine gewisse Umgebung und eine Unterstützung, dann kann das gut gehen. Wir machen auch eine MCTDH-Summer-School. Und, letztes Mal hat einer der Schüler Kritik geäußert, MCTDH ist zu kompliziert. Das ist nicht wahr, die Quantendynamik ist kompliziert. MCTDH versucht es so einfach zu machen wie möglich. Aber Quantendynamik ist kompliziert. Da muss man sich reinhängen. </i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i> Auch wenn einem durch das MCTDH-Projekt die Programmierung abgenommen worden ist, die intellektuelle Leistung, sich damit zu beschäftigen, die kann einem niemand abnehmen. Die muss man dann bringen."</i></div>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte6_understanding.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** Also die Nutzer müssen schon auch verstehen, was da passiert, worauf sie es anwenden können und dafür reicht dann eine einfache Dokumentation nicht aus. Man muss auch in die Methode einsteigen, in die Paper. Aber dann gibt es vielleicht in der Anwendung wieder Fragen, z.B. "wie schreibe ich jetzt das Operator-File?". Da bekommt ihr sicherlich viele Nutzer-Anfragen.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich kriege manchmal einen Input und raufe mir dann die Haare. Aber im Großen und Ganzen ist es gar nicht so kompliziert, auch das Operator-File. Wir haben ein extra ASCII-File, in das man reinschreibt, wie der Operator aussieht, wie der Hamiltonian auszusehen hat. Das kann man über diese Sum-of-Products Struktur ziemlich gut definieren. Es gibt eine ganze Library von Operatoren, die man dann einbinden kann. Erste Ableitung, zweite Ableitung, irgendwelche Funktionen usw. Das kann man, glaube ich, ganz gut lernen. Wenn man das Input-File schreibt, muss man eine gewisse Vorstellung haben z.B. wie eine Basis funktioniert. Manchmal funktioniert was nicht, weil z.B. die Gitterpunkte viel zu grob gewählt sind. Dann kann gar nichts funktionieren. Dann ist es nicht ein Fehler von MCTDH, sondern es ist wirklich ein Inputfehler. Ich kriege manchmal Anfragen und einen Input file, Dann versuche ich zu helfen."</i></div>
**IU:** Das kostet dich ja auch wieder Zeit.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Das kostet mich wieder Zeit, aber ich bin ja pensioniert und habe die Zeit."</i></div>
**IU:** Von daher können sich diese Nutzer dann auch wirklich glücklich schätzen. Weil es schwierig ist, die Zeit zu finden und Support zu leisten. Im Prinzip kann man das auch über Forschungsprojekte gar nicht finanzieren.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Genau. Das ist wieder dieser Punkt, den wir schon besprochen haben. Dass da die DFG vielleicht mal ein bisschen die Politik ändert."</i></div>
**IU:** Natürlich ist die Methode viel verbreitet und angewandt worden. Du hast ja auch schon angesprochen, dass die Nutzer zwar keinen Code zurück beigetragen haben, aber dadurch, dass sie Fehler gefunden haben, sie durchaus zur Entwicklung beigetragen haben.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich habe viel gelernt von den Nutzern. Einerseits, weil sie auf Fehler aufmerksam gemacht haben oder Fragen gestellt haben, die klargemacht haben, dass der Input oder die Dokumentation ein bisschen missverständlich war. Dass man das so verstehen kann, wie der Nutzer das verstanden hat, aber ich das gar nicht so gemeint habe. Und dass man dann  ins Programm noch irgendwelche Fehlermeldungen einbaut. Man macht einen Input, der unsinnig ist und dann soll MCTDH das vielleicht entdecken und sagen, das ist eine nicht erlaubte Kombination von Dingen. Ich habe dann oft eine Fehlermeldung eingebaut, die das Programm stoppt und auf den fehlerhaften Input hinweist. Insofern lerne ich immer viel von den Nutzern."</i></div>
**IU:** Und du hast ja auch angesprochen, ihr habt ja auch schon eine Summer School gemacht und plant jetzt wieder eine. Wie ist die Idee entstanden, die Summer School zu machen?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ich glaube, die kam von Oriol. Und das haben wir dann vor zwei Jahren gemacht, das war sehr schön. Und wir machen sie dieses Jahr wieder, Ende Juli, es kommen so etwa 50 Leute. Die erste Summer School war ein bisschen breiter, da haben wir auch Leute von MCTDHB und MCTDHF dazu genommen. Also MCTDH ist ein Programm zur Lösung der Schrödinger-Gleichung für unterscheidbare Teilchen und kann somit die Molekulardynamik lösen. Aber dann gibt es natürlich auch identische Teilchen, also Fermionen wie Elektronen, oder Bosonen. Die Bosonenforschung ist ja ein Schwerpunkt in der Physik, also ultrakalte Physik usw. Und da haben Leute Programme geschrieben, die diese Symmetrien einbauen. In der letzten Summer School gab es  eine Session, MCTDHB und MCTDHF, aber die haben wir jetzt rausgenommen. Wir wollen uns mehr auf das eigentliche MCTDH konzentrieren. Gleicherweise hatten wir damals noch einen Vortrag über Tensor Trains und DMRG und solche Sachen, die mit MCTDH verwandt ist. Auch das nehmen wir jetzt raus. Diese Summer School ist mehr auf die Anwendung von MCTDH konzentriert."</i></div>
**IU**: Und ihr habt aber auch eine Konferenzserie.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, wir haben die High Dimensional Quantum Dynamics Serie, HDQD, die findet im Prinzip alle zwei Jahre statt. Die Thematik der Konferenz ist natürlich nicht allein auf MCTDH ausgerichtet, sondern eben auf High Dimensional Quantum Dynamics. Aber MCTDH hatte natürlich immer eine sehr starke Bedeutung, eine sehr starke Betonung. Zu Beginn hatte ich diese Konferenz-Reihe organisiert. Inzwischen mache ich das nicht mehr, inzwischen macht das ein Committee. Zu Beginn war ich das alleine, ich habe immer versucht jemanden zu finden, der die HDQD ausrichtet. Und es war zu Beginn schwierig. Später hat sich das geändert, dann kamen die Leute zu mir und wollten eine HDQD ausrichten. Und inzwischen ist es relativ etabliert, und es gibt ein Committee, das jetzt entscheidet, wer die Konferenz ausrichtet. Die vorletzte HDQD war in Groningen, die habe ich noch zugeteilt. Und die allerletzte war in Hamburg, 2024. Und die nächste wird, glaube ich, in Spanien sein. Also in 2026 wird es dann wieder eine HDQD geben, alle zwei Jahre."</i></div>
**IU:** Und wie viele Teilnehmer habt ihr da im Moment?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "So 150 vielleicht. Wir haben klein angefangen, mit etwa 50 Teilnehmern. Die erste Konferenz war 2005 in Leiden mit Geert-Jan Kroes im sogenannten Lorentz-Center. Das heißt, die eigentliche Organisation ist dort gemacht worden, ich hatte nur mit der wissenschaftlichen Organisation zu tun, Auswahl der Speakers, Aufstellung des Programms usw. Das habe ich natürlich gerne gemacht. Und dann haben Geert-Jan Kroes und ich die HDQD ins Leben gerufen. Und das war ein großer Erfolg, es war eine Konferenz, die war mehr aufs Technische fokussiert. Was sind die Methoden, um High Dimensional Quantum Dynamics zu lösen? Vom Stil eine andere Konferenz. Und die Leute waren so begeistert, dass sie gesagt haben, das machen wir wieder. Und dann habe ich versucht, das alle zwei Jahre zu organisieren, was mir nicht immer gelungen ist. Sie fiel dann mal aus, und so waren es mal drei Jahre zur nächsten HDQD, und wegen Covid auch einmal vier. Aber ich habe immer jemanden gefunden, der eine HDQD organisiert, und zwar in Montpellier, Birmingham,  Mittelwihr, Rostock, Lille und Groningen. Jetzt ist es mehr organisiert, der Stil hat sich auch geändert, ein bisschen zu meinem Bedauern. Es war so eine Konferenz on the point, mehr von und für Leute, die Programme entwickeln. Und jetzt ist es doch mehr eine allgemeine Konferenz, sie unterscheidet sich nicht mehr so stark von anderen Konferenzen. So ist der Lauf der Dinge. Jetzt steuern wir mehr auf die 150, 200 oder so Teilnehmer zu. Aber der Schwerpunkt High Dimensional Quantum Dynamics ist geblieben."</i></div>
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
<i>HDM: "Um das Programm selber kümmern sich hauptsächlich nur noch Markus Schröder und ich."</i></div>
**IU:** Aber dann gibt es natürlich Compiler, die sich ändern, die Hardware ändert sich.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Genau. Von der Seite gibt es immer mal wieder Bedarf. Aber das sind natürlich Kleinigkeiten. Es kommt ein neuer Compiler, und plötzlich funktioniert es nicht. Dann muss man den Befehl raussuchen, der den neuen zusätzlichen Check abschaltet. Und dann kompiliert es wieder. Und solche Sachen, Kleinigkeiten passieren immer."</i></div>
**IU:** Wenn man jetzt an die Programmiersprache selber, also Fortran, denkt, ist es ja auch eine Programmiersprache, die sehr viel genutzt wurde, also besonders in der Chemie, in der theoretischen Physik auch, für diese Probleme. Aber heute nicht mehr so viel.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Fortan ist, glaube ich, die beste Sprache für number crunching. Und natürlich, die modernere Sprache ist C++, die kann natürlich auch viel mehr, aber das viel mehr braucht man in der Regel nicht. Zumindest nicht, wenn man solche Dinge macht wie wir. C++ hat einen großen Vorteil. Viele Leute fangen jetzt an mit Python. Und man kann das natürlich auch mischen. Python ist wunderbar, es ist sehr einfach, es ist sehr mächtig, aber leider sehr langsam. Man könnte jetzt Programme schreiben, wo der ganze Input und alles Mögliche auf Python läuft und dann das number crunching ausgelagert wird an eine höhere Sprache. Und da eignet sich dann C++ besser, weil es die gleiche Datenstruktur wie Python hat. Und das wäre mit Fortran etwas komplizierter. Das ist etwas bedauerlich, dass die Python-Leute sich an C++ orientiert haben und nicht an Fortran. Insofern kann gut sein, dass die Zukunft stark darin liegt, dass man so eine Mischung von Python und C++ programmiert."</i></div>   
**IU:** Aber an sich hat Fortran ja in dem Bereich Quantendynamik oder Quantenmechanik sehr viel beigetragen.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Ja, sehr viel beigetragen. Es gibt sehr viel in Fortran geschriebene Software. Und mit 90 und den höheren 2003 und was es jetzt gibt, ist Fortran auch sehr viel stärker geworden. Es ist sehr viel flexibler und kann viel mehr. Ich bin mit Fortran ganz glücklich. Aber das muss jeder selber entscheiden. Ich hänge vielleicht auch an der Tradition. Ich bin mit Fortran groß geworden. So ist es halt."</i></div>
**IU:** Gibt es Pläne in der nahen Zukunft, außer der Summer School, mit MCTDH?
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Nein, wir werden weiter möglichst große Systeme studieren, so weit wir können. Wir haben hier in der Gruppe von Oriol Vendrell eine gewisse Tradition, protonierte Wassercluster zu untersuchen. Der letzte und größte Wassercluster den wir untersucht haben ist das Extended Zundel Kation, das ist ein Zundel mit noch vier Wassern drumherum. Das sind 51 Freiheitsgrade. Das ist schon ziemlich groß. Und in dieser Richtung werden wir sicher weitergehen. Wir berechnen die Absorptionsspektren der Cluster. Das ist die Anwendung. Und von der Programmentwicklung, da sehe ich im Moment nichts, was spektakulär ist, aber das kann natürlich kommen. </i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Wenn wir auf ein Problem stoßen für das wir eine neue zusätzliche Entwicklung brauchen, dann würde man die auch leisten, so weit es möglich ist. Man ist ja immer problem-driven. Man bekommt ein Problem, man setzt sich ja nicht hin und denkt sich etwas Großartiges aus, sondern die Probleme kommen und man versucht sie zu lösen."</i></div>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte7_motivation.wav' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
**IU:** Ja, dann bedanke ich mich bei dir.
<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Schönen Dank für das Gespräch, es war schön. Dankeschön. Und hoffentlich trägst es dazu bei, weitere MCTDH-User anzulocken."</i></div>
**IU:** Ja, bestimmt.

<script>
// Enhance heading anchor links
document.addEventListener('DOMContentLoaded', function() {
    // Add anchor links to all headings
    const headings = document.querySelectorAll('h1, h2, h3, h4, h5, h6');
    
    headings.forEach(function(heading) {
        // Create anchor link if heading has an id
        if (heading.id) {
            const link = document.createElement('a');
            link.className = 'header-link';
            link.href = '#' + heading.id;
            link.innerHTML = '🔗';
            link.title = 'Link to this section';
            heading.appendChild(link);
        }
    });
    
    // Audio controls - pause other audio when one starts playing
    const audioElements = document.querySelectorAll('audio');
    
    audioElements.forEach(function(audio) {
        audio.addEventListener('play', function() {
            audioElements.forEach(function(otherAudio) {
                if (otherAudio !== audio) {
                    otherAudio.pause();
                }
            });
        });
    });
    
    // Smooth scrolling for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function (e) {
            e.preventDefault();
            const target = document.querySelector(this.getAttribute('href'));
            if (target) {
                target.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
            }
        });
    });
});
</script>

## Key Topics Covered

- Early experiences with programming in theoretical chemistry
- Development and open-source release of MCTDH
- Challenges in funding research software development
- The importance of documentation and community support
- Evolution of computational methods and hardware

## Full Interview Resources

### Complete Transcript
**[Read Full Interview Transcript](/interview-hd-meyer-full/)**

### Audio Interview

<div class="audio-section">
  <div class="audio-info">
    <h4>🎧 Full Interview Available</h4>
    <p><strong>Language:</strong> German</p>
    <p><strong>Date:</strong> May 8, 2025</p>
    <p><strong>Duration:</strong> Complete interview with Prof. Hans-Dieter Meyer</p>
  </div>
  
  <div class="audio-links">
    <a href="https://shows.acast.com/rse-pioneers/episodes/68d0ff2f146cfd1a6552805e" target="_blank" rel="noopener noreferrer" class="audio-button">
      🎧 Listen on Acast
    </a>
  </div>
  
  <div class="audio-note">
    <p><em>Note: The audio player opens in a new window due to platform restrictions. Click the link above to access the full interview.</em></p>
  </div>
</div>

### Related Images

{% include gallery caption="*Images from Professor Meyer's career and the MCTDH project.*" %}

**Autoren von MCTHD**: Michael Beck, Andreas Jäckle, Graham Worth, Hans-Dieter Meyer  
**Contributors zu MCTHD**: Marie-Catherine Heitz, Stephan Wefing, Uwe Manthe, Suren Sukiasyan, Andreas Raab, Masahiro Ehara, Christoph Cattarius, Fabien Gatti, Frank Otto, Mathias Nest, Michael R. Brill, Oriol Vendrell, Markus Schröder, Daniel Pelaez-Ruiz, Phillip S. Thomas, Ying-Chih Chiang, Keyvan Sadri, David Mendive-Tapia

### Related links
Es finden regelmäßig [Workshops und Lehrveranstaltungen zu MCTDH][MCTDH-summer-school] statt. Darüberhinaus entstand die ["High-Dimensional Quantum Dynamics" Konferenzreihe][HDQD-conferences], und es gibt weitere (variierte) Implementierungen des MCTDH Algorithmus in anderen Programmen (Uwe Manthe (Bielefeld), Graham Worth (University College London, [“Quantics”][Quantics]), Haobin Wang (Denver)). 

- [**MCTDH**: "The Heidelberg MCTDH program package" - http://mctdh.uni-hd.de/][MCTDH]
- [**MCTDH references**: "References for the Heidelberg MCTDH program package" http://mctdh.uni-hd.de/][MCTDH-refs]
- [**MCTDH book**: "H.-D. Meyer, F. Gatti, and G. A. Worth, Eds., Multidimensional Quantum Dynamics: MCTDH Theory and Applications, Wiley-VCH, Weinheim, 2009, ISBN  978-3-527-32018-9" - https://www.wiley-vch.de/de/fachgebiete/naturwissenschaften/multidimensional-quantum-dynamics-978-3-527-32018-9][MCTDH-book]
- [**MCTDH Summer School**: "MCTDH Summer School" - https://www.mctdh-school.uni-heidelberg.de/][MCTDH-summer-school]
- [**HDQD conferences**: "High-dimensional Quantum Dynamics Conferences" https://qdn.cnrs.fr/?page_id=44][HDQD-conferences]
- [**Quantics**: "The Quantics program package" - https://www2.chem.ucl.ac.uk/worthgrp/quantics/doc/index.html][Quantics]

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
