---
layout: page
title: "275 Symmetry Span"
category: doc
date: 2014-08-27 17:16:50
image1: /assets/game_275_mean.png
image2: /assets/game_275_adj_mean.png
image3: /assets/game_275_no_gamesets.png
image4: /assets/game_275_no_players.png
cuepool1: /assets/cuepool-symmetry-span-all.csv
json1: /assets/json-275.txt
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

## How the game works
<p>
<ul>
<li>The game has two components:</li>
<ul>
<li>A symmetry component where the user must identify if an image is symmetrical or not.</li>
<ul>
<li>The image is made up of two smaller images and the larger image will be symmetrical when the second smaller image is the flipped version of the first smaller image.</li>
<li>Each image is composed of 32 yellow colored or non-colored dots arranged in an 8 long by 4 wide matrix.</li>
<li>This component has weight 2.0 per stimuli</li>
</ul>
<li>A span component. A picture of an animal is displayed alongside each symmetry question. After all stimuli have been presented the user is asked to recall the order they were presented in.</li>
<ul>
<li>This component has weight 5.0 per stimuli.</li>
</ul>
</ul>
<li>Cues for both the span and symmetry components are selected randomly with replacement.</li>
<li>2 stimuli are presented at level 1. Every level after adds 1 stimuli, e.g. level 2 displays 3 stimuli, level 3 displays 4 stimuli, etc.</li>
</ul>
</p>

## Cuepools
<p>
Click <a href="{{ page.cuepool1 }}">here for a CSV file</a> of the combined cuepool data. This includes data on the number of colored dots in each image.
<ul>
<li>Symmetry Span - A Left/Right</li>
<ul>
<li>Level 1, 2, 3</li>
<li>Left - avg. no. colored dots: 19.75</li>
<li>Right - avg. no. colored dots: 19.72</li>
</ul>
<li>Symmetry Span - B Left/Right</li>
<ul>
<li>Level 4, 5, 6</li>
<li>Left - avg. no. colored dots: 20.55</li>
<li>Right - avg. no. colored dots: 20.88</li>
</ul>
<li>Symmetry Span - C Left/Right</li>
<ul>
<li>Level 7, 8, 9</li>
<li>Left - avg. no. colored dots: 21.43</li>
<li>Right - avg. no. colored dots: 21.77</li>
</ul>
<li>Symmetry Span - D Left/Right</li>
<ul>
<li>Level 10, 11, 12</li>
<li>Left - avg. no. colored dots: 22.43</li>
<li>Right - avg. no. colored dots: 22.90</li>
</ul>
<li>Symmetry Span - E Left/Right</li>
<ul>
<li>Level 13, 14, 15</li>
<li>Left - avg. no. colored dots: 23.04</li>
<li>Right - avg. no. colored dots: 23.14</li>
</ul>
</ul>
</p>

## Example JSON
<p>
<ul>
<li><a href="{{ page.json1 }}">Here is a link to some example JSON</a> for game 275 level 1.</li>
<li>This JSON is only the 'play_data' portion of the actual JSON from a gameplay session.</li>
<li>Additionally the intro sequence has also been removed from the 'play_data'.</li>
<li>Stimuli are displayed in the 'show_cue' actions.</li>
<li>Responses are evaluated after all stimuli have been displayed. The score event is 'correct_cue_position' for the span component of the task.</li>
<li>Score events 'correct_non_response' and 'correct_response' are part of the symmetry tak.</li>
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



