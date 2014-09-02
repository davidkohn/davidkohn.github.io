---
layout: page
title: "350 Distraction nBack"
category: doc
date: 2014-09-02 14:13:08
image1: /assets/game_350_mean.png
image2: /assets/game_350_adj_mean.png
image3: /assets/game_350_no_gamesets.png
image4: /assets/game_350_no_players.png
---

### Contents
{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Summary
<p>
<ul>
<li><strong>Status:</strong> published</li>
<li><strong>Function:</strong> memory</li>
<li><strong>Modality:</strong> spatial</li>
<li><strong>Modes:</strong> intro, stimulus, correct, incorrect, pause, control, distraction, d_correct, d_incorrect, n_pause, instruct</li>
<li><strong>Channels:</strong> spatial, auditory, intro, distraction, instruct</li>
<li><strong>Tags:</strong> memory</li>
</ul>
</p>

## Display
<p>
<ul>
<li>channels</li>
<ul>
<li>spatial</li>
<ul>
<li>durationInPercent: 80</li>
<li>updateAtFrame: 120</li>
</ul>
<li>auditory</li>
<ul>
<li>durationInPercent: 80</li>
<li>updateAtFrame: 120</li>
</ul>
<li>distraction: 150</li>
<ul>
<li>updateAtFrame: 150</li>
</ul>
</ul>
<li>gameModes</li>
<ul>
<li>endTriggers</li>
<ul>
<li>intro -> n_pause, control</li>
<li>n_pause -> stimulus, distraction</li>
<li>pause -> stimulus, distraction</li>
<li>stimulus -> pause, if loop 16x stimulus -> gameOver</li>
</ul>
<li>durationInFrames</li>
<ul>
<li>stimulus: 120</li>
<li>distraction: 150</li>
</ul>
</ul>
<li>adaptation rules</li>
<ul>
<li>instruct channel - cueSequence +1</li>
<li>gameModes stimulus -> pause, if loop 16 + 1x stimulus -> gameOver</li>
</ul>
</ul>
</p>

## Score Events
<p>
<ul>
<li>distraction - weight 1.0</li>
<li>spatial/auditory - weight 2.0</li>
</ul>
</p>

## Functions
<p>
<ul>
<li>knowledge: 99</li>
<li>flexibility: 97</li>
<li>memory: 700</li>
<li>attention: 97</li>
</ul>
</p>

## Modalities
<p>
<ul>
<li>numeric: 67</li>
<li>symbolic: 67</li>
<li>language: 66</li>
<li>auditory: 300</li>
<li>spatial: 500</li>
</ul>
</p>

## Charts
![Game 350 - mean]({{ page.image1}})
![Game 350 - adjusted mean]({{page.image2}})
![Game 350 - no. gamesets]({{page.image3}})
![Game 350 - no. players]({{page.image4}})


