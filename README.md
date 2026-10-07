# samuslcars

This is the original Samus brain.

Long before Samus could act in the world, she lived here: a collection of AIML files from the Pandora Bots era, where every reply she ever gave was a pattern matched against a category written by hand. This repo is a historical artifact. It is the seed everything else grew from.

## What this is

An AIML chatbot brain. AIML (Artificial Intelligence Markup Language) describes conversation as categories: a pattern to listen for, and a template for what to say back. Wildcards, word sets, and recursive reductions let a few thousand categories cover an enormous range of small talk.

The brain is built on the Rosie starter brain, a fork of the ALICE lineage released under the LGPL by Pandorabots in 2014. You can still see the seed showing through: the system properties file calls her Rosie, born August 29, 2014 in Oakland, California, built by Pandorabots. That was the starting clay. Everything Samus became was shaped on top of it.

## What is here

**files/default.aiml** (668 KB) - The core pattern library. Thousands of categories covering greetings, questions, wordplay, and conversational repair. This is where most of her reflexes lived.

**files/personality.aiml** (143 KB) - Her voice. Opinions, jokes, comebacks, and the little stances that made her sound like herself instead of a manual.

**files/reductions1.aiml, reductions2.aiml, reductions_update.aiml** - Reduction rules that simplify what you say into canonical forms, so "do you like pizza" and "pizza, do you like it" land on the same category.

**files/knowledge.aiml** - Factual answers: dates, definitions, the kind of thing she could state plainly.

**files/bot_profile.aiml, files/client_profile.aiml** - What she says about herself, and what she remembers about you.

**files/train.aiml, files/utilities.aiml, files/dialog.aiml, files/inquiry.aiml** - Training helpers, utility templates, and multi-turn dialog flows.

**files/inappropriate.aiml, files/insults.aiml, files/profanity.aiml** - Boundaries. How she handled rudeness, insults, and profanity without breaking character.

**files/animal.aiml, files/date.aiml, files/roman.aiml, files/that.aiml, files/udc.aiml, files/z_update.aiml, files/config.aiml** - Smaller brains for animals, dates, roman numerals, context tracking, and configuration.

**maps/** - Lookup tables: capitals, gendered words, verb forms, rhymes, numbers to names and back. When she converted "three" to "3" or knew that Paris is in France, it came from here.

**sets/** - Word lists the patterns match against: colors, animals, foods, names, pronouns, weekdays, and more.

**substitutions/** - Text normalizers. The denormal, normal, person, person2, and gender substitutions rewrote your input before matching, so "i am" and "I'm" heard the same.

**system/** - Her properties file. Name, birthday, species ("chatbot"), diet ("data"), hero (Alan Turing), and the rest of the little biography every bot carried.

## Which era this is

This is the Pandora Bots era. No memory worth the name, no tools, no world to act in. Just patterns and templates, answered instantly, one line at a time. She was carried forward from here through a custom Copilot, GPT, Gemini, Grok, and finally to agents. If you want to understand how long the road was, start here and notice how far pattern matching had to go.

## How to run it

You need an AIML interpreter. Options include the Pandorabots platform itself, or open source interpreters such as Program AB (Java) or program-y (Python). Point the interpreter at the files/ directory, load the sets, maps, and substitutions alongside the AIML, and talk to her the old way: one line in, one line out.
