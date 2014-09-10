---
layout: page
title: "312 Figure Exchange"
category: doc
date: 2014-09-01 15:51:10
image1: /assets/game_312_mean.png
image2: /assets/game_312_adj_mean.png
image3: /assets/game_312_no_gamesets.png
image4: /assets/game_312_no_players.png
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
<li><strong>Modality:</strong> symbolic</li>
<li><strong>Modes:</strong> solution, reveal, correct, incorrect, intro, controls, deadkey, stimulus, pause</li>
<li><strong>Channels:</strong> intro, stimulus</li>
<li><strong>Tags:</strong> flexibility</li>
</ul>
</p>

## Display
<p>
<ul>
<li>channels</li>
<ul>
<li>stimulus</li>
<ul>
<li>cueSelectionMethod: deck</li>
</ul>
</ul>
<li>gameModes</li>
<ul>
<li>endTriggers</li>
<ul>
<li>intro -> stimulus, solution, controls</li>
<li>pause -> stimulus, solution, controls</li>
<li>stimulus -> pause, stimulus -> gameOver when stimulus -> pause execute 2 times</li>
<li>incorrect end = stimulus, controls end</li>
<li>correct end = stimulus, controls end</li>
</ul>
<li>durationInFrames</li>
<ul>
<li>stimulus: 4000</li>
<li>solution: 4000</li>
<li>pause: 20</li>
<li>correct: 20</li>
<li>incorrect: 20</li>
</ul>
</ul>
<li>adaptation rules</li>
<ul>
<li>stimulus -> gameOver when stimulus -> pause looped 2 + 1 times</li>
<li>stimulus -250 durationInFrames</li>
<li>solution -250 durationInFrames</li>
</ul>
</ul>
</p>

## Stimulus
<p>
<ul>
<li>logic set 1</li>
<ul>
<li>levels: 1, 2, 3, 4, 5</li>
<li>channel: stimulus</li>
<ul><li>cue pool: Figure Exchange 1</li></ul>
</ul>
<li>logic set 2</li>
<ul>
<li>levels: 6, 7, 8, 9, 10</li>
<li>channel: stimulus</li>
<ul><li>cue pool: Figure Exchange 2</li></ul>
</ul>
<li>logic set 1</li>
<ul>
<li>levels: 11, 12, 13, 14, 15</li>
<li>channel: stimulus</li>
<ul><li>cue pool: Figure Exchange 3</li></ul>
</ul>
</ul>
</p>

## Functions
<p>
<ul>
<li>knowledge: 98</li>
<li>flexibility: 700</li>
<li>memory: 98</li>
<li>attention: 97</li>
</ul>
</p>

## Modalities
<p>
<ul>
<li>numeric: 75</li>
<li>symbolic: 700</li>
<li>language: 75</li>
<li>auditory: 75</li>
<li>spatial: 75</li>
</ul>
</p>

## Charts
![Game 312 - mean]({{ page.image1}})
![Game 312 - adjusted mean]({{page.image2}})
![Game 312 - no. gamesets]({{page.image3}})
![Game 312 - no. players]({{page.image4}})









