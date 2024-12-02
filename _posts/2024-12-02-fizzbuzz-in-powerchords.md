---
title: 'fizzbuzz in powerchords'
date: 2024-12-02
permalink: /posts/2024/12/fizzbuzz-in-powerchords/
tags:
  - programming
  - music
  - computation
  - guitar
---

# fizzbuzz in powerchords

is your guitar turing complete? maybe. let's implement fizzbuzz in power chords because we can.

first we need to understand what makes something turing complete:
- infinite memory (fretboard theoretically extends forever)
- read/write head (your fretting hand)
- state register (chord shapes)
- branching logic (melodic patterns)
- symbols (notes/muting)

turns out a guitar is theoretically turing complete if you're willing to handwave some physical limitations. mostly the infinite neck thing, but hey, math is about abstractions right?

here's fizzbuzz implemented in power chords:

```text
// Guitar Code Translation
// Time signature: 4/4
// Tempo: 120 BPM
// Standard tuning

00:00 - Palm mute E5                   // Read input
00:01 - Palm mute E5                   // Read condition
00:02 - Palm mute E5                   // Read input
00:03 - A5 [sustain]                   // Write output and return
00:04 - Palm mute E5                   // Read input
00:05 - Palm mute E5                   // Read condition
00:06 - G5 -> D5 [sustain]             // Evaluate condition
00:07 - Palm mute E5                   // Read input
00:08 - A5 [sustain]                   // Write output and return
00:09 - Palm mute E5                   // Read input
00:10 - Palm mute E5                   // Read condition
00:11 - G5 -> D5 [sustain]             // Evaluate condition
00:12 - Palm mute E5                   // Read input
00:13 - A5 [sustain]                   // Write output and return
00:14 - Palm mute E5                   // Read input
00:15 - A5 [sustain]                   // Write output and return
```

palm muting represents reading from memory - it's our read head in action. each read is followed by a computation represented by chord progressions. fizzbuzz becomes a triple progression (E5 -> A5 -> D5), fizz is a double (E5 -> A5), and buzz takes a different path (A5 -> D5). the sustain marks our output operation.

you need these read operations (palm mutes) because a turing machine always needs to read before it computes. our guitar implementation faithfully follows this - read (palm mute), compute (progression), write (sustain). it's probably the least efficient implementation of fizzbuzz ever, but it's definitely the most metal.

here's the code that generates these metal computations:

```python
class GuitarCodeTranslator:
    def __init__(self):
        # Core operations mapped to power chords
        self.chord_map = {
            'READ': 'E5',
            'WRITE': 'A5',
            'COMPUTE': 'D5',
            'BRANCH': 'G5',
            'LOOP': 'C5'
        }
```

the rules are simple:
- read operation = palm mute
- computations = chord progressions  
- output = sustain
- timing follows a 4/4 signature because we're not monsters

under the hood, it walks your python AST and converts each node into a musical pattern. when it sees a modulo operation, it knows to insert a read operation first. every computation needs its input read first - that's what makes it turing complete.

```python
def fizzbuzz(n):
    if n % 3 == 0 and n % 5 == 0:
        return "FizzBuzz"
    elif n % 3 == 0:
        return "Fizz"
    elif n % 5 == 0:
        return "Buzz"
    return n
```

becomes a sequence of palm mutes and power chord progressions that sound weirdly prog rock. those modulo operations translate into patterns that would fit right into a tool breakdown.

why would you do this? because math and metal are just abstract ways of describing patterns in the universe. or maybe i've just been listening to too much tool.

you can find the full implementation [here](https://github.com/tehruhn/turing_complete_guitar). next up: implementing quicksort with pinch harmonics.

edit: yes, i know the fretboard isn't actually infinite. pls no emails about the halting problem.