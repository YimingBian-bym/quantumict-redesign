---
permalink: /people/
title: "People"
author_profile: false
classes: wide
toc: false
---

<style>
/*
  People page:
  A wide, text-first layout that keeps the Academic Pages / Markdown style.
*/

.people-simple {
  max-width: 1080px;
  margin: 0 auto;
  color: #243247;
}

.people-simple .people-intro {
  max-width: 900px;
  margin: 0 0 3.2rem;
  color: #56657a;
  font-size: 1.08rem;
  line-height: 1.85;
}

.people-simple h2 {
  margin-top: 3.8rem;
  margin-bottom: 0;
  padding-bottom: 0.7rem;
  color: #17355f;
  font-size: 1.72rem;
  font-weight: 650;
  letter-spacing: -0.02em;
  border-bottom: 1px solid #d9e1eb;
}

.people-simple a {
  color: #1f5fa9;
  text-decoration: none;
}

.people-simple a:hover {
  text-decoration: underline;
  text-underline-offset: 0.18em;
}

/* Principal investigator */

.people-lead {
  display: grid;
  grid-template-columns: minmax(210px, 0.62fr) minmax(0, 1.38fr);
  gap: clamp(3rem, 7vw, 6rem);
  align-items: start;
  padding: 2rem 0 2.4rem;
  border-bottom: 1px solid #e3e8ef;
}

.people-lead__profile {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  min-width: 0;
}

.people-lead__photo {
  display: block;
  width: 180px;
  height: 225px;
  margin: 0 0 1.35rem;
  object-fit: cover;
  object-position: center top;
  border-radius: 2px;
  background: #edf1f5;
}

.people-lead__name {
  margin: 0;
  color: #1b3d6b;
  font-size: 1.55rem;
  font-weight: 650;
  line-height: 1.3;
}

.people-lead__meta {
  margin: 0.7rem 0 0;
  padding: 0;
  list-style: none;
}

.people-lead__meta li {
  margin: 0 0 0.42rem;
  color: #6a778a;
  font-size: 0.92rem;
  line-height: 1.5;
}

.people-lead__email {
  color: #4e5f75;
  white-space: nowrap;
}

.people-lead__details {
  color: #56657a;
  font-size: 1rem;
  line-height: 1.78;
}

.people-lead__details p {
  margin: 0 0 0.8rem;
}

.people-lead__links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.65rem 1.4rem;
  margin-top: 1.2rem;
}

.people-lead__links a {
  font-size: 0.94rem;
  font-weight: 620;
}

/* Member rows */

.people-list {
  margin: 0;
  padding: 0;
  list-style: none;
}

.people-row {
  display: grid;
  grid-template-columns: minmax(220px, 0.9fr) minmax(180px, 0.7fr) minmax(0, 1fr);
  gap: 1.5rem;
  align-items: center;
  min-height: 76px;
  padding: 1.15rem 0;
  border-bottom: 1px solid #e3e8ef;
}

.people-row__name {
  color: #1b3d6b;
  font-size: 1.08rem;
  font-weight: 650;
  line-height: 1.45;
}

.people-row__role {
  color: #637188;
  font-size: 0.96rem;
  line-height: 1.5;
}

.people-row__meta {
  color: #7a8798;
  font-size: 0.92rem;
  line-height: 1.55;
  text-align: right;
}

.people-row__link {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  font-weight: 620;
}

.people-row__link::after {
  content: "→";
  color: #7193bd;
  font-size: 0.9em;
}

/* Alumni */

.people-alumni .people-row {
  grid-template-columns: minmax(220px, 0.8fr) minmax(170px, 0.55fr) minmax(0, 1.15fr);
}

.people-empty {
  color: #8a95a4;
}

@media (max-width: 760px) {
  .people-simple {
    max-width: 100%;
  }

  .people-simple .people-intro {
    margin-bottom: 2.4rem;
  }

  .people-simple h2 {
    margin-top: 3rem;
    font-size: 1.48rem;
  }

  .people-lead {
    grid-template-columns: 1fr;
    gap: 1.8rem;
  }

  .people-lead__profile {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }

  .people-lead__photo {
    width: 150px;
    height: 188px;
    margin-bottom: 1.15rem;
  }

  .people-row,
  .people-alumni .people-row {
    grid-template-columns: 1fr;
    gap: 0.3rem;
    min-height: 0;
    padding: 1.25rem 0;
  }

  .people-row__meta {
    text-align: left;
  }
}
</style>

<div class="people-simple">

<p class="people-intro">
QuantumICT is a research group working on high-performance scientific computing,
first-principles methods, kinetic simulation, quantum algorithms, and related
computational approaches.
</p>

<h2>Principal Investigator</h2>

<section class="people-lead">
  <div class="people-lead__profile">
    <img
      class="people-lead__photo"
      src="{{ '/images/people/honghui-shang.jpg' | relative_url }}"
      alt="Honghui Shang"
    >

    <div>
      <h3 class="people-lead__name">
        <a href="https://shanghui.github.io/">Honghui Shang</a>
      </h3>

      <ul class="people-lead__meta">
        <li>Professor at USTC</li>
        <li>Hefei, China</li>
        <li class="people-lead__email">shh@ustc.edu.cn</li>
        <li><a href="https://orcid.org/0000-0003-4957-4251">ORCID</a></li>
      </ul>
    </div>
  </div>

  <div class="people-lead__details">
    <p>
      Professor at the University of Science and Technology of China.
      Her research focuses on physical algorithms and numerical methods for
      scientific computing, including quantum algorithms, artificial intelligence,
      first-principles methods, and high-performance computing.
    </p>

    <div class="people-lead__links">
      <a href="https://shanghui.github.io/">Personal Website</a>
      <a href="https://scholar.google.com/citations?hl=zh-CN&amp;user=HBY4LJ8AAAAJ">Google Scholar</a>
      <a href="https://faculty.ustc.edu.cn/shanghonghui/en/index.htm">USTC Faculty Profile</a>
    </div>
  </div>
</section>

<h2>Current Members</h2>

<ul class="people-list">
  <li class="people-row">
    <div class="people-row__name">
      <a class="people-row__link" href="{{ '/members/kanbowen' | relative_url }}">Bowen Kan</a>
    </div>
    <div class="people-row__role">Doctoral Student</div>
    <div class="people-row__meta">Member profile</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">
      <a class="people-row__link" href="{{ '/members/zhaobowen' | relative_url }}">Bowen Zhao</a>
    </div>
    <div class="people-row__role">Master's Student</div>
    <div class="people-row__meta">Member profile</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Daiyou Xie</div>
    <div class="people-row__role">Doctoral Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Jiexuan Zhou</div>
    <div class="people-row__role">Master's Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Leilei Zhu</div>
    <div class="people-row__role">Doctoral Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Pengyu Zhou</div>
    <div class="people-row__role">Master's Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">
      <a class="people-row__link" href="{{ '/members/xuzhiqian' | relative_url }}">Zhiqian Xu</a>
    </div>
    <div class="people-row__role">Doctoral Student</div>
    <div class="people-row__meta">Member profile</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">
      <a class="people-row__link" href="https://xiazhuozhao.com/">Zhuozhao Xia</a>
    </div>
    <div class="people-row__role">Master's Student</div>
    <div class="people-row__meta">Personal website</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Shitian Wan</div>
    <div class="people-row__role">Master's Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Yumeng Zhou</div>
    <div class="people-row__role">Doctoral Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Yimang Chen</div>
    <div class="people-row__role">Master's Student</div>
    <div class="people-row__meta people-empty">—</div>
  </li>
</ul>

<h2>Previous Members</h2>

<ul class="people-list people-alumni">
  <li class="people-row">
    <div class="people-row__name">Haiwen Luo</div>
    <div class="people-row__role">Master, 2023</div>
    <div class="people-row__meta">National Supercomputer Center in Wuxi</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Yangjun Wu</div>
    <div class="people-row__role">Master, 2024</div>
    <div class="people-row__meta">ByteDance</div>
  </li>

  <li class="people-row">
    <div class="people-row__name">Yingxiang Gao</div>
    <div class="people-row__role">Graduated</div>
    <div class="people-row__meta people-empty">—</div>
  </li>
</ul>

</div>
