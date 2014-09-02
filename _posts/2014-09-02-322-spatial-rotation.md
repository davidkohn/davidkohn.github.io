---
layout: page
title: "322 Spatial Rotation"
category: doc
date: 2014-09-02 12:56:42
image1: /assets/game_322_mean.png
image2: /assets/game_322_adj_mean.png
image3: /assets/game_322_no_gamesets.png
image4: /assets/game_322_no_players.png
---

### Contents
{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Summary
<p>
<ul>
<li><strong>Status:</strong> published</li>
<li><strong>Function:</strong> flexibility</li>
<li><strong>Modality:</strong> spatial</li>
<li><strong>Modes:</strong> incorrectD, incorrectR, incorrectU, incorrectL, correctD, correctR, correctU, correctL, timer, correct, incorrect, pause, intro, stimulus, controls</li>
<li><strong>Channels:</strong> intro, objectA, side, objectB, objectC, front, top, followA, followB, followC, next</li>
<li><strong>Tags:</strong> flexibility</li>
</ul>
</p>

## Display
<p>
<ul>
<li>gameModes</li>
<ul>
<li>endTriggers</li>
<ul>
<li>intro -> stimulus, timer, controls</li>
<li>timer end = stimulus end</li>
<li>stimulus -> pause</li>
<li>correct end = timer/correctL/correctU/correctR/correctD</li>
<li>incorrect end = timer/incorrectL/incorrectU/incorrectR/incorrectD</li>
<li>pause -> stimulus, timer, controls, pause -> gameOver if pause loops 12x</li>
</ul>
</ul>
<li>durationInFrames</li>
<ul>
<li>correct: 35</li>
<li>incorrect: 35</li>
<li>timer: 1500</li>
<li>pause: 12</li>
</ul>
</ul>
</p>

## Stimulus
<p>
<ul>
<li>levels: 1</li>
<ul>
<li>channel: objectA, cue pool: spatial rotation - objects 1A</li>
<li>channel: side, cue pool: spatial rotation - sides 1</li>
<li>channel: front, cue pool: spatial rotation - fronts 1</li>
<li>channel: top, cue pool: spatial rotation - tops 1</li>
<li>channel: objectB, cue pool: spatial rotation - objects 1B</li>
<li>channel: objectC, cue pool: spatial rotation - objects 1C</li>
</ul>
<li>levels: 2, 3</li>
<li>levels: 4, 5</li>
<li>levels: 6, 7</li>
<li>levels: 8, 9</li>
<li>levels: 10, 11</li>
<li>levels: 12, 13</li>
<li>levels: 14, 15</li>
</ul>
</p>

## Functions
<p>
<ul>
<li>knowledge: 97</li>
<li>flexibility: 500</li>
<li>memory: 299</li>
<li>attention: 97</li>
</ul>
</p>

## Modalities
<p>
<ul>
<li>numeric: 75</li>
<li>symbolic: 75</li>
<li>language: 75</li>
<li>auditory: 75</li>
<li>spatial: 75</li>
</ul>
</p>

## Charts
![Game 322 - mean]({{ page.image1}})
![Game 322 - adjusted mean]({{page.image2}})
![Game 322 - no. gamesets]({{page.image3}})
![Game 322 - no. players]({{page.image4}})

