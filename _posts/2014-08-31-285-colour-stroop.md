---
layout: page
title: "285 Colour Stroop"
category: doc
date: 2014-08-31 22:15:50
image1: /assets/game_285_mean.png
image2: /assets/game_285_adj_mean.png
image3: /assets/game_285_no_gamesets.png
image4: /assets/game_285_no_players.png
cuepool1: /assets/cuepool-colour-stroop.csv
json1: /assets/json-285.txt
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

## How the game works
<p>
<ul>
<li>Stimuli are presented over 60 seconds.</li>
<li>Two stimuli are presented each time. The stimuli are two words which are the names of colors. The words are also colored in themselves. The user is asked if 'meaning' and 'color' match. </li>
<li>The game has a targetscore component.</li>
<ul>
<li>An initial 'l' target scores are generated where 'l' is the level number, e.g. 1 target scores on level 1, 15 target scores on level 15.</li>
<li>Target score events have a weight of 1.0.</li>
<li>A target score event is also generated for the last question as the user is never able to answer the last question, i.e. the game will always end when the user is looking at a question.</li>
</ul>
<li>Correct responses, i.e. correctresponse, have a weight of 1.0.</li>
<li>Score is determined as (1.0 * no. correct responses) / (((level no. + 1) * 1.0) + (no. stimuli presented * 1.0))</li>
<li>For example, if the user answers 2 out of 3 questions correct on level 1 their score will be, 2/5 or 40%. If the user answers 1 out of 4 questions correctly on level 15 their score will be 1/20 or 5%.</li>
</ul>
</p>

## Cue Pools
<p>
<ul>
<li>The colors and words red, black, yellow and blue are displayed.</li>
<li>Here is <a href="{{ page.cuepool1 }}">a CSV file of the cuepool</a>.</li>
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

## Example JSON
<p>
<ul>
<li><a href="{{ page.json1 }}">Here is a link to some example JSON</a> for game 285 level 1.</li>
<li>This JSON is only the 'play_data' portion of the actual JSON from a gameplay session.</li>
<li>Stimuli are displayed in the 'show_cue' actions.</li>
<li>Responses are evaluated after all stimuli have been displayed. The score event is 'correct_cue_position'.</li>
</ul>
</p>

## Charts
![Game 285 - mean]({{ page.image1}})
![Game 285 - adjusted mean]({{page.image2}})
![Game 285 - no. gamesets]({{page.image3}})
![Game 285 - no. players]({{page.image4}})


