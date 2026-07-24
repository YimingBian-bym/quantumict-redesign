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
   Homepage layout reset
   ========================================================= */

#main {
  width: 100% !important;
  max-width: none !important;
  margin: 0 !important;
  padding: 0 !important;
}

#main .page {
  float: none !important;
  width: 100% !important;
  margin: 0 !important;
  padding: 0 !important;
}

#main .page__inner-wrap,
#main .page__content {
  width: 100% !important;
  max-width: none !important;
  margin: 0 !important;
  padding: 0 !important;
}

.page__title,
.page__meta {
  display: none !important;
}

/*
  不覆盖 masthead、greedy-nav 和 site-title，
  让首页导航栏与其他页面保持一致。
*/

/* =========================================================
   Global homepage styles
   ========================================================= */

.lab-home {
  --navy: #092955;
  --navy-deep: #041d3c;
  --blue: #005ee8;
  --blue-light: #dceaff;
  --text: #183154;
  --muted: #5f7189;
  --line: #dce3ec;
  --surface: #f3f7fc;
  --white: #ffffff;

  width: 100%;
  margin: 0 !important;
  color: var(--text);
  font-family:
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    Arial,
    sans-serif;
}

.lab-home,
.lab-home * {
  box-sizing: border-box;
}

.lab-home a {
  text-decoration: none;
}

.lab-container {
  width: min(1240px, calc(100% - 48px));
  margin: 0 auto;
}

.lab-display {
  font-family: Georgia, "Times New Roman", serif;
  font-weight: 500;
  letter-spacing: -0.035em;
}

/*
  About Us / Research / Our Team /
  Publications / Join Us

  字号为 3.04rem，约为 01 / 02 / 03 的两倍。
*/

.lab-label {
  max-width: 100%;
  margin: 0 0 1.15rem;
  color: var(--blue);
  font-size: 3.04rem;
  font-weight: 800;
  letter-spacing: 0.035em;
  line-height: 1;
  overflow-wrap: anywhere;
  text-transform: uppercase;
}

.lab-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  color: var(--blue) !important;
  font-size: 0.9rem;
  font-weight: 700;
  transition:
    gap 160ms ease,
    opacity 160ms ease;
}

.lab-link:hover {
  gap: 0.72rem;
  opacity: 0.78;
}

/* =========================================================
   Hero
   ========================================================= */

.lab-hero {
  position: relative;
  overflow: hidden;
  color: #ffffff;
  background:
    radial-gradient(
      circle at 84% 26%,
      rgba(94, 160, 255, 0.4),
      transparent 31%
    ),
    linear-gradient(
      112deg,
      #062957 0%,
      #06438c 53%,
      #1768db 100%
    );
}

.lab-hero::before {
  position: absolute;
  top: -290px;
  right: -40px;
  width: 680px;
  height: 680px;
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 50%;
  content: "";
}

.lab-hero::after {
  position: absolute;
  right: 9%;
  bottom: -360px;
  width: 720px;
  height: 720px;
  border: 1px solid rgba(255, 255, 255, 0.07);
  border-radius: 50%;
  content: "";
}

.lab-hero__inner {
  position: relative;
  z-index: 2;
  display: grid;
  min-height: 560px;
  grid-template-columns:
    minmax(0, 1.05fr)
    minmax(350px, 0.95fr);
  gap: 5rem;
  align-items: center;
  padding-top: 4.8rem;
  padding-bottom: 4.8rem;
}

.lab-hero__institution {
  margin: 0 0 1.15rem;
  color: #d4e5ff;
  font-size: 0.77rem;
  font-weight: 750;
  letter-spacing: 0.18em;
  line-height: 1.7;
  text-transform: uppercase;
}

.lab-hero h1 {
  max-width: 730px;
  margin: 0;
  color: #ffffff;
  font-size: clamp(3.8rem, 6.2vw, 6.3rem);
  line-height: 0.94;
}

.lab-hero__accent {
  width: 42px;
  height: 2px;
  margin: 1.6rem 0 1.2rem;
  background: #75b2ff;
}

.lab-hero__lead {
  max-width: 680px;
  margin: 0;
  color: #ffffff;
  font-size: 1.14rem;
  font-weight: 650;
  line-height: 1.6;
}

.lab-hero__description {
  max-width: 650px;
  margin: 1rem 0 0;
  color: #d3e0f2;
  font-size: 1rem;
  line-height: 1.8;
}

.lab-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 0.9rem;
  margin-top: 2rem;
}

.lab-button {
  display: inline-flex;
  min-height: 48px;
  align-items: center;
  justify-content: space-between;
  gap: 2rem;
  padding: 0.75rem 1.2rem;
  border: 1px solid transparent;
  border-radius: 3px;
  font-size: 0.9rem;
  font-weight: 650;
  transition:
    transform 160ms ease,
    background 160ms ease,
    border-color 160ms ease;
}

.lab-button:hover {
  transform: translateY(-2px);
}

.lab-button--light {
  color: #082a56 !important;
  background: #ffffff;
}

.lab-button--light:hover {
  background: #edf4ff;
}

.lab-button--outline {
  color: #ffffff !important;
  border-color: rgba(255, 255, 255, 0.68);
  background: rgba(255, 255, 255, 0.03);
}

.lab-button--outline:hover {
  border-color: #ffffff;
  background: rgba(255, 255, 255, 0.09);
}

/* =========================================================
   Scientific orbital visual
   ========================================================= */

.lab-visual {
  position: relative;
  width: min(420px, 100%);
  aspect-ratio: 1;
  margin: auto;
}

.lab-visual::before {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 82%;
  height: 45%;
  transform: translate(-50%, -50%) rotate(-22deg);
  border: 1px solid rgba(255, 255, 255, 0.17);
  border-radius: 50%;
  content: "";
}

.lab-visual::after {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 86%;
  height: 37%;
  transform: translate(-50%, -50%) rotate(44deg);
  border: 1px solid rgba(255, 255, 255, 0.12);
  border-radius: 50%;
  content: "";
}

.lab-orbit {
  position: absolute;
  border: 1px solid rgba(255, 255, 255, 0.22);
  border-radius: 50%;
}

.lab-orbit--outer {
  inset: 6%;
  border-style: dotted;
}

.lab-orbit--middle {
  inset: 20%;
}

.lab-orbit--inner {
  inset: 34%;
  border-style: dotted;
}

.lab-core {
  position: absolute;
  top: 50%;
  left: 50%;
  display: grid;
  width: 7.5rem;
  height: 7.5rem;
  place-items: center;
  transform: translate(-50%, -50%);
  border: 1px solid rgba(255, 255, 255, 0.58);
  border-radius: 50%;
  color: #ffffff;
  background: rgba(255, 255, 255, 0.06);
  box-shadow:
    0 0 55px rgba(146, 193, 255, 0.25),
    inset 0 0 30px rgba(255, 255, 255, 0.08);
  font-family: Georgia, "Times New Roman", serif;
  font-size: 4.1rem;
  font-weight: 400;
}

.lab-particle {
  position: absolute;
  width: 0.76rem;
  height: 0.76rem;
  border-radius: 50%;
  background: #ffffff;
  box-shadow:
    0 0 9px rgba(255, 255, 255, 0.95),
    0 0 25px rgba(125, 181, 255, 0.95);
}

.lab-particle--one {
  top: 8%;
  left: 39%;
}

.lab-particle--two {
  top: 31%;
  right: 7%;
}

.lab-particle--three {
  right: 34%;
  bottom: 6%;
}

.lab-particle--four {
  top: 57%;
  left: 7%;
  width: 0.48rem;
  height: 0.48rem;
}

.lab-stars {
  position: absolute;
  inset: 0;
  opacity: 0.5;
  background-image:
    radial-gradient(circle, #ffffff 1px, transparent 1.5px),
    radial-gradient(circle, #ffffff 1px, transparent 1.5px);
  background-position:
    0 0,
    22px 27px;
  background-size:
    48px 48px,
    61px 61px;
  -webkit-mask-image:
    radial-gradient(circle, #000 0%, transparent 72%);
  mask-image:
    radial-gradient(circle, #000 0%, transparent 72%);
}

/* =========================================================
   About
   ========================================================= */

.lab-about {
  padding: 4.2rem 0 3.8rem;
  border-bottom: 1px solid var(--line);
}

.lab-about__grid {
  display: grid;
  grid-template-columns:
    minmax(0, 1fr)
    minmax(340px, 0.95fr);
  gap: 7rem;
  align-items: start;
}

.lab-about h2 {
  max-width: 680px;
  margin: 0;
  color: var(--navy);
  font-size: clamp(2.2rem, 3.4vw, 3.45rem);
  line-height: 1.12;
}

.lab-about__content {
  padding-top: 0.35rem;
}

.lab-about__content p {
  margin: 0;
  color: var(--muted);
  font-size: 0.98rem;
  line-height: 1.85;
}

/* =========================================================
   Research
   ========================================================= */

.lab-research {
  padding: 3.5rem 0 4.2rem;
}

.lab-section-title {
  margin-bottom: 1.2rem;
}

.lab-section-title h2 {
  margin: 0;
  color: var(--navy);
  font-size: clamp(2rem, 3vw, 3.05rem);
  line-height: 1.15;
}

.lab-research__grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  margin-top: 0.2rem;
}

.lab-research-item {
  min-height: 210px;
  padding: 1.1rem 3.5rem 0 0;
}

.lab-research-item + .lab-research-item {
  padding-left: 3.5rem;
  border-left: 1px solid var(--line);
}

/* 01 / 02 / 03 */

.lab-research-item__number {
  display: block;
  margin-bottom: 0.9rem;
  color: var(--blue);
  font-size: 1.52rem;
  font-weight: 800;
  letter-spacing: 0.06em;
  line-height: 1.3;
}

.lab-research-item h3 {
  margin: 0 0 0.65rem;
  color: var(--navy);
  font-size: 1.16rem;
  line-height: 1.4;
}

.lab-research-item p {
  max-width: 350px;
  margin: 0;
  color: var(--muted);
  font-size: 0.93rem;
  line-height: 1.72;
}

.lab-research-item .lab-link {
  margin-top: 1.1rem;
}

/* =========================================================
   Team and publications
   ========================================================= */

.lab-information {
  background:
    linear-gradient(
      90deg,
      #f4f7fb 0%,
      #eef4fb 50%,
      #f5f8fc 100%
    );
}

.lab-information__grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.lab-information__item {
  min-height: 250px;
  padding: 3.2rem 4rem 3.2rem 0;
}

.lab-information__item + .lab-information__item {
  padding-right: 0;
  padding-left: 4rem;
  border-left: 1px solid #d8e1ed;
}

.lab-information h3 {
  margin: 0;
  color: var(--navy);
  font-size: clamp(1.65rem, 2.3vw, 2.25rem);
  line-height: 1.25;
}

.lab-information p {
  max-width: 530px;
  margin: 0.7rem 0 0;
  color: var(--muted);
  font-size: 0.94rem;
  line-height: 1.75;
}

/* =========================================================
   Join us
   ========================================================= */

.lab-join {
  margin: 0 !important;
  border: 0 !important;
  background: #ffffff;
}

.lab-join__grid {
  display: grid;
  grid-template-columns:
    minmax(300px, 0.85fr)
    minmax(390px, 1.05fr)
    auto;
  gap: 4rem;
  align-items: center;
  padding-top: 3.5rem;
  padding-bottom: 3.5rem;
}

.lab-join h2 {
  margin: 0;
  color: var(--navy);
  font-size: clamp(1.8rem, 2.7vw, 2.65rem);
  line-height: 1.2;
}

.lab-join__description {
  margin: 0;
  color: var(--muted);
  font-size: 0.94rem;
  line-height: 1.75;
}

.lab-join .lab-actions {
  flex-wrap: nowrap;
  justify-content: flex-end;
  margin: 0;
}

.lab-button--navy {
  color: #ffffff !important;
  border-color: var(--navy);
  background: var(--navy);
}

.lab-button--navy:hover {
  border-color: #064891;
  background: #064891;
}

.lab-button--border {
  color: var(--navy) !important;
  border-color: #8294aa;
  background: #ffffff;
}

.lab-button--border:hover {
  border-color: var(--navy);
  background: #f5f8fc;
}

/* =========================================================
   Original gray footer
   ========================================================= */

.page__footer {
  display: block !important;
  clear: both !important;
  position: relative !important;
  width: 100% !important;
  margin: 0 !important;
  padding: 0 !important;
  border-top: 1px solid #e1e5ea;
  background: #f2f3f3 !important;
}

.page__footer footer {
  width: min(1240px, calc(100% - 48px)) !important;
  max-width: none !important;
  margin: 0 auto !important;
  padding: 2.4rem 0 !important;
}

.page__footer-follow {
  margin: 0 0 1rem !important;
}

.page__footer-follow ul {
  margin: 0 !important;
  padding: 0 !important;
}

.page__footer-follow li {
  color: #7c8796;
}

.page__footer-follow a,
.page__footer-copyright,
.page__footer-copyright a {
  color: #7c8796 !important;
}

.page__footer-follow a:hover,
.page__footer-copyright a:hover {
  color: #005ee8 !important;
}

.page__footer-copyright {
  margin: 1rem 0 0 !important;
  font-size: 0.86rem;
  line-height: 1.7;
}

body {
  padding-bottom: 0 !important;
}

/* =========================================================
   Responsive layout
   ========================================================= */

@media (max-width: 1050px) {
  .lab-hero__inner {
    grid-template-columns:
      minmax(0, 1.1fr)
      minmax(280px, 0.9fr);
    gap: 2.5rem;
  }

  .lab-hero h1 {
    font-size: clamp(3.4rem, 6.4vw, 5rem);
  }

  .lab-about__grid {
    gap: 3.5rem;
  }

  .lab-research-item {
    padding-right: 2rem;
  }

  .lab-research-item + .lab-research-item {
    padding-left: 2rem;
  }

  .lab-information__item {
    padding-right: 2.5rem;
  }

  .lab-information__item + .lab-information__item {
    padding-left: 2.5rem;
  }

  .lab-join__grid {
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }

  .lab-join .lab-actions {
    grid-column: 1 / -1;
    justify-content: flex-start;
  }
}

@media (max-width: 800px) {
  .lab-container {
    width: min(1240px, calc(100% - 32px));
  }

  .lab-hero__inner {
    min-height: auto;
    grid-template-columns: 1fr;
    padding-top: 4rem;
    padding-bottom: 3.5rem;
  }

  .lab-visual {
    width: min(340px, 80%);
  }

  .lab-about__grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }

  .lab-research__grid {
    grid-template-columns: 1fr;
  }

  .lab-research-item,
  .lab-research-item + .lab-research-item {
    min-height: auto;
    padding: 1.8rem 0;
    border-left: 0;
    border-top: 1px solid var(--line);
  }

  .lab-information__grid {
    grid-template-columns: 1fr;
  }

  .lab-information__item,
  .lab-information__item + .lab-information__item {
    min-height: auto;
    padding: 2.8rem 0;
    border-left: 0;
  }

  .lab-information__item + .lab-information__item {
    border-top: 1px solid #d8e1ed;
  }

  .lab-join__grid {
    grid-template-columns: 1fr;
    gap: 1.3rem;
  }

  .lab-join .lab-actions {
    grid-column: auto;
  }

  .page__footer footer {
    width: calc(100% - 32px) !important;
  }
}

@media (max-width: 520px) {
  .lab-container {
    width: calc(100% - 24px);
  }

  .lab-hero h1 {
    font-size: 3.1rem;
  }

  .lab-hero__description {
    font-size: 0.94rem;
  }

  .lab-visual {
    width: 240px;
  }

  .lab-core {
    width: 5.5rem;
    height: 5.5rem;
    font-size: 3rem;
  }

  .lab-actions,
  .lab-join .lab-actions {
    align-items: stretch;
    flex-direction: column;
  }

  .lab-button {
    width: 100%;
  }

  .lab-about {
    padding-top: 3rem;
  }

  .lab-about h2 {
    font-size: 2.15rem;
  }

  .page__footer footer {
    width: calc(100% - 24px) !important;
    padding-top: 2rem !important;
    padding-bottom: 2rem !important;
  }
}

/* =========================================================
   High-priority label overrides
   ========================================================= */

/*
  Academic Pages 会为正文中的 p 标签设置默认字号。
  使用高优先级选择器和 !important，确保标签字号生效。
*/

.page__content p.lab-label {
  max-width: 100% !important;
  margin: 0 0 1.15rem !important;
  color: var(--blue) !important;
  font-size: 1.34rem !important;
  font-weight: 800 !important;
  letter-spacing: 0.035em !important;
  line-height: 1 !important;
  overflow-wrap: anywhere !important;
  text-transform: uppercase !important;
}

/* 01 / 02 / 03 保持为 1.52rem */

.page__content .lab-research-item__number {
  font-size: 1.52rem !important;
}

/* Tablet */

@media (max-width: 800px) {
  .page__content p.lab-label {
    font-size: 2.5rem !important;
  }
}

/* Mobile：仍保持为数字的约两倍 */

@media (max-width: 520px) {
  .page__content p.lab-label {
    font-size: 2.5rem !important;
    line-height: 1 !important;
  }

  .page__content .lab-research-item__number {
    font-size: 1.25rem !important;
  }
}
</style>

<div class="lab-home">

  <!-- Hero -->
  <section class="lab-hero">
    <div class="lab-container lab-hero__inner">

      <div class="lab-hero__content">

        <p class="lab-hero__institution">
          HFNL · University of Science and Technology of China
        </p>

        <h1 class="lab-display">
          QuantumICT<br>
          Research Group
        </h1>

        <div class="lab-hero__accent"></div>

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
            class="lab-button lab-button--light"
            href="{{ '/research/' | relative_url }}"
          >
            <span>Explore Our Research</span>
            <span aria-hidden="true">→</span>
          </a>

          <a
            class="lab-button lab-button--outline"
            href="{{ '/people/' | relative_url }}"
          >
            <span>Meet the Group</span>
            <span aria-hidden="true">→</span>
          </a>

        </div>
      </div>

      <div class="lab-visual" aria-hidden="true">

        <div class="lab-stars"></div>

        <div class="lab-orbit lab-orbit--outer"></div>
        <div class="lab-orbit lab-orbit--middle"></div>
        <div class="lab-orbit lab-orbit--inner"></div>

        <div class="lab-core">Q</div>

        <div class="lab-particle lab-particle--one"></div>
        <div class="lab-particle lab-particle--two"></div>
        <div class="lab-particle lab-particle--three"></div>
        <div class="lab-particle lab-particle--four"></div>

      </div>

    </div>
  </section>

  <!-- About -->
  <section class="lab-about">
    <div class="lab-container lab-about__grid">

      <div>
        <p class="lab-label">About Us</p>

        <h2 class="lab-display">
          Developing computational tools to understand complex
          scientific systems.
        </h2>
      </div>

      <div class="lab-about__content">

        <p>
          QuantumICT is a research group at HFNL and USTC. Our work
          focuses on developing efficient computational methods and
          applying them to scientific problems across multiple time
          and length scales.
        </p>

        <a
          class="lab-link"
          href="{{ '/research/' | relative_url }}"
        >
          <span>Discover our research</span>
          <span aria-hidden="true">→</span>
        </a>

      </div>

    </div>
  </section>

  <!-- Research -->
  <section class="lab-research">
    <div class="lab-container">

      <div class="lab-section-title">

        <p class="lab-label">Research</p>

        <h2 class="lab-display">
          Our main research directions
        </h2>

      </div>

      <div class="lab-research__grid">

        <article class="lab-research-item">

          <span class="lab-research-item__number">01</span>

          <h3>High-Performance Computing</h3>

          <p>
            Efficient algorithms and large-scale computational
            approaches for scientific simulations and
            data-intensive research.
          </p>

          <a
            class="lab-link"
            href="{{ '/research/' | relative_url }}"
          >
            <span>Learn more</span>
            <span aria-hidden="true">→</span>
          </a>

        </article>

        <article class="lab-research-item">

          <span class="lab-research-item__number">02</span>

          <h3>First-Principles Methods</h3>

          <p>
            Development and implementation of atomistic methods
            based on fundamental physical principles.
          </p>

          <a
            class="lab-link"
            href="{{ '/research/' | relative_url }}"
          >
            <span>Learn more</span>
            <span aria-hidden="true">→</span>
          </a>

        </article>

        <article class="lab-research-item">

          <span class="lab-research-item__number">03</span>

          <h3>Kinetic Monte Carlo</h3>

          <p>
            Computational methods for investigating dynamic
            processes over extended time scales.
          </p>

          <a
            class="lab-link"
            href="{{ '/research/' | relative_url }}"
          >
            <span>Learn more</span>
            <span aria-hidden="true">→</span>
          </a>

        </article>

      </div>
    </div>
  </section>

  <!-- Team and publications -->
  <section class="lab-information">
    <div class="lab-container lab-information__grid">

      <div class="lab-information__item">

        <p class="lab-label">Our Team</p>

        <h3 class="lab-display">
          Researchers working across computation and physical science
        </h3>

        <p>
          Learn more about the principal investigator,
          current students, and alumni of the group.
        </p>

        <a
          class="lab-link"
          href="{{ '/people/' | relative_url }}"
        >
          <span>View all members</span>
          <span aria-hidden="true">→</span>
        </a>

      </div>

      <div class="lab-information__item">

        <p class="lab-label">Publications</p>

        <h3 class="lab-display">
          Explore our research output
        </h3>

        <p>
          Browse publications covering method development,
          high-performance simulation, and scientific applications.
        </p>

        <a
          class="lab-link"
          href="{{ '/publications/' | relative_url }}"
        >
          <span>View publications</span>
          <span aria-hidden="true">→</span>
        </a>

      </div>

    </div>
  </section>

  <!-- Join us -->
  <section class="lab-join">
    <div class="lab-container lab-join__grid">

      <div>

        <p class="lab-label">Join Us</p>

        <h2 class="lab-display">
          Work with the QuantumICT Group.
        </h2>

      </div>

      <p class="lab-join__description">
        We welcome motivated students and researchers interested
        in computational science, high-performance simulation,
        and scientific method development.
      </p>

      <div class="lab-actions">

        <a
          class="lab-button lab-button--navy"
          href="{{ '/join-us/' | relative_url }}"
        >
          <span>Opportunities</span>
          <span aria-hidden="true">→</span>
        </a>

        <a
          class="lab-button lab-button--border"
          href="mailto:shh@ustc.edu.cn"
        >
          <span>Contact Us</span>
          <span aria-hidden="true">→</span>
        </a>

      </div>

    </div>
  </section>

</div>
