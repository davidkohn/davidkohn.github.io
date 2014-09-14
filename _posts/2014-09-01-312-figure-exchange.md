---
layout: page
title: "312 Figure Exchange"
category: doc
date: 2014-09-01 15:51:10
image1: /assets/game_312_mean.png
image2: /assets/game_312_adj_mean.png
image3: /assets/game_312_no_gamesets.png
image4: /assets/game_312_no_players.png
json1: /assets/json-312.txt
cuepool1: /assets/cuepool-figure-exchange.csv
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

## How the game works
<p>
<ul>
<li>Two stimuli are presented each time. Stimuli A is a group of 4 card suits: hearts, clubs, spades and diamonds. Stimuli B is the same thing but the ordering is different. The user is asked how many moves it takes to get from A to B: 1, 2, 3, 4 or 5.</li>
<li>Stimuli are selected randomly without replacement.</li>
<li>At level 1 stimuli are presented for 80 seconds each. 2 stimuli are presented at level 1.</li>
<li>On each subsequent level 1 more stimulus is presented. Stimuli are displayed for 450 frames or 9 seconds less on each subsequent level. </li>
<li>For example at level 2, 3 stimuli are presented for 71 seconds each.</li>
<li>Correct and incorrect responses both have weight 1.0.</li>
</ul>
</p>

## Stimulus
<p>
<a href="{{page.cuepool1}}">CSV file of the cuepool data</a>.
<ul>
<li>logic set 1</li>
<ul>
<li>levels: 1, 2, 3, 4, 5</li>
<li>cue pool: Figure Exchange 1</li>
<li>average no. moves: 1.9</li>
</ul>
<li>logic set 2</li>
<ul>
<li>levels: 6, 7, 8, 9, 10</li>
<li>cue pool: Figure Exchange 2</li>
<li>average no. moves: 2.5</li>
</ul>
<li>logic set 1</li>
<ul>
<li>levels: 11, 12, 13, 14, 15</li>
<li>cue pool: Figure Exchange 3</li>
<li>average no. moves: 4.1</li>
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

## Example JSON
<p>
<ul>
<li><a href="{{ page.json1 }}">Here is a link to some example JSON</a> for game 312 level 1.</li>
<li>This JSON is only the 'play_data' portion of the actual JSON from a gameplay session.</li>
</ul>
</p>

## Charts
![Game 312 - mean]({{ page.image1}})
![Game 312 - adjusted mean]({{page.image2}})
![Game 312 - no. gamesets]({{page.image3}})
![Game 312 - no. players]({{page.image4}})









