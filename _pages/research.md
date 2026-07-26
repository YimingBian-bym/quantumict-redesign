---
permalink: /research/
title: "Research"
author_profile: false
classes: wide
toc: false
---

<style>
.page__title { display: none; }
.page__content { margin-top: 0; }
.page__content p, .page__content li { font-size: inherit; }

.research-page {
  --ink: #142238;
  --muted: #637188;
  --blue: #1d5fbf;
  --deep: #061f45;
  --line: #d9e1eb;
  --soft: #f3f6fa;
  color: var(--ink);
}

.research-shell {
  width: min(1160px, calc(100% - 48px));
  margin: 0 auto;
}

.research-label {
  margin: 0 0 1rem;
  color: var(--blue);
  font-size: .76rem;
  font-weight: 750;
  letter-spacing: .16em;
  line-height: 1.2;
  text-transform: uppercase;
}

.research-display,
.research-heading,
.research-subheading {
  margin: 0;
  color: var(--ink);
  font-weight: 630;
  letter-spacing: -.045em;
}

.research-display {
  font-size: clamp(2.8rem, 6vw, 6.8rem);
  line-height: .98;
}

.research-heading {
  font-size: clamp(1.9rem, 3.4vw, 3.3rem);
  line-height: 1.06;
}

.research-subheading {
  font-size: clamp(1.45rem, 2.3vw, 2.2rem);
  line-height: 1.14;
}

.research-body {
  color: var(--muted);
  font-size: clamp(1rem, 1.15vw, 1.12rem);
  line-height: 1.86;
}

.research-body p { margin-top: 0; }
.research-body p:last-child { margin-bottom: 0; }

/* Cover */
.research-hero {
  position: relative;
  width: 100vw;
  margin-left: calc(50% - 50vw);
  overflow: hidden;
  color: #fff;
  background:
    radial-gradient(circle at 84% 24%, rgba(91,164,255,.22), transparent 28%),
    radial-gradient(circle at 70% 82%, rgba(51,112,202,.18), transparent 34%),
    linear-gradient(122deg, #061b3c 0%, #082b5b 52%, #0a3b78 100%);
}

.research-hero::before,
.research-hero::after {
  content: "";
  position: absolute;
  pointer-events: none;
  border: 1px solid rgba(255,255,255,.14);
  border-radius: 50%;
}

.research-hero::before {
  width: 34rem;
  height: 34rem;
  top: -18rem;
  right: -8rem;
}

.research-hero::after {
  width: 22rem;
  height: 22rem;
  right: 6rem;
  bottom: -15rem;
}

.research-hero__inner {
  position: relative;
  z-index: 1;
  padding: clamp(5.5rem, 10vw, 9.5rem) 0 clamp(4.5rem, 8vw, 7.5rem);
}

.research-hero .research-label { color: #9fc8ff; }
.research-hero .research-display { color: #fff; max-width: 1000px; }

.research-hero__lead {
  max-width: 760px;
  margin: 2rem 0 0;
  color: rgba(255,255,255,.78);
  font-size: clamp(1.08rem, 1.65vw, 1.42rem);
  line-height: 1.7;
}

.research-hero__index {
  display: grid;
  grid-template-columns: repeat(3, minmax(0,1fr));
  gap: 1.5rem;
  margin-top: clamp(3.5rem, 7vw, 6rem);
  padding-top: 1.5rem;
  border-top: 1px solid rgba(255,255,255,.22);
}

.research-hero__index-item {
  display: grid;
  grid-template-columns: auto 1fr;
  gap: .9rem;
}

.research-hero__index-number {
  color: #8ec0ff;
  font-size: .75rem;
  font-weight: 750;
  letter-spacing: .1em;
}

.research-hero__index-title {
  color: rgba(255,255,255,.9);
  font-size: .88rem;
  font-weight: 620;
  line-height: 1.45;
}

/* Overview */
.research-overview {
  padding: clamp(5rem, 9vw, 8.5rem) 0;
}

.research-overview__grid {
  display: grid;
  grid-template-columns: minmax(230px,.78fr) minmax(0,1.55fr);
  gap: clamp(3rem,8vw,8rem);
}

.research-overview__statement {
  margin: 2.1rem 0 0;
  padding-left: 1.35rem;
  border-left: 3px solid var(--blue);
  color: var(--ink);
  font-size: clamp(1.12rem,1.65vw,1.4rem);
  font-weight: 560;
  line-height: 1.55;
}

/* Main directions */
.research-directions {
  border-top: 1px solid var(--line);
}

.research-direction {
  display: grid;
  grid-template-columns: minmax(150px,.34fr) minmax(0,1.66fr);
  gap: clamp(2rem,6vw,6.5rem);
  padding: clamp(5rem,9vw,8rem) 0;
  border-bottom: 1px solid var(--line);
}

.research-direction__number {
  color: var(--blue);
  font-size: clamp(3.5rem,7vw,6.8rem);
  font-weight: 580;
  letter-spacing: -.06em;
  line-height: .85;
}

.research-direction__eyebrow {
  margin: 0 0 .9rem;
  color: var(--muted);
  font-size: .74rem;
  font-weight: 730;
  letter-spacing: .14em;
  text-transform: uppercase;
}

.research-direction__intro {
  max-width: 850px;
  margin: 1.75rem 0 0;
}

.research-direction__details {
  display: grid;
  grid-template-columns: repeat(2,minmax(0,1fr));
  gap: clamp(2rem,5vw,5rem);
  margin-top: 3.3rem;
  padding-top: 2rem;
  border-top: 1px solid var(--line);
}

.research-detail__title {
  margin: 0 0 1rem;
  color: var(--ink);
  font-size: .82rem;
  font-weight: 750;
  letter-spacing: .12em;
  text-transform: uppercase;
}

.research-detail ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.research-detail li {
  position: relative;
  margin: 0;
  padding: .58rem 0 .58rem 1.15rem;
  color: var(--muted);
  font-size: .98rem;
  line-height: 1.55;
  border-bottom: 1px solid rgba(217,225,235,.72);
}

.research-detail li::before {
  content: "";
  position: absolute;
  top: 1.18rem;
  left: 0;
  width: .34rem;
  height: .34rem;
  background: var(--blue);
  border-radius: 50%;
}

/* Cross-cutting themes */
.research-themes {
  width: 100vw;
  margin-left: calc(50% - 50vw);
  padding: clamp(5rem,9vw,8rem) 0;
  background: var(--soft);
}

.research-themes__head {
  display: grid;
  grid-template-columns: minmax(220px,.7fr) minmax(0,1.3fr);
  gap: clamp(2.5rem,7vw,7rem);
  align-items: end;
  margin-bottom: clamp(3rem,6vw,5.5rem);
}

.research-themes__intro { max-width: 690px; margin: 0; }

.research-themes__grid {
  display: grid;
  grid-template-columns: repeat(4,minmax(0,1fr));
  border-top: 1px solid #cbd5e2;
}

.research-theme {
  min-height: 245px;
  padding: 2rem 1.8rem 1.5rem 0;
  border-right: 1px solid #cbd5e2;
}

.research-theme:not(:first-child) { padding-left: 1.8rem; }
.research-theme:last-child { border-right: 0; }

.research-theme__number {
  margin: 0 0 2.7rem;
  color: var(--blue);
  font-size: .72rem;
  font-weight: 760;
  letter-spacing: .12em;
}

.research-theme h3 {
  margin: 0;
  color: var(--ink);
  font-size: 1.2rem;
  font-weight: 640;
  line-height: 1.28;
}

.research-theme p {
  margin: .9rem 0 0;
  color: var(--muted);
  font-size: .94rem;
  line-height: 1.7;
}

/* Research process */
.research-approach {
  padding: clamp(5rem,9vw,8rem) 0;
}

.research-approach__head { max-width: 760px; }

.research-approach__steps {
  display: grid;
  grid-template-columns: repeat(4,minmax(0,1fr));
  margin-top: clamp(3rem,6vw,5rem);
  border-top: 1px solid var(--ink);
}

.research-step {
  position: relative;
  padding: 1.6rem 2rem 0 0;
}

.research-step:not(:last-child)::after {
  content: "→";
  position: absolute;
  top: 1.5rem;
  right: 1.2rem;
  color: #9aa7b7;
}

.research-step__number {
  color: var(--blue);
  font-size: .72rem;
  font-weight: 760;
  letter-spacing: .12em;
}

.research-step h3 {
  margin: 2rem 0 0;
  color: var(--ink);
  font-size: 1.12rem;
  font-weight: 640;
  line-height: 1.32;
}

.research-step p {
  margin: .8rem 0 0;
  color: var(--muted);
  font-size: .92rem;
  line-height: 1.68;
}

/* Publications call-to-action */
.research-cta {
  width: 100vw;
  margin-left: calc(50% - 50vw);
  padding: clamp(4.5rem,8vw,7rem) 0;
  background: var(--deep);
}

.research-cta__grid {
  display: grid;
  grid-template-columns: minmax(0,1.4fr) auto;
  gap: 3rem;
  align-items: end;
}

.research-cta .research-label { color: #8ebfff; }
.research-cta .research-heading { max-width: 760px; color: #fff; }

.research-cta__text {
  max-width: 670px;
  margin: 1.35rem 0 0;
  color: rgba(255,255,255,.7);
  font-size: 1rem;
  line-height: 1.75;
}

.research-link {
  display: inline-flex;
  align-items: center;
  gap: .65rem;
  padding: .85rem 0;
  color: #fff !important;
  font-size: .86rem;
  font-weight: 720;
  letter-spacing: .1em;
  text-decoration: none !important;
  text-transform: uppercase;
  border-bottom: 1px solid rgba(255,255,255,.55);
  transition: gap 160ms ease, border-color 160ms ease;
}

.research-link:hover {
  gap: .95rem;
  border-color: #fff;
}

@media (max-width: 900px) {
  .research-overview__grid,
  .research-themes__head {
    grid-template-columns: 1fr;
    gap: 2rem;
  }

  .research-themes__grid,
  .research-approach__steps {
    grid-template-columns: repeat(2,minmax(0,1fr));
  }

  .research-theme:nth-child(2) { border-right: 0; }
  .research-theme:nth-child(n+3) { border-top: 1px solid #cbd5e2; }
  .research-theme:nth-child(3) { padding-left: 0; }
  .research-step:nth-child(2)::after { display: none; }

  .research-cta__grid {
    grid-template-columns: 1fr;
    align-items: start;
  }
}

@media (max-width: 680px) {
  .research-shell { width: min(100% - 30px,1160px); }

  .research-hero__index,
  .research-direction,
  .research-direction__details,
  .research-themes__grid,
  .research-approach__steps {
    grid-template-columns: 1fr;
  }

  .research-direction { gap: 2rem; }
  .research-direction__number { font-size: 3.7rem; }

  .research-theme,
  .research-theme:not(:first-child) {
    min-height: 0;
    padding: 1.7rem 0;
    border-right: 0;
    border-top: 1px solid #cbd5e2;
  }

  .research-theme:first-child { border-top: 0; }
  .research-theme__number { margin-bottom: 1rem; }

  .research-step {
    padding: 1.6rem 0 1.8rem;
    border-bottom: 1px solid var(--line);
  }

  .research-step:not(:last-child)::after { display: none; }
  .research-step h3 { margin-top: 1rem; }
}
</style>

<!--
First-draft copy based on the previous QuantumICT website and publicly available
USTC/HFNL profiles. Please ask the PI to review the formal direction names and
scope before final publication.
-->

<div class="research-page">

<header class="research-hero">
  <div class="research-shell research-hero__inner">
    <p class="research-label">Research at QuantumICT</p>

    <h1 class="research-display">
      From fundamental methods<br>
      to large-scale discovery.
    </h1>

    <p class="research-hero__lead">
      We develop accurate computational methods, scalable algorithms, and
      scientific software for understanding matter and chemical processes
      across electronic, atomistic, and long-time scales.
    </p>

    <div class="research-hero__index" aria-label="Core research directions">
      <div class="research-hero__index-item">
        <span class="research-hero__index-number">01</span>
        <span class="research-hero__index-title">High-Performance Computing</span>
      </div>
      <div class="research-hero__index-item">
        <span class="research-hero__index-number">02</span>
        <span class="research-hero__index-title">First-Principles Methods</span>
      </div>
      <div class="research-hero__index-item">
        <span class="research-hero__index-number">03</span>
        <span class="research-hero__index-title">Kinetic Monte Carlo &amp; Multiscale Simulation</span>
      </div>
    </div>
  </div>
</header>

<main>

<section class="research-overview">
  <div class="research-shell research-overview__grid">
    <div>
      <p class="research-label">Overview</p>
      <h2 class="research-heading">Computational science across scales.</h2>
    </div>

    <div class="research-body">
      <p>
        QuantumICT works at the intersection of computational chemistry,
        materials simulation, numerical algorithms, and high-performance
        computing. Our research aims to turn fundamental physical models
        into reliable and scalable computational tools.
      </p>

      <p>
        We are particularly interested in the development and implementation
        of high-accuracy first-principles methods, the efficient use of modern
        computing architectures, and the extension of simulations toward
        larger systems and longer time scales. Quantum algorithms and
        artificial intelligence provide additional routes for improving
        models, algorithms, and scientific workflows.
      </p>

      <p class="research-overview__statement">
        Our goal is not only to perform simulations, but also to develop the
        methods and software that make previously inaccessible simulations possible.
      </p>
    </div>
  </div>
</section>

<section class="research-directions" aria-label="Core research directions">

  <article class="research-shell research-direction">
    <div class="research-direction__number" aria-hidden="true">01</div>

    <div>
      <p class="research-direction__eyebrow">Scalable algorithms and scientific software</p>
      <h2 class="research-heading">High-Performance Computing</h2>

      <div class="research-body research-direction__intro">
        <p>
          Large-scale scientific simulation requires more than access to a
          supercomputer. It requires algorithms, data structures, and software
          that can use massive parallelism efficiently. We develop
          high-performance approaches for computational chemistry and materials
          science, with attention to scalability, numerical stability,
          communication cost, memory use, and performance portability.
        </p>

        <p>
          This direction connects method development with modern computing
          platforms. It supports large electronic-structure calculations,
          spectroscopy simulations, atomistic models, and classical emulation
          of quantum-computing workflows.
        </p>
      </div>

      <div class="research-direction__details">
        <div class="research-detail">
          <h3 class="research-detail__title">Methods and technologies</h3>
          <ul>
            <li>Massively parallel numerical algorithms</li>
            <li>Heterogeneous CPU and accelerator computing</li>
            <li>Distributed tensor and linear-algebra operations</li>
            <li>Performance analysis and software optimization</li>
          </ul>
        </div>

        <div class="research-detail">
          <h3 class="research-detail__title">Scientific applications</h3>
          <ul>
            <li>Extreme-scale first-principles simulation</li>
            <li>Large molecular and materials systems</li>
            <li>Vibrational and Raman-spectrum simulation</li>
            <li>Quantum-chemistry algorithm emulation</li>
          </ul>
        </div>
      </div>
    </div>
  </article>

  <article class="research-shell research-direction">
    <div class="research-direction__number" aria-hidden="true">02</div>

    <div>
      <p class="research-direction__eyebrow">Electronic structure and atomistic properties</p>
      <h2 class="research-heading">First-Principles Methods</h2>

      <div class="research-body research-direction__intro">
        <p>
          First-principles methods provide a route from the laws of quantum
          mechanics to predictive models of molecules and materials. We develop
          and implement accurate electronic-structure and response methods,
          with an emphasis on formulations that are both physically reliable
          and computationally efficient.
        </p>

        <p>
          Our interests include electronic structure, lattice dynamics,
          electron–phonon interactions, vibrational properties, and
          spectroscopy. By combining theoretical formulation, numerical
          implementation, and high-performance computing, we seek to connect
          microscopic interactions with observable material behavior.
        </p>
      </div>

      <div class="research-direction__details">
        <div class="research-detail">
          <h3 class="research-detail__title">Method development</h3>
          <ul>
            <li>Density-functional and electronic-structure methods</li>
            <li>Real-space and perturbative formulations</li>
            <li>Lattice dynamics and vibrational calculations</li>
            <li>Electron–phonon and response-property methods</li>
          </ul>
        </div>

        <div class="research-detail">
          <h3 class="research-detail__title">Questions we address</h3>
          <ul>
            <li>How electronic structure determines material properties</li>
            <li>How atomic motion influences electronic behavior</li>
            <li>How spectra reveal microscopic structure and dynamics</li>
            <li>How accurate methods can scale to larger systems</li>
          </ul>
        </div>
      </div>
    </div>
  </article>

  <article class="research-shell research-direction">
    <div class="research-direction__number" aria-hidden="true">03</div>

    <div>
      <p class="research-direction__eyebrow">Rare events, long time scales, and connected models</p>
      <h2 class="research-heading">Kinetic Monte Carlo &amp; Multiscale Simulation</h2>

      <div class="research-body research-direction__intro">
        <p>
          Many important processes occur over time scales that are difficult
          to access through direct atomistic dynamics. Kinetic Monte Carlo
          methods describe these processes through elementary events and
          transition rates, allowing simulations to reach longer times and
          larger effective scales.
        </p>

        <p>
          We are interested in efficient kinetic models, large event spaces,
          rare-event processes, and links between electronic-structure data
          and long-time dynamics. Data-driven techniques can assist with model
          construction and computational acceleration, while multiscale
          strategies connect information across different levels of description.
        </p>
      </div>

      <div class="research-direction__details">
        <div class="research-detail">
          <h3 class="research-detail__title">Methodological interests</h3>
          <ul>
            <li>Kinetic Monte Carlo algorithms</li>
            <li>Rare-event and transition-rate modeling</li>
            <li>Data-assisted model construction</li>
            <li>Multiscale coupling and workflow design</li>
          </ul>
        </div>

        <div class="research-detail">
          <h3 class="research-detail__title">Target phenomena</h3>
          <ul>
            <li>Long-time atomistic evolution</li>
            <li>Diffusion and activated processes</li>
            <li>Complex reaction and transition networks</li>
            <li>Large-scale kinetic systems</li>
          </ul>
        </div>
      </div>
    </div>
  </article>

</section>

<section class="research-themes">
  <div class="research-shell">
    <div class="research-themes__head">
      <div>
        <p class="research-label">Cross-cutting themes</p>
        <h2 class="research-heading">Ideas that connect our work.</h2>
      </div>

      <p class="research-body research-themes__intro">
        The boundaries between methods, software, and applications are fluid.
        Several themes run across our research directions and help translate
        theoretical ideas into practical computational capabilities.
      </p>
    </div>

    <div class="research-themes__grid">
      <article class="research-theme">
        <p class="research-theme__number">01 / 04</p>
        <h3>Quantum Algorithms</h3>
        <p>
          Algorithms and classical emulation strategies for exploring
          quantum-computing approaches to chemistry and many-body problems.
        </p>
      </article>

      <article class="research-theme">
        <p class="research-theme__number">02 / 04</p>
        <h3>Artificial Intelligence</h3>
        <p>
          Data-driven models and learning-based tools that complement
          physical methods, sampling strategies, and scientific workflows.
        </p>
      </article>

      <article class="research-theme">
        <p class="research-theme__number">03 / 04</p>
        <h3>Scientific Software</h3>
        <p>
          Reproducible implementations that connect mathematical methods
          with modern architectures and real scientific applications.
        </p>
      </article>

      <article class="research-theme">
        <p class="research-theme__number">04 / 04</p>
        <h3>Multiscale Modeling</h3>
        <p>
          Connections between electronic, atomistic, kinetic, and
          quantum-computing descriptions of complex systems.
        </p>
      </article>
    </div>
  </div>
</section>

<section class="research-approach">
  <div class="research-shell">
    <div class="research-approach__head">
      <p class="research-label">Our approach</p>
      <h2 class="research-heading">A continuous path from theory to discovery.</h2>
    </div>

    <div class="research-approach__steps">
      <article class="research-step">
        <span class="research-step__number">01</span>
        <h3>Scientific Question</h3>
        <p>
          Identify the physical mechanism, scale, and observable that the
          simulation must describe.
        </p>
      </article>

      <article class="research-step">
        <span class="research-step__number">02</span>
        <h3>Method Development</h3>
        <p>
          Formulate accurate models and numerical algorithms with clear
          approximations and error controls.
        </p>
      </article>

      <article class="research-step">
        <span class="research-step__number">03</span>
        <h3>Implementation</h3>
        <p>
          Translate methods into scalable software for modern computing
          platforms and scientific workflows.
        </p>
      </article>

      <article class="research-step">
        <span class="research-step__number">04</span>
        <h3>Simulation &amp; Insight</h3>
        <p>
          Apply the resulting tools to complex systems and connect numerical
          results with physical understanding.
        </p>
      </article>
    </div>
  </div>
</section>

<section class="research-cta">
  <div class="research-shell research-cta__grid">
    <div>
      <p class="research-label">Selected work</p>
      <h2 class="research-heading">Explore the publications behind our research.</h2>
      <p class="research-cta__text">
        Browse our work in high-performance scientific computing,
        electronic-structure theory, quantum chemistry, kinetic simulation,
        and related computational methods.
      </p>
    </div>

    <a class="research-link" href="{{ '/publications/' | relative_url }}">
      View publications <span aria-hidden="true">→</span>
    </a>
  </div>
</section>

</main>
</div>
