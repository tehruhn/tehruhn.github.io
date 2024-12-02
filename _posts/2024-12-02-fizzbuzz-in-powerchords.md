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
0:06 - Palm mute E5 (4)
0:07 - D5 (output 4)
0:08 - Palm mute E5 (5)
0:09 - A5 -> D5 [sustain] (output Buzz)
0:10 - Palm mute E5 (6)
0:11 - E5 -> A5 [sustain] (output Fizz)
0:12 - Palm mute E5 (7)
0:13 - G5 (output 7)
0:14 - Palm mute E5 (8)
0:15 - A5 (output 8)
0:16 - Palm mute E5 (9)
0:17 - E5 -> A5 [sustain] (output Fizz)
0:18 - Palm mute E5 (10)
0:19 - A5 -> D5 [sustain] (output Buzz)
0:20 - Palm mute E5 (11)
0:21 - B5 (output 11)
0:22 - Palm mute E5 (12)
0:23 - E5 -> A5 [sustain] (output Fizz)
0:24 - Palm mute E5 (13)
0:25 - D5 (output 13)
0:26 - Palm mute E5 (14)
0:27 - G5 (output 14)
0:28 - Palm mute E5 (15)
0:29 - E5 -> A5 -> D5 [sustain] (output FizzBuzz)
```

palm muting represents reading the next number, like a cursor moving through memory. we use sustains on the fizz/buzz outputs because they're special cases - gotta let those ring out. it's probably the least efficient implementation of fizzbuzz ever, but it's definitely the most metal.

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

under the hood, it walks your python AST and converts each node into a musical pattern. assignments become C->G progressions because they feel like resolution. loops get D->Em->D because they return to where they started. the whole thing ends up sounding surprisingly musical - since code and music are both just patterns with rules.

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

becomes a sequence of chord progressions that sound weirdly prog rock. those modulo operations translate into Am->Em patterns that would fit right into a tool breakdown.

why would you do this? because math and metal are just abstract ways of describing patterns in the universe. or maybe i've just been listening to too much tool.

you can find the full implementation [here](https://github.com/tehruhn/turing_complete_guitar). next up: implementing quicksort with pinch harmonics.

edit: yes, i know the fretboard isn't actually infinite. please no emails about the halting problem.