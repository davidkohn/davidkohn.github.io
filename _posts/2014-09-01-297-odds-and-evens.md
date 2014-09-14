---
layout: page
title: "297 Odds & Evens"
category: doc
date: 2014-09-01 14:50:20
image1: /assets/game_297_mean.png
image2: /assets/game_297_adj_mean.png
image3: /assets/game_297_no_gamesets.png
image4: /assets/game_297_no_players.png
json1: /assets/json-297.txt
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

## How the game works
<p>
<ul>
<li>A set of instructions are displayed at the start of the game telling the user what the rule for the level is.</li>
<li>The game runs for 1 min. 30 stimuli are displayed for 2 seconds each.</li>
<li>For every level after level 1 an additional stimulus is displayed.Additionally, each stimuli is displayed for 1/25 of a second less for each level. For example 31 stimuli will be displayed on level 2, the game will last 0.98 * 2 seconds * 31 stimuli or aproximately 61 seconds. On level 3, 32 stimuli will be displayed each will be displayed for 4 frames less. The game will last 0.94 * 2 seconds * 32 or approximately 60 seconds. On level 4, 33 stimuli will be displayed for 6 frames less so the game will last 0.92 * 2 seconds * 33 or approximately 61 seconds. </li>
<li>The game displays stimuli which are a set of numbers that depend on the cue pool of a given level. The user must press a button is the relationship between the current number and numbers previously displayed matches the rule given at the beginning of the level.</li>
<li>A correct response has weight 1.0. If the relationship between the numbers did not match the rule and the user did not press anything this is counted as a correct non-response which also has weight 1.0. An incorrect response or an incorrect non-response also have wiehgt 1.0</li>
</ul>
</p>


## Cuepools
<p>
<ul>
<li>Level 1</li>
<ul>
<li>Rule: last and current are even.</li>
<li>Cue pool: Odds and Evens - numbers 1-4</li>
</ul>
<li>Level 2</li>
<ul>
<li>Rule: last and current are odd.</li>
<li>Cue pool: Odds and Evens - numbers 1-4</li>
</ul>
<li>Level 3</li>
<ul>
<li>Rule: last and current have parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-4</li>
</ul>
<li>Level 4</li>
<ul>
<li>Rule: last and current have parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-6</li>
</ul>
<li>Level 5</li>
<ul>
<li>Rule: last and current have no parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-6</li>
</ul>
<li>Level 6</li>
<ul>
<li>Rule: last and current have no parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-8</li>
</ul>
<li>Level 7</li>
<ul>
<li>Rule: second to last and current have parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-2</li>
</ul>
<li>Level 8</li>
<ul>
<li>Rule: second to last and current have parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-4</li>
</ul>
<li>Level 9</li>
<ul>
<li>Rule: second to last and current have no parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-6</li>
</ul>
<li>Level 10</li>
<ul>
<li>Rule: second to last and current have no parity.</li>
<li>Cue pool: Odds and Evens - numbers 1-8</li>
</ul>
<li>Level 11</li>
<ul>
<li>Rule: sum of last two have parity with current.</li>
<li>Cue pool: Odds and Evens - numbers 1-2</li>
</ul>
<li>Level 12</li>
<ul>
<li>Rule: sum of last two have parity with current.</li>
<li>Cue pool: Odds and Evens - numbers 1-4</li>
</ul>
<li>Level 13</li>
<ul>
<li>Rule: sum of last two have no parity with current.</li>
<li>Cue pool: Odds and Evens - numbers 1-6</li>
</ul>
<li>Level 14</li>
<ul>
<li>Rule: sum of last two have no parity with current.</li>
<li>Cue pool: Odds and Evens - numbers 1-8</li>
</ul>
<li>Level 15</li>
<ul>
<li>Rule: sum of last three have parity with current.</li>
<li>Cue pool: Odds and Evens - numbers 1-8</li>
</ul>
</ul>
</p>

## Modes
<p>
<ul>
<li>text1a: levels 1</li>
<ul>
<li>Rule: last and current are even.</li>
</ul>
<li>text1b: levels 2</li>
<ul>
<li>Rule: last and current are odd.</li>
</ul>
<li>text2a: levels 3, 4</li>
<ul>
<li>Rule: last and current have parity.</li>
</ul>
<li>text2b: levels 5, 6</li>
<ul>
<li>Rule: last and current have no parity.</li>
</ul>
<li>text3a: levels 7, 8</li>
<ul>
<li>Rule: second to last and current have parity.</li>
</ul>
<li>text3b: levels 9, 10</li>
<ul>
<li>Rule: second to last and current have no parity.</li>
</ul>
<li>text4a: levels 11, 12</li>
<ul>
<li>Rule: sum of last two have parity with current.</li>
</ul>
<li>text4b: levels 13, 14</li>
<ul>
<li>Rule: sum of last two have no parity with current.</li>
</ul>
<li>text5: levels 15</li>
<ul>
<li>Rule: sum of last three have parity with current.</li>
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
<li>levels: 4, 5, 9, 13</li>
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

## Example JSON
<p>
<ul>
<li><a href="{{ page.json1 }}">Here is a link to some example JSON</a> for game 297 level 1.</li>
<li>This JSON is only the 'play_data' portion of the actual JSON from a gameplay session.</li>
</ul>
</p>

## Charts
![Game 297 - mean]({{page.image1}})
![Game 297 - adjusted mean]({{page.image2}})
![Game 297 - no. gamesets]({{page.image3}})
![Game 297 - no. players]({{page.image4}})



