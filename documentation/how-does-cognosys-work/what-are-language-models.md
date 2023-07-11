---
description: A brief survey over LLMs.
---

# 💟 What are language models?

## Language models are a type of algorithm. Here, we try to explain helpfully and clearly how they work.

**"Large language models"** are so-called because they are i) large, they are ii) language, and because they are iii) models:

1.  **large:**

    LLMs are _algorithms_ or mathematical calculations which take in input text as data, encoded in _binary_ format - 010111000 - and do a bunch of calculations on it to produce a result - also text encoded in binary - 0100111101 - that maps to letters, words, text, as a response.

    There are many algorithms that can do this, but one of the associated implications of this term, LLM, is how large they are. While there is no strict size cut-off for how big “big” needs to be, to be considered “big”, it can informally be compared to the size of these models (algorithms) in the recent past, indicating how much “bigger” they are.

    This “bigness” refers to a) the amount of data they have been trained on b) the number of calculations they do, on the data
2.  **language**

    Large language models (LLMs) are used with _language_. They are a sub-field in NLP, or _natural language processing_. Specifically, they use a machine learning architecture called _transformers_. Transformers are a type of **neural network** which includes a component nicknamed _attention_.

    Attention is a means by which the algorithm selects what context it uses for a given prediction, depending on what is being predicted. **Neural networks** are a particular method in statistics where data getting input into a calculation is _transformed_ by a particular series of calculations - adding, subtracting, multiplying, dividing, and exponentiating the data - to produce a particular result.

    The result is then compared to a reference value to check if it worked; if it did not, a calculation is used to change the neural network algorithm itself - the way it transforms the inputs - to bring it just slightly a little nearer to the “bullseye” - the target output it _should_ have predicted. Do this again and again, enough times - perhaps billions of times - and the model (algorithm) slowly adjusts and fine-tunes itself, until it is beginning to produce the desired output, time after time, like tuning a guitar so the strings are in harmony, or natural evolution by which a certain figure is arrived after compendious levels of reproduction, fine-adjustment, and reproduction.

    Large language models are merely transformers that are trained on language data, but the transformer architecture can be used on different types of input, as well.
3.  **models**

    Model is just a term within the community for “AI” or “algorithm”. Right now, there are different AIs, and different AI products. Some of them use the same _model_, behind the scenes - GPT-4, GPT-3, or others. Different models have different performance, characteristics, and behavior.

#### How do they understand language?

This is as open question, but the basic starting point is [**distribution**](https://en.m.wikipedia.org/wiki/Distributional\_semantics). **Everything** that all machine learning algorithms “learn”, “infer”, or _induce_, about language, comes from counting and tracking the occurrence of different words and symbols in relation to each other.

A simpler version of this is the [**n-gram**](https://en.m.wikipedia.org/wiki/N-gram), a technique for counting the co-occurrence of _pairs_ (or triplets, or groups) of words, within some distance from each other.

LLM’s scale this up a bit by using a slightly more complicated way of capturing the “context” - the regularly occurring “neighbors” - that different text, words, or sentences has - called an _embedding_, or a [_word vector_](https://en.m.wikipedia.org/wiki/Word\_embedding). This vector becomes literally a mathematical vector of 1’s and 0’s, which can be analyzed mathematically in a _vector space_, with the techniques of linear algebra.

One Twitter commenter wryly called them “[_post-structuralists_](https://en.m.wikipedia.org/wiki/Post-structuralism)”, because all of the patterns or relationships they are able to generate is based on external, rather than internal, dynamics between the words. Like [Derrida](https://en.wikipedia.org/wiki/Jacques\_Derrida), LLMs reflect what company a word keeps, their interplay - even at a distance - rather than “knowing” intrinsically by any means what a cat “is”.

Large language models are able to slowly be adjusted into calculations that produce seeming comprehension of their inputs because of [_induction_](https://en.m.wikipedia.org/wiki/Solomonoff's\_theory\_of\_inductive\_inference) - a much broader, and deep, topic in formal languages theory, logic, philosophy, logic, information theory, and theoretical computer science, building (partially) on work by people like Claude Shannon, Alan Turing, Noam Chomsky, Kurt Gödel, and the [**halting problem**](https://en.m.wikipedia.org/wiki/Halting\_problem), which has a strong relationship to questions about linguistics, the nature of the grammaticality, systematicity, and studyability of human language.

**Induction** is a question/theory about to what extent it is possible for a repetitive, specific procedure, over and over again, to figure out certain **patterns**, in _any_ input sequence of data. (It is a fascinating question).

**What this means is that large language models are like Google Translate on steroids.** Imagine a simple n-gram algorithm that has counted a common co-occurrence between the word _”the”_ and _”cat”_ - if we generated text by choosing the highest association the n-gram technique had found for any word, we may find this simple algorithm did pick up on some “patterns” that we recognize, or agree with.

But they would be simple, and there would be many more complicated relationships between words that it could not predict, because the way the idea of connections was “captured” was simply the co-occurrence of two words. In order to express more sophisticated relationships, it would be required to build a higher-order - more levels - _hierarchy_ of categories, groups, and concepts, in which to express those rules _in_.

For example, the basic “Newton’s laws” of modern syntax appear to be little formula, such as:

```
S -> NP + VP
NP -> D + N
N -> Adj + N
```

and so on. In phrase structure grammar, these notations are called “non terminal symbols”, because they represent units of the actual rule-system of language, but not the final layer when a transformation of grammar elements is finished, a sentence of actual words.

_Words_, like the ones we are using here, are called “terminal”, because they cannot be expanded anymore, but are the end result of transformation rules, such as the ones above.

This means that in phrase structure grammars, conventional notations like “NP” and actual words and symbols like the letter “C”, “hyacinth”, and so on, are accorded equal status in the sense that the rules of the system - (language) - are purely expressed as transformations on “symbols”.

You can see the connection with the algorithmic theory above, where we now hopefully see a way by which even a machine, a computer _for example_, could possibly produce grammatically correct sentences without “knowing” grammar, without “knowing” anything, because the grammar of sentences can be achieved by a set of unambiguous steps, requiring zero thinking, roughly:

```
replace symbol X with YZ
replace symbol Z with qq
replace qq with “chair”
```

**In order for an algorithm or a machine to be able to **_**induce**_** the processing or transformation rules on an input sequence, it will need to be able to sufficiently model the number of rules, symbols, or relationships that generated the input sequence.**

If the rules of human language are very complex, determined by innumerable connections of various kinds not only between words, but _higher level concepts_, concepts defined in terms of other concepts, themselves respectively defined in terms of other concepts, and so on.

I cannot understand the rule “You should capitalize the first letter of the first word of every sentence in English, except if it is a company name or proper noun that intentionally uses a lowercase first letter, _or_ you are speaking informally and don’t care too much about grammatical perfectness, or want to express that”, without already knowing the definitions for:

* capitalize
* letter
* first
* word
* sentence
* English
* except
* company
* name
* proper noun
* lowercase
* intentionally
* speaking
* informally
* express
* grammatical perfectness

And each of those things can be defined in terms of other categories, too. Which means: **the model has to be big enough to contain many, many relationships, many of which are “composite” or “high dimensional” in the sense that they are actually rules defined in terms of other rules, themselves defined in terms of yet other rules.** If the model isn’t big enough to model all those rules, it can’t reproduce the actual relationships in the data.

## Therefore,

Large language models calculate on words themselves, treating words like numbers, to produce a word as a result of the calculation. If a human wants to tune the calculation to produce _certain_ words - they have a preference - they train it on text data that they want the model to produce text like. If the number of calculations is sufficiently large, the algorithms can induce very higher-order relationships and come _closer_ to mirroring the actual rule system by which language works - how close they can come, is unknown.
