---
layout: page
title: "How Synonyms and Antonyms Work"
category: doc
date: 2014-09-09 10:01:40
---

### Contents
{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

<p>
This article applies to Antonyms, Synonyms, Antonyms 2 and Synonyms 2.
</p>

## How the game works
<p>
<ul>
<li>Time: the game lasts 60 seconds on every level.</li>
<li>Stimuli selection: cues are selected randomly with replacement. </li>
<li>Level differences: </li>
<ul>
<li>Different cue pools are used for different levels.</li>
<li>Different initial targetscores are generated depending on the level. For a given level, l  targetscores are initially generated where l is the level number.</li>
</ul>
<li>How scoring works:</li>
<ul>
<li>An initial targetscore generated depending on the level. For a given level 'l', 'l+1' targetscores are initially generated where 'l' is the level number. Each targetscore has weight 1.0 which contributes to the denominator of the score. Each stimuus has a weight of 2.0. The final stimulus displayed can never be responded to.</li>
<li>score = (2.0 x no questions correct)/((2.0  * no questions displayed) + (1.0 * level no.))</li>
<li>For example if you answer only one question on level 1 and you answer that question correctly you will get a score of (2.0 * 1)/((2.0 * 2) + (1.0 * 1)) = 2/5 or 40%.</li>
<li>For example if you answer only one question on level 15 and your answer is correct the score will be (2.0 * 1)/((2.0 * 2) + (1.0 * 15)) = 2/19 or 11%.</li>
</ul>
</ul>
</p>


