---
permalink: /join-us/
title: "Join Us"
author_profile: false
classes: wide
toc: false
---

<style>
/*
  Join Us page:
  A clear, text-first recruitment page consistent with Research,
  People, and Publications.
*/

.join-simple {
  max-width: 1080px;
  margin: 0 auto;
  color: #243247;
}

.join-intro {
  max-width: 900px;
  margin: 0 0 3.2rem;
  color: #56657a;
  font-size: 1.08rem;
  line-height: 1.85;
}

.join-simple h2 {
  margin: 4rem 0 0;
  padding-bottom: 0.72rem;
  color: #17355f;
  font-size: 1.72rem;
  font-weight: 650;
  line-height: 1.25;
  letter-spacing: -0.02em;
  border-bottom: 1px solid #d9e1eb;
}

.join-section-copy {
  max-width: 920px;
  margin: 1.5rem 0 0;
  color: #59687c;
  font-size: 1rem;
  line-height: 1.82;
}

.join-simple a {
  color: #1f5fa9;
  text-decoration: none;
}

.join-simple a:hover {
  text-decoration: underline;
  text-underline-offset: 0.18em;
}

/* Open positions */

.join-opportunities {
  margin: 0;
  padding: 0;
  list-style: none;
}

.join-opportunity {
  display: grid;
  grid-template-columns: minmax(210px, 0.62fr) minmax(0, 1.38fr);
  gap: clamp(2rem, 5vw, 4.5rem);
  padding: 1.6rem 0;
  border-bottom: 1px solid #e3e8ef;
}

.join-opportunity__title {
  color: #1b3d6b;
  font-size: 1.08rem;
  font-weight: 660;
  line-height: 1.5;
}

.join-opportunity__text {
  margin: 0;
  color: #637188;
  font-size: 0.97rem;
  line-height: 1.75;
}

/* Research areas */

.join-research-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  column-gap: clamp(2.5rem, 6vw, 5rem);
  margin: 0;
  padding: 0;
  list-style: none;
}

.join-research-item {
  padding: 1.45rem 0;
  border-bottom: 1px solid #e3e8ef;
}

.join-research-item__title {
  margin: 0;
  color: #1b3d6b;
  font-size: 1.04rem;
  font-weight: 660;
  line-height: 1.5;
}

.join-research-item__text {
  margin: 0.4rem 0 0;
  color: #6a778a;
  font-size: 0.93rem;
  line-height: 1.68;
}

/* Backgrounds and application materials */

.join-detail-list {
  margin: 1.25rem 0 0;
  padding: 0;
  list-style: none;
}

.join-detail-row {
  display: grid;
  grid-template-columns: minmax(220px, 0.72fr) minmax(0, 1.28fr);
  gap: clamp(2rem, 5vw, 4.5rem);
  padding: 1.25rem 0;
  border-bottom: 1px solid #e3e8ef;
}

.join-detail-row__label {
  color: #425873;
  font-size: 0.98rem;
  font-weight: 650;
  line-height: 1.55;
}

.join-detail-row__text {
  margin: 0;
  color: #66758a;
  font-size: 0.96rem;
  line-height: 1.7;
}

/* Contact */

.join-contact {
  display: grid;
  grid-template-columns: minmax(210px, 0.62fr) minmax(0, 1.38fr);
  gap: clamp(2.5rem, 6vw, 5rem);
  margin: 1.8rem 0 0;
  padding: 1.7rem 1.8rem;
  border-left: 3px solid #8faecc;
  background: #f5f7fa;
}

.join-contact__name {
  margin: 0;
  color: #1b3d6b;
  font-size: 1.18rem;
  font-weight: 680;
  line-height: 1.4;
}

.join-contact__position {
  margin: 0.45rem 0 0;
  color: #68768a;
  font-size: 0.92rem;
  line-height: 1.6;
}

.join-contact__details {
  color: #56657a;
  font-size: 0.97rem;
  line-height: 1.75;
}

.join-contact__details p {
  margin: 0 0 0.65rem;
}

.join-contact__email {
  color: #33465f;
  font-weight: 650;
  white-space: nowrap;
}

.join-contact__links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem 1.35rem;
  margin-top: 1rem;
}

.join-contact__links a {
  font-size: 0.91rem;
  font-weight: 640;
}

@media (max-width: 760px) {
  .join-intro {
    margin-bottom: 2.5rem;
  }

  .join-simple h2 {
    margin-top: 3.2rem;
    font-size: 1.48rem;
  }

  .join-opportunity,
  .join-detail-row,
  .join-contact {
    grid-template-columns: 1fr;
    gap: 0.55rem;
  }

  .join-research-list {
    grid-template-columns: 1fr;
  }

  .join-contact {
    gap: 1.25rem;
    padding: 1.45rem;
  }
}
</style>

<div class="join-simple">

<p class="join-intro">
We welcome motivated students and postdoctoral researchers who are interested
in scientific computing, quantum chemistry, and the development and application
of computational methods and scientific software.
</p>

<h2>Open Opportunities</h2>

<ul class="join-opportunities">
  <li class="join-opportunity">
    <div class="join-opportunity__title">Graduate Students</div>
    <p class="join-opportunity__text">
      We welcome students who would like to work on physical algorithms,
      numerical methods, scientific software, and large-scale computational
      applications.
    </p>
  </li>

  <li class="join-opportunity">
    <div class="join-opportunity__title">Postdoctoral Researchers</div>
    <p class="join-opportunity__text">
      We welcome postdoctoral applicants interested in developing new
      computational methods and applying them to challenging problems in
      physics, chemistry, and materials science.
    </p>
  </li>
</ul>

<h2>Research Areas</h2>

<p class="join-section-copy">
Prospective members may work across one or more of the group's current research
directions.
</p>

<ul class="join-research-list">
  <li class="join-research-item">
    <h3 class="join-research-item__title">High-Performance Scientific Computing</h3>
    <p class="join-research-item__text">
      Scalable algorithms, parallel software, and large-scale simulations on
      modern high-performance computing systems.
    </p>
  </li>

  <li class="join-research-item">
    <h3 class="join-research-item__title">First-Principles Methods</h3>
    <p class="join-research-item__text">
      Electronic-structure methods, density-functional perturbation theory,
      molecular and materials simulations, and related numerical techniques.
    </p>
  </li>

  <li class="join-research-item">
    <h3 class="join-research-item__title">Quantum Algorithms and Neural-Network Quantum States</h3>
    <p class="join-research-item__text">
      Quantum computational chemistry, tensor-network methods, generative
      models, and machine-learning approaches to many-electron problems.
    </p>
  </li>

  <li class="join-research-item">
    <h3 class="join-research-item__title">Kinetic and Multiscale Simulation</h3>
    <p class="join-research-item__text">
      Kinetic Monte Carlo, atomistic simulation, machine-learning potentials,
      and multiscale methods for complex physical processes.
    </p>
  </li>
</ul>

<h2>Who Should Apply</h2>

<p class="join-section-copy">
Applicants with strong training in one or more of the following areas are
especially encouraged to contact us.
</p>

<ul class="join-detail-list">
  <li class="join-detail-row">
    <div class="join-detail-row__label">Physical Chemistry</div>
    <p class="join-detail-row__text">
      Electronic structure, quantum chemistry, spectroscopy, or molecular and
      materials simulation.
    </p>
  </li>

  <li class="join-detail-row">
    <div class="join-detail-row__label">Computational Physics</div>
    <p class="join-detail-row__text">
      Numerical simulation, quantum many-body methods, statistical mechanics,
      or computational materials science.
    </p>
  </li>

  <li class="join-detail-row">
    <div class="join-detail-row__label">Applied Mathematics</div>
    <p class="join-detail-row__text">
      Numerical analysis, optimization, scientific machine learning, or
      large-scale computational methods.
    </p>
  </li>

  <li class="join-detail-row">
    <div class="join-detail-row__label">Computer Science</div>
    <p class="join-detail-row__text">
      High-performance computing, parallel programming, scientific software,
      machine learning, or algorithm development.
    </p>
  </li>
</ul>

<h2>How to Apply</h2>

<p class="join-section-copy">
Please contact Honghui Shang by email and include the following materials:
</p>

<ul class="join-detail-list">
  <li class="join-detail-row">
    <div class="join-detail-row__label">Curriculum Vitae</div>
    <p class="join-detail-row__text">
      A current CV summarizing your education, research experience, projects,
      publications, and relevant technical background.
    </p>
  </li>

  <li class="join-detail-row">
    <div class="join-detail-row__label">Research Skills</div>
    <p class="join-detail-row__text">
      A brief description of your research experience, computational skills,
      and the methods or scientific problems that interest you.
    </p>
  </li>
</ul>

<h2>Contact</h2>

<section class="join-contact">
  <div>
    <h3 class="join-contact__name">Honghui Shang</h3>
    <p class="join-contact__position">
      Professor<br>
      University of Science and Technology of China<br>
      Hefei, China
    </p>
  </div>

  <div class="join-contact__details">
    <p>
      Please send your application materials and a brief introduction to:
    </p>

    <p class="join-contact__email">shh@ustc.edu.cn</p>

    <div class="join-contact__links">
      <a href="https://shanghui.github.io/">Personal Website</a>
      <a href="https://faculty.ustc.edu.cn/shanghonghui/en/index.htm">USTC Faculty Profile</a>
      <a href="{{ '/research/' | relative_url }}">Research</a>
      <a href="{{ '/people/' | relative_url }}">People</a>
    </div>
  </div>
</section>

</div>
