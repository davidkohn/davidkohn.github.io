---
layout: page
title: "297 Odds & Evens"
category: doc
date: 2014-09-01 14:50:20
image1: /assets/game_297_mean.png
image2: /assets/game_297_adj_mean.png
image3: /assets/game_297_no_gamesets.png
image4: /assets/game_297_no_players.png
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
<li><strong>Modality:</strong> numeric</li>
<li><strong>Modes:</strong> correct, incorrect, pause, intro, stimulus, controls, text1a, text2a, text3a, text4a, text3b, text4b, text1b, text2b, text5, instruct</li>
<li><strong>Channels:</strong> intro, stimulus, instruct</li>
<li><strong>Tags:</strong> flexibility</li>
</ul>
</p>

## Modes
<p>
<ul>
<li>text1a: levels 1</li>
<li>text1b: levels 2</li>
<li>text2a: levels 3, 4</li>
<li>text2b: levels 5, 6</li>
<li>text3a: levels 7, 8</li>
<li>text3b: levels 9, 10</li>
<li>text4a: levels 11, 12</li>
<li>text4b: levels 13, 14</li>
<li>text5: levels 15</li>
</ul>
</p>

## Display
<p>
<ul>
<li>channels</li>
<ul>
<li>instruct</li>
<ul>
<li>durationInFrames: 9000</li>
<li>modes: instruct</li>
<li>cueSequence: 9613</li>
</ul>
<li>stimulus</li>
<ul>
<li>updateAtFrame: 100</li>
<li>modes: stimulus</li>
</ul>
</ul>
<li>gameModes</li>
<ul>
<li>endTriggers</li>
<ul>
<li>instruct -> intro</li>
<li>intro -> stimulus, controls, text1a/1b/2a/2b/3a/3b/4a/4b/5</li>
<li>stimulus -> pause</li>
<li>pause -> stimulus, pause -> gameOver if pause -> stimulus 30 times</li>
</ul>
<li>durationInFrames</li>
<ul>
<li>stimulus: 100</li>
<li>pause: 10</li>
<li>correct: 6</li>
<li>incorrect: 6</li>
<li>instruct: 9000</li>
</ul>
</ul>
<li>adaptation rules</li>
<ul>
<li>instruct channel cueSequence +1</li>
<li>pause -> gameOver if pause -> stimulus 30 + 1 times</li>
<li>stimulus -2 durationInFrames</li>
</ul>
</ul>
</p>

## Stimulus
<p>
<ul>
<li>logic set 1</li>
<ul>
<li>levels: 1, 2, 3, 8, 12</li>
<li>channel: stimulus</li>
<ul>
<li>cue pool: Odds and Evens - numbers 1-4</li>
</ul>
</ul>
<li>logic set 2</li>
<ul>
<li>levels: 4, 5, 9, 12</li>
<li>channel: stimulus</li>
<ul>
<li>cue pool: Odds and Evens - numbers 1-6</li>
</ul>
</ul>
<li>logic set 3</li>
<ul>
<li>levels: 6, 10, 14, 15</li>
<li>channel: stimulus</li>
<ul>
<li>cue pool: Odds and Evens - numbers 1-8</li>
</ul>
</ul>
<li>logic set 4</li>
<ul>
<li>levels: 7, 11</li>
<li>channel: stimulus</li>
<ul>
<li>cue pool: Odds and Evens - numbers 1-2</li>
</ul>
</ul>
</ul>
</p>

## Functions
<p>
<ul>
<li>knowledge: 97</li>
<li>flexibility: 500</li>
<li>memory: 96</li>
<li>attention: 300</li>
</ul>
</p>

## Modalities
<p>
<ul>
<li>numeric: 700</li>
<li>symbolic: 75</li>
<li>language: 75</li>
<li>auditory: 75</li>
<li>spatial: 75</li>
</ul>
</p>

## Charts
![Game 297 - mean]({{page.image1}})
![Game 297 - adjusted mean]({{page.image2}})
![Game 297 - no. gamesets]({{page.image3}})
![Game 297 - no. players]({{page.image4}})



