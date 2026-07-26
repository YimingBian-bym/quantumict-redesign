---
permalink: /news/
title: "News"
author_profile: false
classes: wide
toc: false
---

<style>
/*
  News page:
  A chronological, text-first archive consistent with the other redesigned pages.
*/

.news-simple {
  max-width: 1080px;
  margin: 0 auto;
  color: #243247;
}

.news-intro {
  max-width: 880px;
  margin: 0 0 3.4rem;
  color: #56657a;
  font-size: 1.08rem;
  line-height: 1.85;
}

.news-year {
  margin: 4rem 0 0;
  padding-bottom: 0.72rem;
  color: #17355f;
  font-size: 1.72rem;
  font-weight: 650;
  line-height: 1.25;
  letter-spacing: -0.02em;
  border-bottom: 1px solid #d9e1eb;
}

.news-list {
  margin: 0;
  padding: 0;
  list-style: none;
}

.news-item {
  display: grid;
  grid-template-columns: minmax(105px, 0.22fr) minmax(0, 1.78fr);
  gap: clamp(1.8rem, 5vw, 4.5rem);
  padding: 1.65rem 0 1.75rem;
  border-bottom: 1px solid #e3e8ef;
}

.news-date {
  padding-top: 0.12rem;
}

.news-date__month {
  display: block;
  color: #1f5fa9;
  font-size: 0.82rem;
  font-weight: 720;
  line-height: 1.3;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.news-date__day {
  display: block;
  margin-top: 0.12rem;
  color: #536983;
  font-size: 1.48rem;
  font-weight: 660;
  line-height: 1.15;
}

.news-type {
  display: inline-block;
  margin: 0 0 0.48rem;
  color: #78869a;
  font-size: 0.76rem;
  font-weight: 720;
  line-height: 1.3;
  letter-spacing: 0.09em;
  text-transform: uppercase;
}

.news-title {
  max-width: 900px;
  margin: 0;
  color: #1b3d6b;
  font-size: 1.16rem;
  font-weight: 660;
  line-height: 1.5;
}

.news-title a {
  color: inherit;
  text-decoration: none;
}

.news-title a:hover {
  color: #1f5fa9;
  text-decoration: underline;
  text-underline-offset: 0.18em;
}

.news-excerpt {
  max-width: 900px;
  margin: 0.52rem 0 0;
  color: #637188;
  font-size: 0.96rem;
  line-height: 1.75;
}

.news-more {
  display: inline-block;
  margin-top: 0.8rem;
  color: #1f5fa9;
  font-size: 0.88rem;
  font-weight: 660;
  text-decoration: none;
}

.news-more:hover {
  text-decoration: underline;
  text-underline-offset: 0.18em;
}

.news-empty {
  margin-top: 2rem;
  color: #7a8798;
  font-size: 0.98rem;
}

@media (max-width: 680px) {
  .news-intro {
    margin-bottom: 2.7rem;
  }

  .news-year {
    margin-top: 3.2rem;
    font-size: 1.48rem;
  }

  .news-item {
    grid-template-columns: 1fr;
    gap: 0.75rem;
    padding: 1.4rem 0 1.5rem;
  }

  .news-date {
    display: flex;
    align-items: baseline;
    gap: 0.38rem;
  }

  .news-date__day {
    margin-top: 0;
    font-size: 0.92rem;
  }
}
</style>

<div class="news-simple">

<p class="news-intro">
Selected updates from QuantumICT, including research highlights, publications,
awards, conferences, and group activities.
</p>

{% assign current_year = "" %}
{% assign news_count = 0 %}

{% for post in site.posts %}
  {% if post.categories contains "news" %}
    {% assign news_count = news_count | plus: 1 %}
    {% assign post_year = post.date | date: "%Y" %}

    {% if post_year != current_year %}
      {% unless current_year == "" %}
        </ul>
      {% endunless %}

      <h2 class="news-year">{{ post_year }}</h2>
      <ul class="news-list">
      {% assign current_year = post_year %}
    {% endif %}

    <li class="news-item">
      <time class="news-date" datetime="{{ post.date | date_to_xmlschema }}">
        <span class="news-date__month">{{ post.date | date: "%b" }}</span>
        <span class="news-date__day">{{ post.date | date: "%d" }}</span>
      </time>

      <article>
        <span class="news-type">{{ post.news_type | default: "Update" }}</span>

        <h3 class="news-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>

        {% if post.excerpt %}
          <p class="news-excerpt">{{ post.excerpt | strip_html | strip_newlines }}</p>
        {% endif %}

        <a class="news-more" href="{{ post.url | relative_url }}">Read more →</a>
      </article>
    </li>
  {% endif %}
{% endfor %}

{% unless current_year == "" %}
  </ul>
{% endunless %}

{% if news_count == 0 %}
  <p class="news-empty">News updates will be added here.</p>
{% endif %}

</div>
