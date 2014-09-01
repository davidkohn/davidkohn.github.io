---
layout: page
title: "285 Colour Stroop"
category: doc
date: 2014-08-31 22:15:50
image1: /assets/game_285_mean.png
image2: /assets/game_285_adj_mean.png
image3: /assets/game_285_no_gamesets.png
image4: /assets/game_285_no_players.png
---

### Contents
{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

## Summary
<p>
<ul>
<li><strong>Status:</strong> published</li>
<li><strong>Function:</strong> attention</li>
<li><strong>Modality:</strong> language</li>
<li><strong>Modes: </strong>intro, stimulus, timer, correct, targetscore, incorrect, stimuluspause</li>
<li><strong>Channels: </strong>wordsmeaning, wordscolour, into, targetscore</li>
<li><strong>Tags: </strong>attention</li>
</ul>
</p>

## Display
<p>
<ul>
<li>Channels</li>
<ul>
<li>targetscore</li>
<ul><li>updateAtFrame: 5</li>
<li>modes: targetscore</li>
</ul>
<li>wordsmeaning</li>
<ul><li>retries: 3</li>
<li>modes: stimulus</li>
</ul>
<li>wordscolour</li>
<ul><li>modes: stimulus</li></ul>
</ul>
<li>gameModes</li>
<ul>
<li>endTriggers</li>
<ul><li>intro -> stimulus, timer</li>
<li>stimuluspause -> stimulus</li>
<li>timer end = stimulus end</li>
<li>timer -> gameOver</li>
</ul>
<li>durationInFrames</li>
<ul><li>targetscore: 5</li>
<li>timer: 3000</li>
<li>stimuluspause: 6</li>
<li>correct: 10</li>
<li>incorrect: 10</li>
</ul>
</ul>
<li>Adaptation rules</li>
<ul><li>+5 duration to targetscore</li></ul>
</ul>
</p>

## Stimulus
<p>
<ul>
<li>channel: wordsmeaning</li>
<ul><li>cue pool: colour stroop - meaning (grey)</li></ul>
<li>channel: targetscore</li>
<ul><li>cue pool: colour stroop - taget</li>
<li>channel: wordscolour</li>
<ul>
<li>cue pool: colour stroop colour</li>
</ul>
</ul>
</ul>
</p>

## Rules
<p>
<ul>
<li>ID: 398</li>
<ul><li>criteria: targetscore.matchesTag(targetscore)</li>
<li>channel: targetscore</li>
</ul>
<li>ID: 399</li>
<ul><li>criteria: wordsmeaning.hasSameTagsAs(wordscolour)</li>
<li>channel: wordsmeaning</li></ul>
<li>ID: 400</li>
<ul><li>criteria: !wordsmeaning.hasSameTagsAs(wordscolour)</li>
<li>channel: wordsmeaning</li></ul>
</ul>
</p>

## Score Events
<p>
<ul>
<li>ID: 716</li>
<ul><li>score name: correct_response</li>
<li>channel: wordsmeaning</li>
<li>label: picked right</li>
<li>weight: 1.0</li>
<li>play events: start correct</li>
</ul>
<li>ID: 717</li>
<ul><li>score name: correct_non_response</li>
<li>channel: wordsmeaning</li>
<li>label: correctly ignored</li>
<li>weight: 1.0</li>
<li>penalty events</li>
<ul><li>start incorrect</li></ul>
</ul>
<li>ID: 718</li>
<ul><li>score name: correct_response</li>
<li>channel: targetscore</li>
<li>label: target score</li>
<li>weightL 1.0</li>
</ul>
</ul>
</p>

## Functions
<p>
<ul>
<li>knowledge: 98</li>
<li>flexibility: 98</li>
<li>memory: 98</li>
<li>attention: 699</li>
</ul>
</p>

## Modalities
<p>
<ul>
<li>numeric; 75</li>
<li>symbolic: 75</li>
<li>language: 700</li>
<li>auditory: 75</li>
<li>spatial: 75</li>
</ul>
</p>

## Charts
![Game 285 - mean]({{ page.image1}})
![Game 285 - adjusted mean]({{page.image2}})
![Game 285 - no. gamesets]({{page.image3}})
![Game 285 - no. players]({{page.image4}})


