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
// FizzBuzz implementation in power chords
// Time signature: 4/4
// Tempo: 120 BPM
// Base position: Standard tuning

// Setup:
// - Single power chord = number
// - E5 -> A5 progression = Fizz
// - A5 -> D5 progression = Buzz
// - E5 -> A5 -> D5 progression = FizzBuzz
// - Palm mute = read number
// - Open strum = output

// Initialize counter
0:00 - Palm mute E5 (counter = 1)

// Main loop
0:01 - E5 (output 1)
0:02 - Palm mute E5 (2)
0:03 - A5 (output 2)
0:04 - Palm mute E5 (3)
0:05 - E5 -> A5 [sustain] (output Fizz)
```

(rest of the implementation continues with the same pattern)

but why stop there? let's write code that converts any python function into guitar tabs. here's a translator that turns your code into a sequence of chord progressions:

```python
class GuitarTranslator:
    def __init__(self):
        self.basic_chords = ['Em', 'G', 'C', 'D', 'Am']
        self.special_progressions = {
            'if': ['Em', 'G'],
            'else': ['Am', 'C'],
            'while': ['D', 'Em', 'D'],
            'return': ['G', 'Em', 'C'],
            'assignment': ['C', 'G'],
        }
        # map different operations to chord progressions
        self.operator_maps = {
            'Add': ['G', 'C'],
            'Sub': ['Em', 'Am'],
            'Mult': ['D', 'G'],
            'Div': ['Am', 'Em'],
            'Eq': ['C', 'C'],
        }
```

the rules are simple:
- control flow gets specific progressions (if = Em->G)
- operations map to intervals (addition = G->C)
- values become chords based on their magnitude
- timing follows a 4/4 signature because we're not monsters

why would you do this? because math and metal are just abstract ways of describing patterns in the universe. or maybe i've been listening to too much tool.

you can find the full implementation [here](https://github.com/tehruhn/turing_complete_guitar). it's probably the least efficient but most headbangable implementation of fizzbuzz ever created.

brb implementing quicksort with pinch harmonics.

edit: yes, i know the fretboard isn't actually infinite. please dont email me about the halting problem.