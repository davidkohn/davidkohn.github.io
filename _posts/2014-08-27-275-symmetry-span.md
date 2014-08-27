---
layout: page
title: "275 Symmetry Span"
category: doc
date: 2014-08-27 17:16:50
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
</p>



