## Lazy Refucktoring

 * [wat](#wat)
 * [the code](#the-code)
 * [how to refucktor](#how-to-refucktor)
 * [once you are done](#once-you-are-done)
 * [disclaimer and thanks](#disclaimer-and-thanks)


### Wat

The idea came after a chat with [katieamazing](https://github.com/katieamazing).

The goal is to have fun changing the source code of a famous library, in such a way that

 * tests still pass
 * it is much more difficult to understand what is going on
 * the whole process is fun

The ideal setup is to pair program on this, one small change at a time.

A couple rules:

 * no automatic code obfuscation library should be used, that's not as fun
 * dont refucktor tests, you want the poor thing to be in a working condition


### The code

I took code from [lazy.js](https://github.com/dtao/lazy.js), I chose it over other repos because
of its high quality code, since we're going to mess up some code it felt like a great starting point:
it's so easy to refucktor something that's so well written.

People can choose to refucktor from one of the follow types, whichever they feel will let them
have the most fun, the names might look scary to a developer, but nothing scares a refucktorer:

 * [from Software Engineer to Senior Refucktorer] - ArrayWrapper AssignSequence
 * [no refucks are given today] - ZippedSequence ShuffedSequence
 * [lol wat] - UniqueArrayWrapper WatchedPropertySequence

It's not so important to understand the code to refucktor it, you could say it could help
create really refucktored code, but no worries, the goal is to have fun, which is why
I did not use adjectives like "easy", "difficult", "medium", and so on.


### How to refucktor

Pick a category, let's say "lol wat", then pick a type, let's say "WatchedPropertySequence", have a look
at the code to understand what you're dealing with (or not), apply a refucktor that makes you giggle,
or just write whatever you think would be fun, then run tests.

Remember that a Senior Refucktorer always tests their code, so:

 * pick some code
 * refucktor
 * run tests (always work with green tests, undo your refucktor if they are red)


### Once you are done

Once you feel you've refucktored enough run this command at the root of the project

```bash
$ git diff >refucks/your-pair-name.patch
```

Instead of `your-pair-name` choose a suitable, funny name; that command will generate a patch
so that other people can execute this command


```bash
$ path -p1 <refucks/your-pair-name.patch
```

and have a look at what improvements you made!


### Disclaimer and thanks

The code from lazy.js has been altered beyond usefulness and perhaps recognition, please
don't use this for anything that's "serious stuff".

Thanks a lot to [the original author](https://github.com/dtao) for the quality code they provided.
