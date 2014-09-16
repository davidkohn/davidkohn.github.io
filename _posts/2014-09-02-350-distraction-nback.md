---
layout: page
title: "350 Distraction nBack"
category: doc
date: 2014-09-02 14:13:08
image1: /assets/game_350_mean.png
image2: /assets/game_350_adj_mean.png
image3: /assets/game_350_no_gamesets.png
image4: /assets/game_350_no_players.png
json1: /assets/json-350.txt
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

## How the game works
<p>
<ul>
<li>Spatial and audio update/duration of 120 frames, but lasts 80%.</li>
<li>Distraction updates at 150 frames.</li>
<li>16 stimuli displayed at level 1. 1 stimuli added every level after 1.</li>
<li>Correct responses for spatial and auditory have weight 2.0.</li>
<li>Correct responses for distraction have weight 1.0.</li>
<li>The user is presented with a shape, audio cue and a direction. The user is asked if any of these matches the stimuli displayed n-stimuli back.</li>
<li>Game has n-back rule nBackA(1,0.5) where initial = 1 and scale = 0.5. nBackNumber = initial + parseInt((currentAdaptationLevel - 1) * scale, 10).</li>
</ul>
</p>

## Stimulus
<p>
<ul>
<li>Distraction</li>
<ul>
<li>Symbol pointed in 4 different directions.</li>
</ul>
<li>Shapes</li>
<ul>
<li>Pink triangle</li>
<li>Yellow pentagon</li>
<li>Purple hexagon</li>
<li>Green diamond</li>
<li>Red circle</li>
<li>Blue square</li>
<li>Orange star</li>
</ul>
<li>Audio</li>
<ul>
<li>Spoken letters</li>
<ul>
<li>t, k, e, o, y, w, g, l, d, p, f, q, u, v, a, j</li>
</ul>
</ul>
</ul>
</p>

## Levels
<p>
<ul>
<li>1-back: level 1, 2</li>
<li>2-back: level 3, 4</li>
<li>3-back: level 5, 6</li>
<li>4-back: level 7, 8</li>
<li>5-back: level 9, 10</li>
<li>6-back: level 11, 12</li>
<li>7-back: level 13, 14</li>
<li>8-back: level 15</li>
</ul>
</p>

## Example JSON
<p>
<ul>
<li><a href="{{ page.json1 }}">Here is a link to some example JSON</a> for game 350 level 1.</li>
<li>This JSON is only the 'play_data' portion of the actual JSON from a gameplay session.</li>
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


