---
title: "RSE pioneers: Hans-Dieter Meyer"
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
toc_label: "Interview Sections"
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
    <a href="{{ site.baseurl }}/interview/2025/08/25/Hans-Dieter-Meyer.html" class="audio-button" style="display: inline-block; background: #0d2476ff; color: white !important; padding: 12px 24px; text-decoration: none !important; border-radius: 8px; font-weight: bold; transition: all 0.3s ease; box-shadow: 0 2px 8px rgba(13, 36, 118, 0.3);">
      🇩🇪 Read German Interview (original language)
    </a>
  </div>

Computer-assisted research has now reached almost all disciplines, challenging researchers in the application and development of research software. With the AI revolution, the next wave of upheaval is already on the horizon.

Some disciplines, however, have been little changed by the digitization of the research process in the past 20 years: particularly those that already have conducted computer-assisted research. Theoretical chemistry is one such example: here, scientists have "always" developed computer programs and used them in research, with everything that entails - learning programming languages, and how to use compilers and profilers. Over the years, this has led to the creation of several large software packages like [GAMESS](https://www.ameslab.gov/gamess-open-source-quantum-chemistry-software), [Gaussian](https://gaussian.com/), [Molpro](https://www.molpro.net/), and [others](https://en.wikipedia.org/wiki/Category:Computational_chemistry_software) - fundamental building blocks for research and research infrastructures, without which many insights would not have been possible.

How did these first RSEs advance research, what factors influenced the success and adaptation of research software? What are the differences between today and back then? RSE Pioneers addresses these questions.

## About the person

Hans-Dieter Meyer studied physics in Göttingen and completed his doctoral thesis at the University of Göttingen under J.P. Toennies in 1978 on the topic of “Formation of dimers in rare gas beams from nozzles.” He then went to the University of California, Berkeley, USA, as a DFG-funded postdoc, where he continued to work on the simulation of scattering processes under W. H. (Bill) Miller. After his stay in Berkeley, Dieter first returned to Göttingen and then joined the Chair of Theoretical Chemistry at the University of Heidelberg (Lorenz Cederbaum's group) in 1980. In 1991, Dieter habilitated on the topic of “Stationary and time-dependent treatment of molecular scattering processes” and has been an adjunct professor at the University of Heidelberg since 2005.

Hans-Dieter Meyer is the main developer and long-time maintainer of the open-source research software “Heidelberg-MCTDH” (Multi-Configuration Time-Dependent Hartree). [MCTDH][MCTDH] is a highly efficient algorithm for solving the time-dependent Schrödinger equation and is written in Fortran (various Fortran dialects, with parts in C and Python). The algorithm is described in [several publications][mctdh-refs] and a [book][MCTDH-book], and the software package, consisting of various programs, has been downloaded about 550 times. In the quantum dynamics community, MCTDH is famous for its efficiency and high accuracy in solving wave packet dynamics problems. The publications that introduced MCTDH have been cited over 5,000 times in total, and the Heidelberg MCTDH homepage lists over 300 publications that use MCTDH. MCTDH has therefore made a fundamental contribution to research in quantum dynamics and has shaped research projects and research careers. Without the development of the algorithm, but especially the software package that made the algorithm accessible, as well as the support provided to users, the research landscape would be much poorer, and [many insights would not have been gained][MCTDH-highlight]. 

According to Google Scholar, Hans-Dieter Meyer has published 358 research articles (ResearchGate: 316, Web of Science: 285), which have been cited 27,244 times (ResearchGate: 22,448, Web of Science: 19,739) (h-index 75 (ResearchGate: h-index 68, Web of Science: h-index 64)).

## The beginnings
Hans-Dieter Meyer began conducting computer-assisted research during his doctoral studies, at that time still using punch cards and writing small programs for data analysis, mainly in Fortran. Dieter learned programming mainly by himself and through observation. In the beginning, programming and debugging code was much more time-consuming: It was only with the purchase of the first monitors and computers for the research groups that it became possible to develop software more directly and correct errors immediately. All of this was part of everyday life and an integral part of the research itself.

The work on MCTDH began in the early 1990s with the development of the method and the algorithm. These represent two sides of the same coin: on the one hand, the mathematical description, approximation, and verification of the approach; on the other hand, the numerical representation of the approach. Through implementation, the approach is both verified and validated by comparison with exactly solvable models and experimental data. After the initial implementation of the method, the MCTDH software was expanded and professionalized (raising the technological maturity level beyond the prototype).

## Release of the software for general use

Once the software had reached a higher level of maturity, its release to the public was a major milestone:

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "At first, we hadn't thought about making the software public. That came later, I don't remember exactly when, in the late 90s or early 2000s. It was a long discussion and also a difficult decision. [...] But of course it was the only right decision.</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>It was only because we made MCTDH open source and accessible to others, and wrote the software in such a way that it is really usable for people who are not so deeply involved, that MCTDH has become so widespread.</i> 
</div>
<i>Otherwise, it would have been a minor side project. It's too complicated. You can't just tell a doctoral student to write such kind of software; that doesn't work. The development of such a research software requires perserverance, stamina and personal investment over longer stretches of time."</i>
</div>

**IU:** Researchers often feel, 'I wrote this, it's mine, I don't want to make it public because then others will use it and steal my results.' What would you say to someone making such a statement?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "We may have had those concerns too, but that's old thinking. Software programs should be released so that they can be used. It makes no sense for everyone to keep reinventing the wheel and writing similar software. This becomes clear when you think of libraries such as LAPACK. These were written by people who put in a lot of effort and are now acknowledged and cited, but if these libraries hadn't been released so that only their own university could use these wonderful routines, it wouldn't have made much sense. I think I'm preaching to the choir here. That was different back in the 1990s when we made our decision. I think people now realize that such types of research software should be made public."</i> 
</div>

## RSE Practices

**IU:** You've been following programming and software development over the years, and if you look back at different phases, how do you see the importance of programming and software development, for example, during your Ph.D., later when you released MCTDH, and now in research?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "It depends a bit on where and how you research. But for us, it was always essential. Theoretical chemistry is always very programming-intensive. The things that can be analytically solved have been solved by previous generations. We are very dependent on solving problems numerically. Either you have to write the code yourself, which we did, or you use existing software. This is much more common in quantum chemistry than in dynamics. We are promoting a trend that I don't like very much, where young Ph.D. students say, 'I'll just use the existing packages and obtain nice results and write a paper, but I've never gotten my hands dirty with programming.' This is the other side of making the software public, but that's just the way it is. Our field is very computer-intensive. You have to be able to work with computers, you should be able to program, and you should be able to develop software.</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Compared to the earlier days, now you can solve larger systems. This is due to the fact that computers are becoming more powerful. But it's also due to the algorithms that have become much better. You have to work on both, you can't just sit there and wait for the next generation of computers to be large enough to solve the problems. You have to develop and invent the algorithms, and enormous contributions have been made in that respect. MCTDH has made a big contribution in this regard.</i>
</div>
<i>That we can now calculate the dynamics of molecules with 50 degrees of freedom or so quantum-mechanically, this would have been hard to imagine 20 years ago. This can be seen in the fact that certain output formats had to be expanded. When MCTDH was written, we couldn't imagine that we would treat over 100 degrees of freedom. We only printed two digits. We had maybe five degrees of freedom, later twelve or so, but that we would include over 100, this was beyond our imagination. We had to change the output format so that it wouldn't print stars. From things like this you can see how much progress has been made."</i>
</div>

**IU:** These two knobs, algorithmically and hardware-wise, can be seen in MCTDH, just like in the step to ML-MCTDH (multilayer MCTDH). But also in the use of hardware.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Parallelization, for example."</i></div>

**IU:** Have the most important skills needed for programming also changed with the hardware?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "I still learned programming in the old style, where memory was expensive and we were reusing arrays after they were used. This is very error-prone and should be avoided. Nowadays, memory is not a problem at all. The style of programming has changed completely. The programming span of Fortran 90 is different from Fortran 77, there have been many changes. This is also a problem for MCTDH, it's relatively old. There is still a lot of code written in Fortran 77. This is not possible to change, these parts will remain. You have to see that you can combine it and encapsulate it well."</i>
</div>
**IU:** Maybe readability also becomes more important because more routines are reused.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Yes, exactly. More comments written in."</i></div>
**IU:** You've also used version control and testing, and written documentation, for example. How did you start with that?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "At first, we just programmed "wild-west style". We then introduced the first version control in '99 with PRCS. Which later became too cumbersome and too old, and we introduced Subversion in 2010. Nowadays, many people use Git. But I'm happy with Subversion, with SVN, it can do everything I need. This was a very important step, that we could now track what was changed when. Especially because several people were working on the code at the time."</i></div>
**IU:** And the tests?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "We wrote a test routine. I think there are about 50 inputs that are processed. But it's actually too little. You have very fine control over MCTDH with the input variables. It's a very general program for solving the Schrödinger equation for distinguishable particles. You can do many different things with it. Therefore, there are always problems because people try out things that we never thought of and then get into trouble. Therefore, I learn a lot from the users. They send me an email, and then I see, we need to change this, we should change that. This is very nice. At the beginning, I had hoped that the users would contribute, maybe write some evaluation routine. But this has never happened."</i></div>
**IU:** And MCTDH is very easy to compile on different machines.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Yes, it's very easy to compile MCTDH on any possible hardware."</i></div>
**IU:** Did you employ a strategy to test the compilation everywhere, or did that develop over time?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "This developed over time. Linux is a wonderful thing. Linux runs on all computers. Thank goodness it also runs on Apple computers. It's not Linux, but a Unix system. You have to make some adjustments. If you have an Apple laptop, MCTDH also runs on it. If you have a Windows computer, you should install Linux if you want to use MCTDH. And high-performance computers usually run Linux. Therefore, there was actually little to do. We always test everything with the GNU compilers."</i></div>
**IU:** You've made MCTDH usable and put it under version control, etc., so you've applied software engineering best practices in the research context, although the term didn't exist yet. Have you ever discussed this publicly? Was this ever a topic with other researchers or even within the group? 

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "We discussed it a lot at the beginning, before we did it. But after that, the decision was made. I can only recommend this to others. This is the only way that the work doesn't get lost. There is too much software that was written and then forgotten. You might want to use it, but the Ph.D. student who wrote it is no longer there. There is a point that I also want to emphasize:</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>If you want to make it public, you also have to write a good documentation. Programming is often fun, but writing documentation is less fun. But this is incredibly important.</i>
</div>
<i>Especially when it becomes as complex as MCTDH. I look at the documentation myself because I've forgotten how the keyword is spelled to enable or disable a certain function. Good documentation is absolutely essential. I believe that much software is not usable because it is not well enough documented."</i></div>
**IU:** And how did you start writing the documentation?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "We write it all in HTML. And then we have developed further documentation, there is a User's Guide that is written in LaTeX. And there is also a so-called Lab Session. This is a tutorial where you can try out different inputs and then learn to use MCTDH. But this is more of a guide to using and learning MCTDH. The HTML documentation is very helpful in daily work when you want to know exactly how the input should look like if you want to do something."</i></div>

## Scientific Breakthroughs through MCTDH

**IU:** Are there people who have influenced you in the development of research software? Were there any specific moments or turning points, people who helped you to follow a certain strategy, something like that?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "I was lucky that Graham Worth joined our group relatively early, in '94. He had a lot of experience with programming, and we really profited from that. He professionalized the whole thing. He was a postdoc here until the end of 2000 and I'm grateful to him. And then there was Frank Otto, a Ph.D. student who had already programmed on an Atari or something as a high-school student. It's very nice when you have employees who know more than you. And otherwise, from the programming perspective, Haobin Wang is to be mentioned, who developed ML (Multilayer). Not with us, in the United States. I was there in 2001 for a birthday party of Bill Miller, that's where I met Haobin Wang. And he had started developing Multilayer MCTDH. We discussed it a lot because we had similar ideas, we called it Cascading. But we never really did anything with it, it seemed too complex to us. And we said, if we start implementing this and it doesn't work, then we'll be doing a lot of unnecessary work. But Haobin Wang just did it. And it worked wonderfully. And then we all followed suit. In this regard, he's my hero."</i></div>
**IU:** And a turning point was the public release of MCTDH. But were there any other points where you changed direction?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Not really. ML, that's Multilayer MCTDH, is an important step forward for larger systems. The Heidelberg ML was mainly programmed by Oriol Vendrell. And we didn't have a big plan. The problems came up and we tried to solve them. We tried to make it better and better. [...] What was a strong and important development in the last few years was the rewriting of the general potential program into the so-called Sum-of-Products form. [...] You can bring the potential into a more compact form, the CPD form, also known as CANDECOMP or Parallel Factors. Markus Schröder made a huge contribution here, because now we have a program, MCCPD, Monte Carlo CPD, which brings general potential surfaces into the sum-of-products format. Quantum chemists provide programs to the scientific community, where you specify coordinates and they return the potential (Born-Oppenheimer) energy. That means they have generated a general fit, but we refit this on the sum-of-products form. The last thing we did in collaboration with Fabien Gatti and others was hydrogen on a graphite surface, and we included several graphite atoms that could move and transfer energy. And this was a big step, because it led to 75 degrees of freedom. And then refitting the surface with 75 degrees of freedom, this was something we couldn't have imagined a few years ago. [...]"</i></div>
**IU:** This shows that you can't rely on computers getting better and just solving larger systems. The problem changes, the representation changes, and this must be represented.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "You need the development of algorithms, that's for sure. When the problem arises and becomes so large that it really bothers you, do you start thinking about new algorithms. In this regard, I'm also happy that MCTDH, which is now 35 years old, is still alive. I was always considering that someone would come up with a completely new idea and develop that much better and more beautiful. But MCTDH has held up. Of course, because we've continued to develop it with ML and so on, which was an important step. But it's still a very good method and can still keep up and is still very much at the forefront."</i></div>

## Development of Research Software in the Academic Environment

**IU:** If you think about it now, this is about the development of research software in the research landscape, and you mentioned that you had Ph.D. students who worked on it and so on. Where do you see critical points in the development of research software in the academic system?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "A critical point is the financing. The DFG finances only scientific research<small>[Note: The DFG has taken a step in the direction of funding research software development.]</small>. If you want to do a bit of software development, you can do it on the side, but you can't write it into an application for funding."</i><small>[Note: A DFG application by Dieter was rejected for this reason].</small> <i>"This doesn't work. And this is different in the UK. Graham Worth received funding, specifically for software development. He then made a fork of the Heidelberg MCTDH, called QUANTICS, and he received funding specifically for the development. This is missing in Germany. This was always a problem for me. You had to have a scientific project but you wanted to do software development. Of course we also wanted to do applications, we don't just develop software for the sake of it. But to get software development into a DFG application, you have to describe the motivation the other way around. You have to write that the application comes first and the development then happens alongside, but in fact good software development is too important. And I hope that this will change a bit."</i></div>
**IU:** And then in the projects you have worked on applications but also included a bit of software maintenance?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Yes, of course. At the beginning, we started with H+H<sub>2</sub>-scattering and things like that. And we put these in the foreground and wrote nice papers about them. Over time, MCTDH developed. But the applications were always the focus of the projects."</i></div>
**IU:** And apart from the fact that you need money to finance the people who develop the software, it's also the case that not always a paper comes out of it. How can you value these contributions, and was this valued in the past when Ph.D. students made contributions?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "As I said, the money is only for the research that has come out, that there was some calculation done, a cross-section or a spectrum or something like that. And the actual software development is not valued. I mean, I value it, but not so much from the funding agency's point of view. And this is the point I criticize, that we should be more flexible."</i></div>
**IU:** This may also have an impact on the career of Ph.D. students if they invest time in it, but it's not counted.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "I had a postdoc who came and said, he didn't want to do software development, he needed papers for his career. I understood this, then we did some nice things with him. This is how it is. For Ph.D. students, it's easier. A Ph.D. student has to write a dissertation, but is not yet thinking about their career at that moment."</i></div>
**IU:** MCTDH has had some publications that should be cited when using the software. Do you think this is a good way to value these contributions?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "I don't see any other way. By now MCTDH is very well-known. But at the beginning, it was difficult. It was strange to many people. Our first really big breakthrough was Pyrazin. [...]</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Pyrazin could be solved in 1999. That's a long time ago. And we thought that was a big breakthrough. But it didn't have much resonance, because we were too far ahead. The others were doing two or three degrees of freedom, and we were doing 24. They didn't quite understand the method, they thought this was a special model. None of the authors were invited to give a talk about it in the following two years or so. Later, our work was very well-recognized. Pyrazin has become a standard model to test other methods. Many semi-classical methods try to solve Pyrazin, yes, this has changed a lot. But this is still very memorable for me, when we solved Pyrazin, we thought we would get great applause. Nothing. The recognition came with a delay."</i>
</div>
<i>A big breakthrough was the Zundel cation. This was also better than what others could do at the time, we could analyze and solve it completely. We got a lot of recognition for this. Nowadays, this is no longer a problem. But at the time, it was."</i></div>

## The Emergence of a Community

**IU:** MCTDH is also used by many researchers who then base their research on the availability and usability of MCTDH. Do you see critical points with this? Having a user community in the research landscape?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "No, it's actually very nice. It's clear that people download MCTDH and use it. And then maybe they turn to other problems, that's just the way it is. They don't necessarily make it the center of their whole research life like I did, but they have a specific problem and use MCTDH for it. Then they might do something else. Some people stay with it, use MCTDH continuously for almost all their things, it differs. I sometimes get an email from a student who wants to use MCTDH. Then I have big doubts that this will be successful. If someone wants to do this alone, if they don't have a suitable environment, it's too complex. Then the student has to be very good, that's it. Mostly I never hear from them again. You need an environment, someone from the quantum chemistry community to say, 'Now we're going to do dynamics.' It is a different way of thinking, the time-dependence. I always find that this is difficult for people. They think very much in eigenstates and now they have to think in wave packets. You need a certain environment and support. One of the students of our MCTDH summer school criticized MCTDH, saying it's too complex. This is not true, quantum dynamics is complex. MCTDH tries to make it as simple as possible. But quantum dynamics is complex. You have to dive in deep."</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>Even if the MCTDH project has taken the programming tasks off your hands, the intellectual effort of dealing with it, this can't be taken away from you."</i></div>
</div>
**IU:** So the users have to understand what's happening, where they can apply MCTDH, and just the documentation isn't enough. You have to get involved in the method, in the papers. But then there may be questions in the application, e.g. "How do I write this in the operator file?"? You certainly get many user inquiries.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "I sometimes get an input and then I pull my hair out. But overall, it's not that complicated, even the operator file. We have an extra ASCII file where you can write in how the operator looks, how the Hamiltonian should look. This can be defined quite well through the sum-of-products structure. There is a whole library of operators that you can then include. First derivative, second derivative, some functions, etc. This can be picked up quite quickly. If you write the input file, you have to have a certain understanding, e.g. how a basis works. Sometimes something doesn't work because, e.g., the grid points are too coarse. Then nothing can work. This is not a MCTDH error, but a real input error. I sometimes get inquiries and an input file, then I try to help."</i></div>
**IU:** Which costs you time.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "This costs me time again, but I'm retired and have the time."</i></div>
**IU:** Therefore, these users can really be happy. Because it's difficult to find the time and provide support. In principle, you can't even finance this through research projects.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Exactly. This is again that point we've already discussed. That the DFG maybe changes its policy a bit."</i></div>
**IU:** Of course, the method is very widely used and applied. You've already mentioned that the users don't really work on the software itself.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Only Markus Schröder and I are mainly responsible for the program itself."</i></div>
**IU:** But then there are compilers that change, hardware changes.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Exactly. From the outside, there are always needs. But these are minor things. A new compiler comes, and suddenly it doesn't work. Then you have to find the command that turns off the new additional check. And then it compiles again. And things like this, minor things happen all the time."</i></div>
**IU:** Also if you think about the programming language itself, Fortran, which was very widely used, especially in chemistry and theoretical physics for these problems. But not so much today.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Fortran is, I think, the best language for number crunching. And of course, the modern language is C++, which can do much more, but you don't need this much in our case. At least not when you're doing things like we are. C++ has a big advantage: Many people are now starting with Python. And you can mix it, of course. Python is wonderful, it's very simple, it's very powerful, but unfortunately, it's very slow. You could now write programs where the entire input and everything is in Python and then the number crunching is outsourced to a higher language. And then C++ is better, because it has the same data structure as Python. And this would be a bit more complicated with Fortran. It is a bit unfortunate that the Python people are orienting themselves towards C++ and not towards Fortran."</i></div>
**IU:** But Fortran has contributed a lot to the field of quantum dynamics or quantum mechanics.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Yes, very much. There is a lot of software written in Fortran. And with 90 and the higher 2003 and what's available now, Fortran has also become much stronger. It's much more flexible and can do much more. I'm happy with Fortran. But this is up to each individual to decide. I'm maybe also stuck in tradition. I grew up with Fortran. That's just the way it is."</i></div>
**IU:** Are there plans in the near future, apart from the Summer School, with MCTDH?

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "No, we will continue to study as large systems as possible, as far as we can. We have a tradition in our group, led by Oriol Vendrell, of investigating protonated water clusters. The last and largest water cluster we investigated was the extended Zundel cation, which has 51 degrees of freedom. This is already quite large. And in this direction, we will certainly continue. We are calculating the absorption spectra of the clusters. This is the application. And from the software development, I don't see anything spectacular at the moment, but this can come. If we encounter a problem that requires a new additional development, then we will also tackle this, as far as possible."</i>
<div style="padding: 0.5rem; margin-top: 0rem; background-color: #0d2476ff; color: white; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>We are always problem-driven. We work on a problem, and we try to solve it."</i></div>
</div>
**IU:** Thank you very much for the conversation.

<div style="padding: 0.5rem; margin-top: -1rem; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4; text-align: block;">
<i>HDM: "Thank you for the conversation, it was nice. Thank you. And I hope it will help to attract more MCTDH users."</i></div>
**IU:** Yes, certainly.

## Key Topics Covered

- Early experiences with programming in theoretical chemistry
- Development and open-source release of MCTDH
- Challenges in funding research software development
- The importance of documentation and community support
- Evolution of computational methods and hardware

## Full Interview Resources

### Complete Transcript
**[Read Full Interview Transcript (German)](/interview-hd-meyer-full/)**

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

**MCTHD authors**: Michael Beck, Andreas Jäckle, Graham Worth, Hans-Dieter Meyer  
**MCTDH Contributors**: Marie-Catherine Heitz, Stephan Wefing, Uwe Manthe, Suren Sukiasyan, Andreas Raab, Masahiro Ehara, Christoph Cattarius, Fabien Gatti, Frank Otto, Mathias Nest, Michael R. Brill, Oriol Vendrell, Markus Schröder, Daniel Pelaez-Ruiz, Phillip S. Thomas, Ying-Chih Chiang, Keyvan Sadri, David Mendive-Tapia

### Related links
Regular [workshops and lectures on MCTDH][MCTDH summer school] take place. In addition, the ["High-Dimensional Quantum Dynamics" conference series][HDQD conferences] has emerged, and there are other (varied) implementations of the MCTDH algorithm in other programs (Uwe Manthe (Bielefeld), Graham Worth (University College London, ["Quantics"][Quantics]), Haobin Wang (Denver)).

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
