---
title: "RSE pioneers - Research Software Engineering Pioneers: Hans-Dieter Meyer"
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
lang: en
permalink: /interview/2025/08/25/Hans-Dieter-Meyer-en.html
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
    left: 0 !important;
    top: 0 !important;
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
</style>

Computer-assisted research has now reached almost all disciplines, challenging researchers in the application and development of research software. With the AI revolution, the next wave of upheaval is already on the horizon.

Some disciplines, however, have been little changed by the digitization of the research process in the past 20 years: particularly those that have "always" (since the 1970s) conducted computer-assisted research. Theoretical chemistry is one such example: here, scientists have "always" developed computer programs and used them in research, with everything that entails - learning programming languages, compilers, and profilers. Over the years, this has led to the creation of several large software packages like [GAMESS](https://www.ameslab.gov/gamess-open-source-quantum-chemistry-software), [Gaussian](https://gaussian.com/), [Molpro](https://www.molpro.net/), and [others](https://en.wikipedia.org/wiki/Category:Computational_chemistry_software) - fundamental building blocks for research and research infrastructures, without which many insights would not have been possible.

How did these first RSEs advance research, what factors influenced the success and spread of research software? What are the differences between today and back then? RSE Pioneers addresses these questions.

<div class="interview-details">
  <h3>Interview Details</h3>
  <p><strong>Interviewee:</strong> Prof. Dr. Hans-Dieter Meyer, Heidelberg University</p>
  <p><strong>Interviewer:</strong> Inga Ulusoy, Scientific Software Center, Heidelberg University</p>
  <p><strong>Date:</strong> May 8, 2025</p>
  <p><strong>Duration:</strong> 60 minutes</p>
  <p><strong>Language:</strong> German (with English summary)</p>
  <p><strong>Topic:</strong> Development and open-source release of the MCTDH (Multi-Configuration Time-Dependent Hartree) software package</p>
</div>

## Introduction

Professor Hans-Dieter Meyer has been working in theoretical chemistry at Heidelberg University since the 1980s. He is the principal developer of the MCTDH (Multi-Configuration Time-Dependent Hartree) software package, one of the most successful quantum dynamics programs worldwide.

MCTDH revolutionized the calculation of quantum dynamics for molecular systems and made it possible to solve problems that were previously computationally intractable. The software has been cited thousands of times and is used by research groups worldwide.

In this interview, Professor Meyer talks about the early days of research software development, the challenges of programming without modern tools, and the decision to make MCTDH open source.

## Early Programming Experiences

**Inga Ulusoy:** Could you tell us about your first experiences with programming?

Professor Meyer began programming in the late 1970s during his doctoral studies. At that time, there were no integrated development environments, no internet, and no Stack Overflow. Everything had to be learned through books and trial and error.

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"At that time, we programmed in Fortran, and you had to submit your programs on punch cards. You had to wait hours or even a day to get your results back. If there was an error, you had to start all over again."</i>
</div>

This experience shaped his approach to programming: careful planning, thorough testing, and detailed documentation became essential skills.

## Development of MCTDH

The development of MCTDH began in the late 1980s. The method was revolutionary because it made it possible to solve the time-dependent Schrödinger equation for complex molecular systems efficiently.

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"The idea behind MCTDH was to represent the wave function as a product of time-dependent basis functions. This allowed us to reduce the exponential scaling problem that plagued other methods."</i>
</div>

### Technical Challenges

The development faced numerous technical challenges:

- **Memory limitations**: Early computers had very limited memory
- **Computing power**: Calculations that now take minutes took days or weeks
- **No version control**: Changes had to be tracked manually
- **Limited collaboration tools**: Sharing code happened via physical media

<div style="display: flex; align-items: center; margin: 1rem 0;">
<img src="{{ '/assets/images/zundel_molden.png' | relative_url }}" alt="The Zundel cation." style="width: 50%; height: auto; margin-right: 1rem;">
<div style="flex: 1; font-style: italic; color: #666;">The Zundel cation, where a proton holds two water molecules together. There are large amplitude motions in a very anharmonic potential, and the kinetic operator is represented in a sum-of-products form with about 150 terms.</div>
</div>

## Success and Recognition

MCTDH achieved significant success in the scientific community. One of the breakthrough applications was the study of the Zundel cation, a system with 15 degrees of freedom that was far beyond what other methods could handle at the time.

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"The Zundel cation was a real breakthrough because it was a genuine molecule, not a model system. With 15 degrees of freedom, it was far better than what other people could do at the time. We could really analyze and solve it completely."</i>
</div>

This success led to widespread recognition and adoption of the MCTDH method in the theoretical chemistry community.

## The Decision to Go Open Source

One of the most significant decisions in the MCTDH story was making the software freely available to the scientific community. This was not a common practice in the early days of scientific software.

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"We decided to make MCTDH freely available because we wanted to enable as many researchers as possible to use the method. Science benefits when tools are accessible to everyone."</i>
</div>

### Impact of Open Source

The open-source release had several positive effects:

- **Wider adoption**: More research groups could access and use the software
- **Community contributions**: Users provided feedback, bug reports, and improvements
- **Educational value**: Students could learn from the well-documented code
- **Scientific reproducibility**: Results could be verified and reproduced

## Documentation and User Support

Professor Meyer emphasized the importance of comprehensive documentation, which was unusual for scientific software at the time.

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"Good documentation was essential because the method was complex. Users needed to understand not just how to run the program, but also the underlying physics and mathematics."</i>
</div>

The MCTDH package includes:

- Detailed user manual with theoretical background
- Practical examples and tutorials
- Input file documentation
- Troubleshooting guides

## Collaboration and Community

**Inga Ulusoy:** How did collaboration work in the early days without modern communication tools?

Collaboration in the pre-internet era required different approaches:

- **Personal meetings**: Much communication happened at conferences and workshops
- **Postal mail**: Code and documentation were shared via physical mail
- **Phone calls**: Important discussions happened over long-distance calls
- **Visiting exchanges**: Researchers spent weeks or months at other institutions

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"Collaboration was more intensive but slower. When we met, we had to make the most of the time because the next opportunity might not come for months."</i>
</div>

## Evolution of the Software

Over the decades, MCTDH has continuously evolved:

### Early Versions (1990s)
- Basic MCTDH implementation
- Fortran 77 codebase
- Limited to small systems

### Modern Versions (2000s-present)
- Extended capabilities (ML-MCTDH, G-MCTDH)
- Modern Fortran standards
- Parallel computing support
- Integration with other software packages

## Challenges in Research Software Development

Professor Meyer identified several persistent challenges in research software development:

### Funding Issues

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"Funding agencies often don't understand that software development is research. They want to fund new physics, not the tools needed to discover that physics."</i>
</div>

### Maintenance and Sustainability

Keeping research software current and functional requires ongoing effort:

- **Code maintenance**: Adapting to new compilers and systems
- **User support**: Helping users with problems and questions
- **Feature development**: Adding new capabilities based on scientific needs
- **Documentation updates**: Keeping manuals current with code changes

## Advice for Modern RSEs

**Inga Ulusoy:** What advice would you give to today's research software engineers?

Professor Meyer offered several insights:

### Focus on Quality

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"Take time to write good code and good documentation. It may seem slower initially, but it saves enormous time in the long run."</i>
</div>

### Understand the Science

Technical skills alone are not sufficient:

- **Learn the domain**: Understand the physics or chemistry behind the code
- **Collaborate with scientists**: Work closely with domain experts
- **Stay current**: Keep up with both computational and scientific developments

### Plan for Longevity

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"Think about who will maintain your software in 10 or 20 years. Write code that others can understand and modify."</i>
</div>

## The Future of MCTDH

Today, MCTDH continues to be actively developed and used worldwide. The software has evolved to include machine learning methods and can handle increasingly complex systems.

<div style="padding: 0.5rem; margin: 1rem 0; background-color: #c8d1efff; color: black; border-radius: 0.375rem; font-size: 1.1rem; line-height: 1.4;">
<i>"The main development now is focused on Markus Schröder and myself. But the user community continues to grow, and we see applications in areas we never imagined when we started."</i>
</div>

## Key Topics Covered

- Early experiences with programming in theoretical chemistry
- Development and open-source release of MCTDH
- Challenges in funding research software development
- The importance of documentation and community support
- Evolution of computational methods and hardware

## Full Interview Resources

### Complete Transcript
**[Read Full German Interview Transcript](/assets/data/InterviewCorrected_5.6.25.markdown)**

### Audio Interview

<div class="audio-section">
  <div class="audio-info">
    <h4>🎧 Full Interview Available</h4>
    <p><strong>Language:</strong> German</p>
    <p><strong>Date:</strong> May 8, 2025</p>
    <p><strong>Duration:</strong> Complete interview with Prof. Hans-Dieter Meyer</p>
  </div>
  
  <div class="audio-links">
    <a href="https://www.buzzsprout.com/2531619/episodes/17727894" target="_blank" rel="noopener noreferrer" class="audio-button">
      🎧 Listen on Buzzsprout
    </a>
  </div>
  
  <div class="audio-note">
    <p><em>Note: The audio player opens in a new window due to platform restrictions. Click the link above to access the full interview.</em></p>
  </div>
</div>

### Related Images

<div class="gallery">
  <div class="gallery-item">
    <a href="https://www.pci.uni-heidelberg.de/tc/dieter.html" target="_blank" rel="noopener noreferrer">
      <img src="{{ '/assets/images/dieter.png' | relative_url }}" alt="Professor Hans-Dieter Meyer" title="Professor Hans-Dieter Meyer">
    </a>
  </div>
  <div class="gallery-item">
    <a href="https://www.pci.uni-heidelberg.de/tc/mctdh.html" target="_blank" rel="noopener noreferrer">
      <img src="{{ '/assets/images/MCTDH.png' | relative_url }}" alt="MCTDH stats" title="MCTDH package tech stats">
    </a>
  </div>
</div>

---

*This interview is part of the RSE Pioneers project, documenting the stories and contributions of early research software engineers in theoretical chemistry and related fields.*
