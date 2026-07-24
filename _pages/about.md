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
.page__title {
  display: none;
}

.page__content {
  font-size: 1rem;
}

.lab-home {
  --lab-navy: #0b1f3a;
  --lab-blue: #246bfd;
  --lab-text: #182235;
  --lab-muted: #64748b;
  --lab-surface: #f4f7fb;
  --lab-border: #dfe7f1;
  color: var(--lab-text);
}

.lab-home * {
  box-sizing: border-box;
}

.lab-hero {
  position: relative;
  overflow: hidden;
  margin-bottom: 4.5rem;
  padding: 4.5rem 3.5rem;
  border-radius: 1.5rem;
  color: #ffffff;
  background:
    radial-gradient(circle at 90% 10%, rgba(95, 166, 255, 0.45), transparent 30%),
    linear-gradient(135deg, #07182f 0%, #123f78 58%, #246bfd 100%);
}

.lab-hero__grid {
  position: relative;
  z-index: 2;
  display: grid;
  grid-template-columns: minmax(0, 1.45fr) minmax(220px, 0.55fr);
  gap: 3rem;
  align-items: center;
}

.lab-eyebrow,
.lab-kicker {
  margin: 0 0 0.85rem;
  font-size: 0.78rem;
  font-weight: 700;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

.lab-eyebrow {
  color: #bbd7ff;
}

.lab-hero h1 {
  margin: 0;
  color: #ffffff;
  font-size: clamp(2.5rem, 6vw, 4.7rem);
  line-height: 1.04;
  letter-spacing: -0.045em;
}

.lab-hero__lead {
  max-width: 720px;
  margin: 1.4rem 0 0;
  color: #ffffff;
  font-size: clamp(1.25rem, 2.4vw, 1.75rem);
  line-height: 1.45;
}

.lab-hero__description {
  max-width: 680px;
  margin: 1rem 0 0;
  color: #d7e6fb;
  line-height: 1.75;
}

.lab-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 0.85rem;
  margin-top: 2rem;
}

.lab-button {
  display: inline-block;
  padding: 0.78rem 1.15rem;
  border: 1px solid transparent;
  border-radius: 0.7rem;
  font-weight: 700;
  text-decoration: none !important;
  transition: transform 160ms ease, background 160ms ease;
}

.lab-button:hover {
  transform: translateY(-2px);
}

.lab-button--primary {
  color: #12315a !important;
  background: #ffffff;
}

.lab-button--secondary {
  color: #ffffff !important;
  border-color: rgba(255, 255, 255, 0.45);
  background: rgba(255, 255, 255, 0.08);
}

.lab-visual {
  position: relative;
  width: min(260px, 100%);
  aspect-ratio: 1;
  margin: auto;
  border: 1px solid rgba(255, 255, 255, 0.27);
  border-radius: 50%;
}

.lab-orbit {
  position: absolute;
  inset: 15%;
  border: 1px solid rgba(255, 255, 255, 0.32);
  border-radius: 50%;
}

.lab-orbit--two {
  inset: 28%;
}

.lab-core {
  position: absolute;
  top: 50%;
  left: 50%;
  display: grid;
  width: 5rem;
  height: 5rem;
  place-items: center;
  transform: translate(-50%, -50%);
  border-radius: 50%;
  color: #12315a;
  background: #ffffff;
  box-shadow: 0 0 50px rgba(171, 211, 255, 0.7);
  font-size: 2rem;
  font-weight: 800;
}

.lab-particle {
  position: absolute;
  width: 0.9rem;
  height: 0.9rem;
  border-radius: 50%;
  background: #ffffff;
  box-shadow: 0 0 20px rgba(255, 255, 255, 0.9);
}

.lab-particle--one {
  top: 12%;
  left: 46%;
}

.lab-particle--two {
  right: 9%;
  bottom: 29%;
}

.lab-particle--three {
  bottom: 13%;
  left: 22%;
}

.lab-section {
  margin: 0 0 4.5rem;
}

.lab-section__heading {
  max-width: 760px;
  margin-bottom: 2rem;
}

.lab-kicker {
  color: var(--lab-blue);
}

.lab-section h2 {
  margin: 0;
  color: var(--lab-navy);
  font-size: clamp(1.8rem, 3vw, 2.55rem);
  line-height: 1.2;
}

.lab-section__intro {
  margin-top: 1rem;
  color: var(--lab-muted);
  font-size: 1.08rem;
  line-height: 1.8;
}

.lab-research-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1.25rem;
}

.lab-card {
  padding: 1.75rem;
  border: 1px solid var(--lab-border);
  border-radius: 1rem;
  background: #ffffff;
  box-shadow: 0 14px 35px rgba(15, 35, 65, 0.06);
}

.lab-card__number {
  color: var(--lab-blue);
  font-size: 0.82rem;
  font-weight: 800;
  letter-spacing: 0.12em;
}

.lab-card h3 {
  margin: 1rem 0 0.75rem;
  color: var(--lab-navy);
  font-size: 1.2rem;
  line-height: 1.35;
}

.lab-card p {
  margin: 0;
  color: var(--lab-muted);
  line-height: 1.7;
}

.lab-link {
  display: inline-block;
  margin-top: 1.2rem;
  color: var(--lab-blue) !important;
  font-weight: 700;
  text-decoration: none !important;
}

.lab-feature {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
  align-items: stretch;
}

.lab-feature__panel {
  padding: 2.2rem;
  border-radius: 1.1rem;
  background: var(--lab-surface);
}

.lab-feature__panel h3 {
  margin-top: 0;
  color: var(--lab-navy);
  font-size: 1.55rem;
}

.lab-feature__panel p {
  color: var(--lab-muted);
  line-height: 1.75;
}

.lab-join {
  padding: 3rem;
  border-radius: 1.3rem;
  color: #ffffff;
  background: var(--lab-navy);
}

.lab-join h2 {
  color: #ffffff;
}

.lab-join p {
  max-width: 700px;
  color: #d2deed;
  line-height: 1.75;
}

@media (max-width: 800px) {
  .lab-hero {
    padding: 3rem 1.5rem;
  }

  .lab-hero__grid,
  .lab-feature {
    grid-template-columns: 1fr;
  }

  .lab-visual {
    width: 190px;
  }

  .lab-research-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .lab-hero {
    padding: 2.5rem 1.25rem;
    border-radius: 1rem;
  }

  .lab-join,
  .lab-feature__panel {
    padding: 1.5rem;
  }
}
</style>

<div class="lab-home">

  <section class="lab-hero">
    <div class="lab-hero__grid">
      <div>
        <p class="lab-eyebrow">HFNL · University of Science and Technology of China</p>

        <h1>QuantumICT<br>Research Group</h1>

        <p class="lab-hero__lead">
          High-performance computational methods for scientific discovery.
        </p>

        <p class="lab-hero__description">
          We develop and apply computational approaches that connect
          high-performance computing, first-principles methods, and
          kinetic Monte Carlo simulations.
        </p>

        <div class="lab-actions">
          <a class="lab-button lab-button--primary"
             href="{{ '/research/' | relative_url }}">
            Explore Our Research
          </a>

          <a class="lab-button lab-button--secondary"
             href="{{ '/people/' | relative_url }}">
            Meet the Group
          </a>
        </div>
      </div>

      <div class="lab-visual" aria-hidden="true">
        <div class="lab-orbit"></div>
        <div class="lab-orbit lab-orbit--two"></div>
        <div class="lab-core">Q</div>
        <div class="lab-particle lab-particle--one"></div>
        <div class="lab-particle lab-particle--two"></div>
        <div class="lab-particle lab-particle--three"></div>
      </div>
    </div>
  </section>

  <section class="lab-section">
    <div class="lab-section__heading">
      <p class="lab-kicker">About Us</p>

      <h2>Developing computational tools to understand complex scientific systems</h2>

      <p class="lab-section__intro">
        QuantumICT is a research group at HFNL and USTC. Our work focuses
        on developing efficient computational methods and applying them to
        scientific problems across multiple time and length scales.
      </p>
    </div>
  </section>

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
          for scientific simulations.
        </p>
        <a class="lab-link" href="{{ '/research/' | relative_url }}">
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
        <a class="lab-link" href="{{ '/research/' | relative_url }}">
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
        <a class="lab-link" href="{{ '/research/' | relative_url }}">
          Learn more →
        </a>
      </article>
    </div>
  </section>

  <section class="lab-section">
    <div class="lab-feature">
      <div class="lab-feature__panel">
        <p class="lab-kicker">Our Team</p>
        <h3>Researchers working across computation and physical science</h3>
        <p>
          Learn more about the principal investigator, current students,
          and alumni of the group.
        </p>
        <a class="lab-link" href="{{ '/people/' | relative_url }}">
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
        <a class="lab-link" href="{{ '/publications/' | relative_url }}">
          View publications →
        </a>
      </div>
    </div>
  </section>

  <section class="lab-section lab-join">
    <p class="lab-eyebrow">Join Us</p>
    <h2>Work with the QuantumICT Group</h2>
    <p>
      We welcome motivated students and researchers interested in
      computational science and method development.
    </p>

    <div class="lab-actions">
      <a class="lab-button lab-button--primary"
         href="{{ '/join-us/' | relative_url }}">
        Opportunities
      </a>

      <a class="lab-button lab-button--secondary"
         href="mailto:shh@ustc.edu.cn">
        Contact Us
      </a>
    </div>
  </section>

</div>
