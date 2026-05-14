---
layout: page
title: research
permalink: /research/
nav: true
nav_order: 2
---

My work sits at the intersection of computing education, computational thinking, and the role of generative AI in learning and teaching. I am particularly interested in how students develop problem-solving skills, how AI tools are perceived and used in educational settings, and how computing education research can better reflect the diversity of global contexts — including Latin America.

<link href="https://fonts.googleapis.com/css2?family=Source+Serif+4:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  .rl-wrap { font-family: 'DM Sans', sans-serif; margin: 2rem 0; }
  .rl-slide {
    background: #faf9f6;
    border-radius: 4px;
    box-shadow: 0 4px 24px rgba(0,0,0,0.10), 0 1px 4px rgba(0,0,0,0.05);
    padding: 40px 48px 44px;
    position: relative;
    overflow: hidden;
  }
  .rl-slide::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: linear-gradient(90deg, #4a7c59, #7bab8b, #c4d8c0);
  }
  .rl-slide h2 {
    font-family: 'Source Serif 4', serif;
    font-weight: 300;
    font-size: 1.45rem;
    color: #2d2d2d;
    letter-spacing: -0.01em;
    margin-bottom: 8px;
    border: none;
    padding: 0;
  }
  .rl-divider {
    height: 1px;
    background: linear-gradient(90deg, #b0c4b1 0%, transparent 80%);
    margin-bottom: 28px;
  }
  .rl-banner {
    background: #ddeadc;
    border: 1.5px solid #b0c9ae;
    border-radius: 3px;
    text-align: center;
    padding: 16px 20px;
    margin-bottom: 14px;
  }
  .rl-banner-text {
    font-family: 'Source Serif 4', serif;
    font-size: 1rem;
    font-weight: 400;
    color: #2e4a32;
    line-height: 1.55;
  }
  .rl-areas-row {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr auto;
    gap: 12px;
    margin-bottom: 28px;
    align-items: stretch;
  }
  @media (max-width: 640px) {
    .rl-areas-row { grid-template-columns: 1fr 1fr; }
    .rl-side-box  { width: auto; }
  }
  .rl-focus-box {
    background: #f3f7f2;
    border: 1.5px solid #b0c9ae;
    border-radius: 3px;
    text-align: center;
    padding: 12px 10px;
  }
  .rl-side-box {
    background: #f9f7f3;
    border: 1px dashed #d9c99a;
    border-radius: 3px;
    text-align: center;
    padding: 10px;
    width: 88px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    opacity: 0.75;
  }
  .rl-box-label {
    font-size: 0.65rem;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 0.07em;
    margin-bottom: 5px;
  }
  .rl-focus-box .rl-box-label { color: #4a7c59; }
  .rl-side-box  .rl-box-label { color: #a08840; font-size: 0.58rem; }
  .rl-box-title { font-size: 0.84rem; line-height: 1.4; font-weight: 400; }
  .rl-focus-box .rl-box-title { color: #2e4a32; }
  .rl-side-box  .rl-box-title { color: #7a6535; font-size: 0.74rem; }
  .rl-side-note { font-size: 0.7rem; opacity: 0.65; display: block; margin-top: 3px; }
  .rl-questions { text-align: center; }
  .rl-questions-title { font-weight: 500; font-size: 0.85rem; color: #2d2d2d; margin-bottom: 14px; }
  .rl-q-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px 32px;
    text-align: left;
  }
  @media (max-width: 560px) { .rl-q-grid { grid-template-columns: 1fr; } }
  .rl-q-item { padding-left: 10px; border-left: 2px solid #c4d8c0; }
  .rl-q-main {
    font-family: 'Source Serif 4', serif;
    font-style: italic;
    font-size: 0.83rem;
    color: #2d2d2d;
    margin-bottom: 2px;
    line-height: 1.45;
  }
  .rl-q-sub { font-size: 0.73rem; color: #888; }
</style>

<div class="rl-wrap">
  <div class="rl-slide">
    <h2>Research lines</h2>
    <div class="rl-divider"></div>
    <div class="rl-banner">
      <div class="rl-banner-text">
        Computational Thinking &amp; Generative AI<br>
        in Computing Education
      </div>
    </div>
    <div class="rl-areas-row">
      <div class="rl-focus-box">
        <div class="rl-box-label">Focus area</div>
        <div class="rl-box-title">Problem-Solving<br>&amp; CT Skills</div>
      </div>
      <div class="rl-focus-box">
        <div class="rl-box-label">Focus area</div>
        <div class="rl-box-title">GenAI Tools &amp; Perceptions</div>
      </div>
      <div class="rl-focus-box">
        <div class="rl-box-label">Focus area</div>
        <div class="rl-box-title">Equity &amp; Access<br>in Latam CER</div>
      </div>
      <div class="rl-side-box">
        <div class="rl-box-label">Side area</div>
        <div class="rl-box-title">AI in Education<span class="rl-side-note">(broader)</span></div>
      </div>
    </div>
    <div class="rl-questions">
      <div class="rl-questions-title">Overarching questions:</div>
      <div class="rl-q-grid">
        <div class="rl-q-item">
          <div class="rl-q-main">How to support students in solving computational problems?</div>
          <div class="rl-q-sub">(CT skills, problem-solving strategies, tools)</div>
        </div>
        <div class="rl-q-item">
          <div class="rl-q-main">What are the perceptions and use of GenAI among educators and students?</div>
          <div class="rl-q-sub">(across educational levels)</div>
        </div>
        <div class="rl-q-item">
          <div class="rl-q-main">Can GenAI-powered tools support learning and teaching, and how?</div>
          <div class="rl-q-sub">(human-centered design, evidence-based practices)</div>
        </div>
        <div class="rl-q-item">
          <div class="rl-q-main">What is the role of Latin America in CEd research and how to increase its participation?</div>
          <div class="rl-q-sub">(equity, global participation)</div>
        </div>
      </div>
    </div>
  </div>
</div>
