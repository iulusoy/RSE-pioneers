---
layout: single
title: Soundbytes from interviews with RSE pioneers
permalink: /soundbytes/
---
<style>
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

## Key moments in the interviews with RSE pioneers

RSE pioneers are the early adopters of research software in the research process, that fundamentally aided the community by providing access to research software. By providing this access and the developed research software as an infrastructure, RSE pioneers fundamentally advanced not only their own scientific pursuits, but also enabled a multitude of indirect research achievements by other researchers using the developed tools.

## What is Research Software Engineering?

Research Software Engineering (RSE) is a relatively new field that combines domain research with software development skills. Research software engineers develop, maintain, and extend the software that underpins research across all disciplines. In some disciplines, research software engineering has existed longer than in others - the pioneers in this series.

## The pioneers

Our featured pioneers are researchers who:
- Developed fundamental algorithms and methods
- Created impactful research software packages used by many other researchers in their field
- Made the decisions to provide open source access to their research software
- Built communities around their software
- Influenced how research software is developed and maintained today

## Soundbytes: Hans-Dieter Meyer

### About Open Source Development

<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Nur dadurch, dass wir das Open Source gemacht haben und den anderen zugänglich gemacht haben und das Programm auch so geschrieben haben, dass es für Leute, die nicht so ganz tief drin sind, wirklich nutzbar ist, hat MCTDH die Verbreitung erfahren.</i> 
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte1_open_source.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<br>

<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Man sollte die Programme freigeben, damit sie nutzbar sind."</i> 
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte2_open_source2.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

### About RSE practices

<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Es ist ja so, dass man immer größere Systeme lösen kann. Das liegt natürlich daran, dass die Computer immer leistungsfähiger werden. Das ist enorm, was in den letzten 20 Jahren passiert ist. Aber es liegt auch an den Algorithmen. Die Algorithmen sind sehr viel besser geworden. Man muss an beiden arbeiten, man kann nicht einfach da sitzen und warten, dass die nächste Computergeneration groß genug ist, um die Probleme zu lösen. Man muss die Algorithmen entsprechend entwickeln und erfinden, und da sind enorme Beiträge geleistet worden. MCTDH hat da selber einen großen Beitrag geleistet.</i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte3_algorithms.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>
<br>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i> Wenn man das öffentlich machen will, muss man auch eine gute Dokumentation schreiben. Und das ist lästig, das macht keinem so richtig viel Spaß. Programmieren macht oft Spaß, aber Dokumentation schreiben etwas weniger. Aber das ist unglaublich wichtig. 
</i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte4_documentation.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

## Scientific breakthroughs with MCTDH

<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Das Pyrazin konnten wir 1999 lösen. Das ist lange her. Und wir hatten gedacht, das ist so ein großer Durchbruch. Aber es hat relativ wenig Resonanz ergeben, denn wir waren einfach zu weit vorne. Die anderen Leute machten zwei oder drei Freiheitsgrade, und wir machten 24. Das haben die nicht so ganz richtig verstanden, gedacht das ist sowas ganz Spezielles. Von den Autoren ist niemand eingeladen worden, mal zu einem Vortrag darüber, in den folgenden zwei Jahren oder so. Später ist unsere Arbeit sehr anerkannt worden. Pyrazin ist ein Standardmodell geworden, um andere Methoden zu testen. Viele semi-klassische Methoden versuchen Pyrazin zu lösen, ja, das hat sich stark geändert. Aber das ist mir immer noch sehr in Erinnerung, als wir Pyrazin gelöst haben, hatten wir gedacht haben, jetzt kriegen wir großen Applaus. Nichts. Die Anerkennung kam mit Verzögerung. </i>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte5_breakthrough.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
</div>

### Research Software Communities

<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i> Auch wenn einem durch das MCTDH-Projekt die Programmierung abgenommen worden ist, die intellektuelle Leistung, sich mit dem wissenschaftlichen Problem und seiner numerischen Umsetzung zu beschäftigen, die kann einem niemand abnehmen. Die muss man dann bringen."</i></div>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte6_understanding.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>

### Outlook

<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Wenn wir auf ein Problem stoßen für das wir eine neue zusätzliche Entwicklung brauchen, dann würde man die auch leisten, so weit es möglich ist. Man ist ja immer problem-driven. Man bekommt ein Problem, man setzt sich ja nicht hin und denkt sich etwas Großartiges aus, sondern die Probleme kommen und man versucht sie zu lösen."</i></div>
<audio controls style="width: 100%; margin: 0.5rem 0 0 0;">
  <source src="{{ '/assets/audio/soundbyte7_motivation.mp3' | relative_url }}" type="audio/wav">
  Your browser does not support the audio element.
</audio>
---


