Download Link: https://assignmentchef.com/product/solved-comp2300-assignment-2-part-2
<br>
In assignment 2 you need to program your discoboard to schedule/trigger a <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Music_sequencer">sequence</a> of “notes”, each with a different pitch/duration/loudness. As in assignment 1, the focus is on controlling the behaviour of your discoboard with assembly code rather than doing a bunch of music theory.

This assignment will again have two parts: in Part 1, you need to play a specific sequence of notes with specific timing. In Part 2, you can generate a new sequence of your own creation to demonstrate the capabilities of your sequencer.

<h2 id="background">Background</h2>

Sequencers are tools for “scheduled execution”, playing the right note at the right time, and they have been instrumental in electronic music history. Drum sequencers, like the classic <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Roland_TR-909">Roland TR-909</a> drum sequencer—a piece of electronic hardware designed for <strong>sequencing</strong> drum patterns—led to the development of electronic dance music, such as Daft Punk’s <a class="acton-tabs-link-processed" href="https://youtu.be/uURB-vo9rZ4">Revolution 909</a> from their classic album <em>Homework</em> (1997).

Sequencers aren’t limited to making drum sounds—the pattern they generate might be a sequence of musical notes, like in a bassline or melody line. In fact, this core concept is not even unique to music—the same ideas are found in scheduling, robotics, cyberphysical systems, and a bunch of other domains. The key idea is that sequencing is a way of controlling a device to perform certain actions at certain times.

<h2 id="part-1">Part 1</h2>

In Part 1, you must program your discoboard to play a specific sequence of notes—and you have 2 options this time, <strong>pick 1</strong>:

<ul>

 <li><a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#hotmk">In the Hall of the Mountain King from “Peer Gynt”</a></li>

 <li><a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#sos-loz">Song of Storms from Legend of Zelda</a></li>

</ul>

All options are considered of equal difficulty and will be marked to the same standard (<a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#part-1-marks">see the marking section for part 1</a>)—ie. you will not gain or lose marks for picking one option over another.

We have provided a list of note names, <strong>frequencies</strong>, and <strong>durations</strong> for each song (including the gaps/silence in between the notes). These “pitch tables” contain the <strong>timing and frequencies</strong> we will use to mark part-1.

We have also included a list of the notes (as letter names), just in case you would like to sing/play them yourself, but <strong>please use the frequency/duration tables for producing your solution</strong>.

No matter which song you pick, your sequencer must:

<ul>

 <li>use an <strong>audible square wave sound</strong> (you can re-use your code from Assignment 1, but make sure to note it in the SoO) (the duty cycle is not important)</li>

 <li><strong>loop forever</strong>—i.e. such that when the sequence finishes playing, it starts again from the beginning (with no interruption to the timing)</li>

</ul>

Setting up and playing audio is the exact same as <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/01-synth/">assignment 1</a>.

<h3 id="hotmk">In the Hall of the Mountain King – Peer Gynt</h3>

<a class="acton-tabs-link-processed" href="https://onlinesequencer.net/2007067">We’ve also done these in an online sequencing software for your preview-ing pleasure</a>.

<table id="note-table">

 <thead>

  <tr>

   <th>Note</th>

   <th>Frequency</th>

   <th>Duration</th>

  </tr>

 </thead>

 <tbody>

  <tr>

   <td>B2</td>

   <td>123.47 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>C#3</td>

   <td>138.59 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>D3</td>

   <td>146.83 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>E3</td>

   <td>164.81 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F#3</td>

   <td>184.99 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>D3</td>

   <td>146.83 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F#3</td>

   <td>184.99 Hz</td>

   <td>0.44 s</td>

  </tr>

  <tr>

   <td>F3</td>

   <td>174.61 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>C#3</td>

   <td>138.59 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F3</td>

   <td>174.61 Hz</td>

   <td>0.44 s</td>

  </tr>

  <tr>

   <td>E3</td>

   <td>164.81 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>C3</td>

   <td>130.81 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>E3</td>

   <td>164.81 Hz</td>

   <td>0.44 s</td>

  </tr>

  <tr>

   <td>B2</td>

   <td>123.47 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>C#3</td>

   <td>138.59 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>D3</td>

   <td>146.83 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>E3</td>

   <td>164.81 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F#3</td>

   <td>184.99 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>D3</td>

   <td>146.83 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F#3</td>

   <td>184.99 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>B3</td>

   <td>246.94 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>A3</td>

   <td>220 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F#3</td>

   <td>184.99 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>D3</td>

   <td>146.83 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>F#3</td>

   <td>184.99 Hz</td>

   <td>0.22 s</td>

  </tr>

  <tr>

   <td>A3</td>

   <td>220 Hz</td>

   <td>0.44 s</td>

  </tr>

  <tr>

   <td>silence</td>

   <td>0 Hz</td>

   <td>0.44 s</td>

  </tr>

 </tbody>

</table>

<a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#a-backing-track-for-in-the-hall-of-the-mountain-king">If you feel like going the extra mile, for street cred.</a>

<h3 id="sos-loz">Song of Storms – Legend of Zelda</h3>

<a class="acton-tabs-link-processed" href="http://onlinesequencer.net/1999846">We’ve also done these in an online sequencing software for your preview-ing pleasure</a>.

<table id="note-table">

 <thead>

  <tr>

   <th>Note</th>

   <th>Frequency</th>

   <th>Duration</th>

  </tr>

 </thead>

 <tbody>

  <tr>

   <td>D4</td>

   <td>293.66 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>F4</td>

   <td>349.23 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>D5</td>

   <td>587.33 Hz</td>

   <td>0.6 s</td>

  </tr>

  <tr>

   <td>D4</td>

   <td>293.66 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>F4</td>

   <td>349.23 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>D5</td>

   <td>587.33 Hz</td>

   <td>0.6 s</td>

  </tr>

  <tr>

   <td>E5</td>

   <td>659.25 Hz</td>

   <td>0.45 s</td>

  </tr>

  <tr>

   <td>F5</td>

   <td>698.46 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>E5</td>

   <td>659.25 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>F5</td>

   <td>698.46 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>E5</td>

   <td>659.25 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>C5</td>

   <td>523.35 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>A4</td>

   <td>440 Hz</td>

   <td>0.45 s</td>

  </tr>

  <tr>

   <td>silence</td>

   <td>0 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>A4</td>

   <td>440 Hz</td>

   <td>0.3 s</td>

  </tr>

  <tr>

   <td>D4</td>

   <td>293.66 Hz</td>

   <td>0.3 s</td>

  </tr>

  <tr>

   <td>F4</td>

   <td>349.23 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>G4</td>

   <td>392.00 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>A4</td>

   <td>440 Hz</td>

   <td>0.75 s</td>

  </tr>

  <tr>

   <td>silence</td>

   <td>0 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>A4</td>

   <td>440 Hz</td>

   <td>0.3 s</td>

  </tr>

  <tr>

   <td>D4</td>

   <td>293.66 Hz</td>

   <td>0.3 s</td>

  </tr>

  <tr>

   <td>F4</td>

   <td>349.23 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>G4</td>

   <td>392.00 Hz</td>

   <td>0.15 s</td>

  </tr>

  <tr>

   <td>E4</td>

   <td>329.63 Hz</td>

   <td>0.9 s</td>

  </tr>

 </tbody>

</table>

<h3 id="part-1-marks">Part 1 Marks</h3>

Marks will be awarded for:

<ul>

 <li>generating notes with a square wave (duty cycle does not matter)</li>

 <li>playing the notes with the <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#exact-timing-frequency">correct pitches (frequency)</a></li>

 <li>playing the notes at the <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#exact-timing-frequency">correct tempo (timing)</a></li>

 <li>code structure, readability &amp; modularity (including comments &amp; use of functions)</li>

 <li>how modular your sequencer is—that is how easy is it to change what sequence / song is played (<strong>to have the possibility of full marks for this part</strong> you will need to use a data structure, <em>such as an array</em>, to store the song’s data).</li>

</ul>

For questions around frequency accuracy, <em>please read</em> <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#how-close">this section</a>.

<h2 id="part-2">Part 2</h2>

In Part 2, your task is to make a <strong>more advanced sequencer</strong>. Your program must generate a musical signal which plays indefinitely (either by “looping” a finite sequence or by coming up with a continuous stream of new notes). You may extend <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/deliverables/02-sequencer/#reusing-part-1">the sequences from part 1</a>, but the sequence must demonstrate the more advanced features of your sequencer.

Keep in mind that your job here is to make a cool <em>sequencer</em>, not a cool song, or a cool synth. As written above, a sequencer’s focus is scheduled execution of musical patterns, so you need to create a program than can schedule execution of <strong>more complex, or multiple</strong>, musical patterns, or do so with <strong>more utility</strong> than the very simple sequencer you create for part-1.

Here are a few ideas, in roughly increasing order of difficulty:

<ul>

 <li>Create a sequencer that sequences more aspects of music than just pitch and duration. E.g., it could continuously change another aspect of music such as <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Dynamics_(music)">dynamics (loudness/softness)</a> or <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Timbre">timbre (type of waveform)</a> on a note-by-note basis.</li>

 <li>Create a sequencer that plays songs that are stored in a more interesting format (or a subset of the format), e.g., <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/ABC_notation">ASCII text – see ABC notation</a>, or <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/MIDI">MIDI bytes</a>.</li>

 <li>Create a sequencer that can play multiple notes simultaneously to create <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Harmony">harmony</a> (also called <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Polyphony_and_monophony_in_instruments#Synthesizer">polyphony</a> in synth lingo). This could also be used to play multiple instrument tracks of the same song at the same time (e.g., keyboard and bass).</li>

 <li>create a sequencer that uses an <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Envelope_(music)#ADSR">amplitude envelope</a> to change the “shape” of your notes, with envelope parameters that change during playback.</li>

 <li>create a <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Polyphony_and_monophony_in_instruments#Synthesizer">polyphonic</a> <a class="acton-tabs-link-processed" href="https://en.wikipedia.org/wiki/Drum_machine">drum machine</a> that sequences non-pitched (e.g., percussive) sounds with sequenceable envelopes and synthesis parameters.</li>

</ul>

Marks for Part 2 will be awarded for a <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/resources/design-document/"><strong>design document</strong></a> describing what you’re doing and how you implemented it in ARM assembly language. You need to explain the <strong>“what”, “how” and “why”</strong> (<a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/resources/design-document/">design, implementation, and analysis</a>) of what you have done. Although it’s ok if you don’t do something <em>super</em>-complex, we do take the <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/resources/faq/#ambition">sophistication</a> of your sequencer into account. <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/resources/faq/#images-in-dd">Using images/diagrams</a> is encouraged. Your design document must be in <strong>pdf</strong> format <a class="acton-tabs-link-processed" href="https://cs.anu.edu.au/courses/comp2300/resources/faq/#can-my-design-document-be-longer-than-two-pages">(2 pages content + appendix + references)</a> with the filename <code>design-document.pdf</code> in top-level folder on the <code>part-2</code> branch.

5/5 - (1 vote)

[youtube https://www.youtube.com/watch?v=4nMUr8Rt2AI]