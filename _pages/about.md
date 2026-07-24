---
permalink: /
title: "QuantumICT Research Group"
author_profile: false
redirect_from:
  - /about/
  - /about.html
  - /QuantumICT/
---

<style>
/* =========================================================
   Override the narrow article layout of Academic Pages
   ========================================================= */

#main {
  width: 100% !important;
  max-width: 1500px !important;
  margin: 0 auto !important;
  padding-right: clamp(20px, 4vw, 64px) !important;
  padding-left: clamp(20px, 4vw, 64px) !important;
}

#main .page {
  float: none !important;
  width: 100% !important;
  margin: 0 !important;
  padding-right: 0 !important;
  padding-left: 0 !important;
}

#main .page__inner-wrap,
#main .page__content {
  width: 100% !important;
  max-width: none !important;
  margin-right: 0 !important;
  margin-left: 0 !important;
}

.masthead__inner-wrap {
  width: 100% !important;
  max-width: 1500px !important;
  padding-right: clamp(20px, 4vw, 64px) !important;
  padding-left: clamp(20px, 4vw, 64px) !important;
}

.page__title {
  display: none;
}

/* =========================================================
   Homepage design variables
   ========================================================= */

.lab-home {
  --lab-navy: #081d38;
  --lab-deep-blue: #123f78;
  --lab-blue: #2568f5;
  --lab-light-blue: #dbeaff;
  --lab-text: #13233b;
  --lab-muted: #62728a;
  --lab-surface: #f3f6fb;
  --lab-border: #dfe7f1;

  width: 100%;
  max-width: 1280px;
  margin: 0 auto;
  color: var(--lab-text);
}

.lab-home,
.lab-home * {
  box-sizing: border-box;
}

.lab-home a {
  text-decoration: none;
}

/* =========================================================
   Hero
   ========================================================= */

.lab-hero {
  position: relative;
  overflow: hidden;
  margin: 2rem 0 5.5rem;
  padding: clamp(3.2rem, 6vw, 6rem);
  border-radius: 1.7rem;
  color: #ffffff;
  background:
    radial-gradient(
      circle at 90% 10%,
      rgba(109, 178, 255, 0.48),
      transparent 31%
    ),
    radial-gradient(
      circle at 15% 90%,
      rgba(37, 104, 245, 0.22),
      transparent 35%
    ),
    linear-gradient(
      135deg,
      #06172e 0%,
      #103d74 55%,
      #2568f5 100%
    );
  box-shadow: 0 28px 70px rgba(8, 29, 56, 0.18);
}

.lab-hero::before {
  position: absolute;
  top: -180px;
  right: -150px;
  width: 430px;
  height: 430px;
  border: 1px solid rgba(255, 255, 255, 0.12);
  border-radius: 50%;
  content: "";
}

.lab-hero::after {
  position: absolute;
  right: 90px;
  bottom: -230px;
  width: 470px;
  height: 470px;
  border: 1px solid rgba(255, 255, 255, 0.09);
  border-radius: 50%;
  content: "";
}

.lab-hero__grid {
  position: relative;
  z-index: 2;
  display: grid;
  grid-template-columns:
    minmax(0, 1.2fr)
    minmax(280px, 0.8fr);
  gap: clamp(2rem, 6vw, 6rem);
  align-items: center;
}

.lab-eyebrow,
.lab-kicker {
  margin: 0 0 1rem;
  font-size: 0.78rem;
  font-weight: 800;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

.lab-eyebrow {
  color: #c8ddff;
}

.lab-hero h1 {
  max-width: 750px;
  margin: 0;
  color: #ffffff;
  font-size: clamp(3rem, 5.5vw, 5.2rem);
  line-height: 1.03;
  letter-spacing: -0.05em;
}

.lab-hero__lead {
  max-width: 720px;
  margin: 1.5rem 0 0;
  color: #ffffff;
  font-size: clamp(1.3rem, 2.2vw, 1.8rem);
  font-weight: 600;
  line-height: 1.45;
}

.lab-hero__description {
  max-width: 680px;
  margin: 1.2rem 0 0;
  color: #d4e3f7;
  font-size: 1.04rem;
  line-height: 1.85;
}

.lab-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 0.9rem;
  margin-top: 2.2rem;
}

.lab-button {
  display: inline-flex;
  min-height: 46px;
  align-items: center;
  justify-content: center;
  padding: 0.82rem 1.25rem;
  border: 1px solid transparent;
  border-radius: 0.72rem;
  font-size: 0.93rem;
  font-weight: 750;
  transition:
    transform 160ms ease,
    background 160ms ease,
    border-color 160ms ease;
}

.lab-button:hover {
  transform: translateY(-2px);
}

.lab-button--primary {
  color: #12315a !important;
  background: #ffffff;
}

.lab-button--primary:hover {
  background: #edf5ff;
}

.lab-button--secondary {
  color: #ffffff !important;
  border-color: rgba(255, 255, 255, 0.42);
  background: rgba(255, 255, 255, 0.08);
}

.lab-button--secondary:hover {
  border-color: rgba(255, 255, 255, 0.7);
  background: rgba(255, 255, 255, 0.14);
}

/* =========================================================
   Scientific visual
   ========================================================= */

.lab-visual {
  position: relative;
  width: min(340px, 100%);
  aspect-ratio: 1;
  margin: auto;
  border: 1px solid rgba(255, 255, 255, 0.23);
  border-radius: 50%;
}

.lab-orbit {
  position: absolute;
  inset: 14%;
  border: 1px solid rgba(255, 255, 255, 0.28);
  border-radius: 50%;
}

.lab-orbit--two {
  inset: 28%;
}

.lab-orbit--three {
  inset: 40%;
}

.lab-core {
  position: absolute;
  top: 50%;
  left: 50%;
  display: grid;
  width: 6.2rem;
  height: 6.2rem;
  place-items: center;
  transform: translate(-50%, -50%);
  border-radius: 50%;
  color: #153964;
  background: #ffffff;
  box-shadow: 0 0 55px rgba(171, 211, 255, 0.7);
  font-size: 2.3rem;
  font-weight: 850;
}

.lab-particle {
  position: absolute;
  width: 0.95rem;
  height: 0.95rem;
  border-radius: 50%;
  background: #ffffff;
  box-shadow: 0 0 22px rgba(255, 255, 255, 0.95);
}

.lab-particle--one {
  top: 11%;
  left: 47%;
}

.lab-particle--two {
  right: 8%;
  bottom: 29%;
}

.lab-particle--three {
  bottom: 12%;
  left: 22%;
}

/* =========================================================
   General sections
   ========================================================= */

.lab-section {
  margin: 0 0 6rem;
}

.lab-section__heading {
  max-width: 850px;
  margin-bottom: 2.4rem;
}

.lab-kicker {
  color: var(--lab-blue);
}

.lab-section h2 {
  margin: 0;
  color: var(--lab-navy);
  font-size: clamp(2rem, 3.3vw, 3rem);
  line-height: 1.18;
  letter-spacing: -0.025em;
}

.lab-section__intro {
  margin: 1.2rem 0 0;
  color: var(--lab-muted);
  font-size: 1.08rem;
  line-height: 1.9;
}

/* =========================================================
   About: horizontal desktop layout
   ========================================================= */

.lab-about {
  display: grid;
  grid-template-columns:
    minmax(300px, 0.95fr)
    minmax(0, 1.05fr);
  gap: clamp(3rem, 7vw, 7rem);
  align-items: start;
}

.lab-about .lab-section__intro {
  margin-top: 0;
}

.lab-link {
  display: inline-flex;
  align-items: center;
  margin-top: 1.25rem;
  color: var(--lab-blue) !important;
  font-size: 0.95rem;
  font-weight: 750;
  transition: transform 150ms ease;
}

.lab-link:hover {
  transform: translateX(3px);
}

/* =========================================================
   Research cards
   ========================================================= */

.lab-research-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.6rem;
}

.lab-card {
  display: flex;
  min-height: 300px;
  flex-direction: column;
  padding: 2rem;
  border: 1px solid var(--lab-border);
  border-radius: 1.1rem;
  background: #ffffff;
  box-shadow: 0 16px 42px rgba(15, 35, 65, 0.065);
  transition:
    transform 170ms ease,
    box-shadow 170ms ease,
    border-color 170ms ease;
}

.lab-card:hover {
  transform: translateY(-5px);
  border-color: #bfd3f5;
  box-shadow: 0 22px 55px rgba(15, 35, 65, 0.12);
}

.lab-card__number {
  color: var(--lab-blue);
  font-size: 0.8rem;
  font-weight: 850;
  letter-spacing: 0.14em;
}

.lab-card h3 {
  margin: 1.2rem 0 0.85rem;
  color: var(--lab-navy);
  font-size: 1.35rem;
  line-height: 1.32;
}

.lab-card p {
  margin: 0;
  color: var(--lab-muted);
  line-height: 1.8;
}

.lab-card .lab-link {
  margin-top: auto;
  padding-top: 1.5rem;
}

/* =========================================================
   Team and publications
   ========================================================= */

.lab-feature {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1.7rem;
}

.lab-feature__panel {
  min-height: 290px;
  padding: clamp(2rem, 4vw, 3rem);
  border: 1px solid #e5ebf3;
  border-radius: 1.2rem;
  background: var(--lab-surface);
}

.lab-feature__panel h3 {
  max-width: 470px;
  margin: 0;
  color: var(--lab-navy);
  font-size: clamp(1.5rem, 2.3vw, 2.05rem);
  line-height: 1.28;
}

.lab-feature__panel p {
  max-width: 560px;
  margin: 1rem 0 0;
  color: var(--lab-muted);
  line-height: 1.8;
}

/* =========================================================
   Join us: horizontal desktop layout
   ========================================================= */

.lab-join {
  padding: clamp(2.5rem, 5vw, 4.5rem);
  border-radius: 1.4rem;
  color: #ffffff;
  background:
    radial-gradient(
      circle at 95% 10%,
      rgba(64, 136, 255, 0.25),
      transparent 32%
    ),
    var(--lab-navy);
}

.lab-join__inner {
  display: grid;
  grid-template-columns:
    minmax(0, 1fr)
    auto;
  gap: 3rem;
  align-items: end;
}

.lab-join h2 {
  max-width: 750px;
  color: #ffffff;
}

.lab-join p {
  max-width: 760px;
  margin: 1.1rem 0 0;
  color: #d2deed;
  font-size: 1.04rem;
  line-height: 1.8;
}

.lab-join .lab-actions {
  justify-content: flex-end;
  margin-top: 0;
}

/* =========================================================
   Responsive layout
   ========================================================= */

@media (max-width: 900px) {
  #main,
  .masthead__inner-wrap {
    padding-right: 24px !important;
    padding-left: 24px !important;
  }

  .lab-hero {
    padding: 3.5rem 2.5rem;
  }

  .lab-hero__grid {
    grid-template-columns:
      minmax(0, 1.15fr)
      minmax(230px, 0.85fr);
    gap: 2.5rem;
  }

  .lab-visual {
    width: 260px;
  }

  .lab-core {
    width: 5.2rem;
    height: 5.2rem;
  }

  .lab-research-grid {
    gap: 1rem;
  }

  .lab-card {
    padding: 1.5rem;
  }
}

@media (max-width: 760px) {
  #main,
  .masthead__inner-wrap {
    padding-right: 16px !important;
    padding-left: 16px !important;
  }

  .lab-hero {
    margin-top: 1rem;
    padding: 3rem 1.6rem;
  }

  .lab-hero__grid,
  .lab-about,
  .lab-feature,
  .lab-join__inner {
    grid-template-columns: 1fr;
  }

  .lab-visual {
    width: 230px;
    margin-top: 1.5rem;
  }

  .lab-research-grid {
    grid-template-columns: 1fr;
  }

  .lab-card {
    min-height: auto;
  }

  .lab-join .lab-actions {
    justify-content: flex-start;
    margin-top: 1rem;
  }

  .lab-section {
    margin-bottom: 4.5rem;
  }
}

@media (max-width: 480px) {
  #main,
  .masthead__inner-wrap {
    padding-right: 12px !important;
    padding-left: 12px !important;
  }

  .lab-hero {
    padding: 2.6rem 1.25rem;
    border-radius: 1.05rem;
  }

  .lab-hero h1 {
    font-size: 2.75rem;
  }

  .lab-visual {
    width: 195px;
  }

  .lab-core {
    width: 4.5rem;
    height: 4.5rem;
    font-size: 1.8rem;
  }

  .lab-feature__panel,
  .lab-join {
    padding: 1.7rem;
  }

  .lab-actions {
    align-items: stretch;
    flex-direction: column;
  }

  .lab-button {
    width: 100%;
  }
}
</style>

<div class="lab-home">

  <!-- Hero -->
  <section class="lab-hero">
    <div class="lab-hero__grid">

      <div>
        <p class="lab-eyebrow">
          HFNL · University of Science and Technology of China
        </p>

        <h1>QuantumICT Research Group</h1>

        <p class="lab-hero__lead">
          High-performance computational methods for scientific discovery.
        </p>

        <p class="lab-hero__description">
          We develop and apply computational approaches that connect
          high-performance computing, first-principles methods, and
          kinetic Monte Carlo simulations.
        </p>

        <div class="lab-actions">
          <a
            class="lab-button lab-button--primary"
            href="{{ '/research/' | relative_url }}"
          >
            Explore Our Research
          </a>

          <a
            class="lab-button lab-button--secondary"
            href="{{ '/people/' | relative_url }}"
          >
            Meet the Group
          </a>
        </div>
      </div>

      <div class="lab-visual" aria-hidden="true">
        <div class="lab-orbit"></div>
        <div class="lab-orbit lab-orbit--two"></div>
        <div class="lab-orbit lab-orbit--three"></div>

        <div class="lab-core">Q</div>

        <div class="lab-particle lab-particle--one"></div>
        <div class="lab-particle lab-particle--two"></div>
        <div class="lab-particle lab-particle--three"></div>
      </div>

    </div>
  </section>

  <!-- About -->
  <section class="lab-section lab-about">

    <div>
      <p class="lab-kicker">About Us</p>

      <h2>
        Developing computational tools to understand complex scientific
        systems
      </h2>
    </div>

    <div>
      <p class="lab-section__intro">
        QuantumICT is a research group at HFNL and USTC. Our work focuses
        on developing efficient computational methods and applying them
        to scientific problems across multiple time and length scales.
      </p>

      <a
        class="lab-link"
        href="{{ '/research/' | relative_url }}"
      >
        Discover our research →
      </a>
    </div>

  </section>

  <!-- Research -->
  <section class="lab-section">

    <div class="lab-section__heading">
      <p class="lab-kicker">Research</p>
      <h2>Our main research directions</h2>
    </div>

    <div class="lab-research-grid">

      <article class="lab-card">
        <span class="lab-card__number">01</span>

        <h3>High-Performance Computing</h3>

        <p>
          Efficient algorithms and large-scale computational approaches
          for scientific simulations and data-intensive research.
        </p>

        <a
          class="lab-link"
          href="{{ '/research/' | relative_url }}"
        >
          Learn more →
        </a>
      </article>

      <article class="lab-card">
        <span class="lab-card__number">02</span>

        <h3>First-Principles Methods</h3>

        <p>
          Development and implementation of atomistic methods based on
          fundamental physical principles.
        </p>

        <a
          class="lab-link"
          href="{{ '/research/' | relative_url }}"
        >
          Learn more →
        </a>
      </article>

      <article class="lab-card">
        <span class="lab-card__number">03</span>

        <h3>Kinetic Monte Carlo</h3>

        <p>
          Computational methods for investigating dynamical processes
          over extended time scales.
        </p>

        <a
          class="lab-link"
          href="{{ '/research/' | relative_url }}"
        >
          Learn more →
        </a>
      </article>

    </div>
  </section>

  <!-- Team and publications -->
  <section class="lab-section">

    <div class="lab-feature">

      <div class="lab-feature__panel">
        <p class="lab-kicker">Our Team</p>

        <h3>
          Researchers working across computation and physical science
        </h3>

        <p>
          Learn more about the principal investigator, current students,
          and alumni of the group.
        </p>

        <a
          class="lab-link"
          href="{{ '/people/' | relative_url }}"
        >
          View all members →
        </a>
      </div>

      <div class="lab-feature__panel">
        <p class="lab-kicker">Publications</p>

        <h3>Explore our research output</h3>

        <p>
          Browse publications covering method development,
          high-performance simulation, and scientific applications.
        </p>

        <a
          class="lab-link"
          href="{{ '/publications/' | relative_url }}"
        >
          View publications →
        </a>
      </div>

    </div>
  </section>

  <!-- Join us -->
  <section class="lab-section lab-join">

    <div class="lab-join__inner">

      <div>
        <p class="lab-eyebrow">Join Us</p>

        <h2>Work with the QuantumICT Group</h2>

        <p>
          We welcome motivated students and researchers interested in
          computational science, high-performance simulation, and
          scientific method development.
        </p>
      </div>

      <div class="lab-actions">
        <a
          class="lab-button lab-button--primary"
          href="{{ '/join-us/' | relative_url }}"
        >
          Opportunities
        </a>

        <a
          class="lab-button lab-button--secondary"
          href="mailto:shh@ustc.edu.cn"
        >
          Contact Us
        </a>
      </div>

    </div>
  </section>

</div>
