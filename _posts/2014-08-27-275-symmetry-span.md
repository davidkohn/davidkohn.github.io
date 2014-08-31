---
layout: page
title: "275 Symmetry Span"
category: doc
date: 2014-08-27 17:16:50
image1: /assets/game_275_mean.png
image2: /assets/game_275_adj_mean.png
image3: /assets/game_275_no_gamesets.png
image4: /assets/game_275_no_players.png
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
<li><strong>Modality:</strong> symbolic</li>
<li><strong>Modes:</strong> intro, spancollection, symmetry, correct, incorrect, spanpause, controls, pause</li>
<li><strong>Channels:</strong> intro, span, symmetryleft, symmetryright, followleft, followright</li>
<li><strong>Tags:</strong> memory</li>
</ul>
</p>

## Display
<p>
<ul>
<li>Channels</li>
<ul>
<li>span</li>
<ul>
<li>cueSelectionMethod: dice</li>
<li>delayInPercent: 10</li>
<li>durationInPercent: 10</li>
<li>modes: symmetry</li>
</ul>
<li>symmetryright</li>
<ul>
<li>cueSelectionMethod: dice</li>
<li>modes: symmetry</li>
</ul>
<li>symmetryleft</li>
<ul>
<li>cueSelectionMethod: dice</li>
<li>retries: 50</li>
<li>modes: symmetry</li>
</ul>
<li>followRight</li>
<ul>
<li>followChannel: symmetryright</li>
<li>modes: symmetry</li>
</ul>
<li>followLeft</li>
<ul>
<li>followChannel: symmetryleft</li>
<li>modes: symmetry</li>
</ul>
</ul>
<li>gameModes</li>
<ul>
<li>endTriggers</li>
<ul>
<li>intro -> symmetry,controls</li>
<li>pause -> symmetry, pause -> spanpause is 2 loops between pause and symmetry</li>
<li>spanpause end = symmetry, controls end</li>
<li>spanpause -> spancollection</li>
</ul>
<li>durationInFrames</li>
<ul>
<li>pause: 8</li>
<li>spanpause: 8</li>
<li>correct: 6</li>
<li>incorrect: 6</li>
</ul>
<li>adaptation rules</li>
<ul>
<li>pause -> spanpause if 2 + <em>i</em> loops between pause and symmetry where <em>i</em> = level - 1</li>
</ul>
</ul>
</ul>
</p>

## Stimulus
<p>
<ul>
<li>channel: span </li>
<ul><li>symmetry span - 8 animals </li></ul>
<li>channel: symmetryLeft </li>
<ul><li>cue pool: symmetry span - A Left</li></ul>
<li>channel: symmetryRight</li>
<ul><li>cue pool: symmetry span - A Right</li></ul>
</ul>
</ul>
</p>

## Rules
<p>
<ul>
<li>ID: 358</li>
<ul><li>criteria: (followleft.ordinalityValue() == followright.ordinalityValue() && ((followleft.containsTag('left') && followright.containsTag('I_flip')) || (followleft.containsTag('r_flip') && followright.containsTag('right')))</li></ul>
<li>ID: 607</li>
<ul><li>criteria: symmetryLeft.ordinalityValue() == symmetryright.ordinalityValue()</li></ul>
</ul>
</p>

## Buttons
<p>
<ul>
<li>Name: Memory - Down - label left</li>
<ul><li>tags: no</li>
<li>ID: 569</li>
</ul>
<li>Name: Memory - Up - label left</li>
<ul><li>tags: yes</li>
<li>ID: 568</li>
</ul>
</ul>
</p>

## Palettes
<p>
<ul>
<li>palette: symmetry span</li>
<li>modes: spancollection</li>
</ul>
</p>

## Collections
<p>
<ul>
<li>modes: spancollection</li>
<li>channel: span</li>
</ul>
</p>

## Score Events
<p>
<ul>
<li>ID: 883</li>
<ul>
<li>score name: correct_non_response</li>
<li>channel: followleft</li>
<li>label: incorrect symmetry</li>
<li>weight: 2.0</li>
<li>play events</li>
<ul><li>start correct</li></ul>
<li>penalty play events</li>
<ul><li>incorrect start</li>
<li>symmetry end</li>
<li>pause start</li>
</ul>
</ul>
<li>ID: 695</li>
<ul>
<li>score name: correct_cue_position</li>
<li>channel: span</li>
<li>label: symbols remembered</li>
<li>weight: 5.0</li>
</ul>
<li>ID: 696</li>
<ul>
<li>score name: correct_response</li>
<li>channel: followleft</li>
<li>label: correct symmetry</li>
<li>weight: 2.0</li>
<li>play events</li>
<ul><li>end symmetry</li>
<li>start pause</li>
<li>start correct</li>
</ul>
<li>penalty play events</li>
<ul>
<li>start incorrect</li>
</ul>
</ul>
</ul>
</p>

## Functions
<p>
<ul>
<li>knowledge: 97</li>
<li>flexibility: 300</li>
<li>memory: 500</li>
<li>attention: 96</li>
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
![Game 275 - mean]({{ page.image1}})
![Game 275 - adjusted mean]({{page.image2}})
![Game 275 - no. gamesets]({{page.image3}})
![Game 275 - no. players]({{page.image4}})



