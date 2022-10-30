---
title: How to write good prompts - notes on Andy Matuschak's article
date: "2022-9-6T22:40:32.169Z"
description: Article about writing good Anki-type questions
---

### ***The central role of retrieval practice***

> The value of fluent recall isn’t just in memorizing facts. Many of these experiments tested students not with parroted memory questions but by asking them to **make inferences, draw concept maps, or answer open-ended questions.** In these studies, improved recall translated into improved general understanding and problem-solving ability.
> 

***Re-reading is passive learning***

> Simply reminding yourself of material (for instance by re-reading it) yields much weaker memory and problem-solving performance.
> 

***Active recall is learning, unlike from school assessing***

> The learning produced by retrieval is called the “testing effect” because it occurs when you explicitly test yourself, reaching within to recall some knowledge from the tangle of your mind.
> 

## Retrieval practice prompts should:

---

### be **focused.**

A question or answer involving too much detail will dull your concentration and stimulate incomplete retrievals, leaving some bulbs unlit.

It’s usually best to focus on one detail at a time.

### be precise.

Vague questions will elicit vague answers, which won’t reliably light the bulbs you’re targeting.💡

### produce consistent answers.

lighting the same bulbs each time you perform the task

Otherwise, you may run afoul of an interference phenomenon called “retrieval-induced forgetting”

### be tractable - разрешимый.

You should strive to write prompts **which you can almost always answer correctly.**

This often means breaking the task down, or adding cues.

### be effortful.

You shouldn’t be able to trivially infer the answer. Cues are helpful, as we’ll discuss later—just don’t “give the answer away.”

That’s one motivation for spacing reviews out over time: if it’s too easy to recall the answer, retrieval practice has little effect.

## ↑

> Achieving these properties is mostly about writing tightly-scoped questions.
> 

### *Writing tightly-scoped questions is surprisingly difficult.*

> You’ll need to break knowledge down into its discrete components so that you can build those pieces back up as prompts for retrieval practice.
> 

<aside>
💡 This decomposition also makes review more efficient.

</aside>

### Two skills to write effective retrieval practice prompts:

---

1. How to characterize exactly what knowledge we’ll reinforce?
2. How to ask questions which reinforce that knowledge?

> Whenever I was making anything complex, I’d constantly pause to consult references, which made it difficult to move with creativity and ease. I rarely felt “flow” while cooking. My experiences felt surprisingly similar to my first few years learning to program, in which I encountered exactly the same problems.
> 

# Let’s Practice!

## Simple facts

---

```abap
Q. What type of chicken parts are used in stock?
A. Bones.
```

```abap
Q. Why do we use bones to make chicken stock?
A. They’re full of gelatin, which produces a rich texture.
```

*and more focused:*

```abap
Q. How do bones produce a chicken stock’s rich texture?
A. They’re full of gelatin.
```

## Lists

---

*From here, we might ask:*

```abap
Q. What are typical aromatics used in chicken stock?
A. onion, carrots, celery, garlic, and parsley
```

*Unless you’re an experienced cook, you’ll probably find this prompt intractable, or you may remember ingredients inconsistently.*

**So, one good strategy is to create “fill missing” list:**

```abap
Q. Typical chicken stock aromatics:
* ???
* carrots
* celery
* garlic
* parsley
A. Onion
```

```abap
Q. Typical chicken stock aromatics:
* onion
* ???
* celery
* garlic
* parsley
A. Carrots
```

<aside>
💡 In the software interfaces, these prompts are often called “cloze deletions.”

</aside>

Another way to help yourself understand lists like this is to write explanation prompts for each of the components:

```abap
Q. Why is carrot a good aromatic for chicken stock?
A. Carrot provides vegetal sweetness; like salt,
this sugar brightens other flavors.
```

<aside>
💡 Explanations make knowledge more meaningful

</aside>

## ****Cues and elaborative encoding****

---

```abap
Q. Typical chicken stock aromatics:
* onion
* carrots
* celery
* garlic
* ??? (herb)
A. Parsley
```

```abap
Q. Typical chicken stock aromatics:
* onion
* ??? (rhymes with parrots)
* celery
* garlic
* parsley
A. Carrots
```

*Add mnemonic to the answer:*

```abap
Q. Typical chicken stock aromatics:
* onion
* ???
* celery
* garlic
* parsley
A. carrots (rhymes with “parrots”: picture a flock of parrots flying 
with carrots in their mouths, dropping them into a pot of stock)
```

<aside>
💡 You make information easier to recall when you connect it to other memories. This process is called **elaborative encoding.**

</aside>

Y*ou can add a prompt specifically intended to **reinforce the association:***

```abap
Q. Mnemonic device for carrots in chicken stock?
A. rhymes with “parrots”: picture a flock of parrots flying with 
carrots in their mouths, dropping them into a pot of stock
```

*Add imagery to your prompts:*

- Q. Chicken stock ingredients:

![https://andymatuschak.org/prompts/aromats-cloze.jpg](https://andymatuschak.org/prompts/aromats-cloze.jpg)

- A. Carrots

![https://andymatuschak.org/prompts/aromats.jpg](https://andymatuschak.org/prompts/aromats.jpg)

---

> Of course, cues and elaborative encoding add extra effort. *You don’t need to use them all the time:* you’d probably find that exhausting. But they’re useful techniques to deploy if you suspect a prompt will prove difficult to remember, or if you’ve noticed yourself struggling in practice.
> 

---

- **How might you make a mnemonic device feel vivid? (name at least two ways)**
    
    e.g. visuals, personal experiences, humor, disgust
    

## ****Interpretation; the “more than you think” rule of thumb****

---

<aside>
💡 Writing good prompts often involves **interpretation**: extracting information which isn’t explicitly written.

</aside>

***Examples for a chicken stock;** some in terms of ratios:*

```abap
Pound of bone, half an onion, quart of water, A smashed clove per pound
```

> Prompts seem to carry a per-unit “price,” so people naturally try to write fewer questions which cover more ground. *But that’s **counter-productive.***
> 

### Prompts are cheaper than you probably imagine.

> Rule of thumb: ***write more prompts than feels natural.***
> 

### Prompts are cheap, but they’re not *free.*

> They have time and emotional cost.
So for familiar subject use fewer prompts.
> 

---

<aside>
💡 As you build fluency in increasingly complex concepts, you can write increasingly complex prompts while keeping each focused on what feels like a single detail.

</aside>

- **What cognitive factor does the appropriate scale of a ‘focused’ prompt depend on?**
    
    The scale of the concepts you’ve internalized (aka ‘chunk size’)
    

## Procedural knowledge

---

Let’s look at the steps of the recipe. This is *procedural knowledge*—knowledge needed to perform specific tasks, ***more knowing how than knowing what.***

---

*We may use cloze deletions:*

```abap
Q:
	1. ???
	2. Bring to a simmer on low heat (this will take about an hour). 
	We use low heat to produce a bright, clean flavor: at higher
	temperatures, the stock will both taste and look duller.
	3. Lower heat to maintain a bare simmer for an hour and a half.
	4. Strain, wait until cool, then transfer to storage containers.
A. Combine all the ingredients in a large pot.
```

> This is an *awfully unfocused prompt*. It includes many unimportant details which distract from the knowledge you actually intend to retrieve. In my experience, wordy prompts like these tend to dull my concentration and produce vague, distracted answers.
> 

*We can improve this prompt somewhat by simply removing words:*

```abap
Q:
	1. ???
	2. Slowly bring to a simmer
	3. Maintain bare simmer for 90m
	4. Strain, wait until cool, then store
A. Combine all ingredients
```

> If you know what stock is: the first and fourth steps aren’t worth writing prompts about.
> 

---

*Explanation type prompts are good to avoid rote learning and build a deeper understanding.*

```abap
Q. Why does Andy’s recipe claim we should prepare chicken stock over low heat?
A. “Brighter, cleaner” flavor.
```

## ****Exercise: how to store chicken stock?****

---

**Paragraph:**

This will yield about 1.5 qt. Chicken stock will keep for a week in the fridge or indefinitely in the freezer. Once chilled, there will be a cap of fat on the stock; skim that off before using the stock, and deploy the fat in place of oil or butter in any savory cooking situation.

---

And it’s **Prompts:**

```abap
Q. 2 lbs of chicken bones yields roughly ??? qt stock
A. 1.5 qt

Q. ??? lbs of chicken bones yields roughly 1.5 qt stock
A. 2 lbs

Q. How long will chicken stock keep in the fridge?
A. A week

Q. How long will chicken stock keep in the freezer?
A. Indefinitely

Q. Once chilled, what should I do before I use a fresh batch of chicken stock?
A. Remove the cap of fat

Q. What should I do with skimmed fat from chicken stock?
A. Keep and use as savory cooking fat
```

## **What stock is and why it matters: conceptual knowledge**

---

**I’ll now introduce some useful lenses for understanding concepts.**

---

### Attributes and tendencies:

What makes stock, stock? What’s always / sometimes / never true.

> Q. How are stocks usually made?
A. Simmering flavorful ingredients in water.
> 
> 
> Q. Why don’t stocks usually have a distinctive flavor?
> A. To make them more versatile.
> 

### Similarities and differences:

Knowing what relates and distinguishes if from other adjacent concepts.

> Q. How is stock different from soup broth?
A. Soup broth has a more complete flavor; stock isn’t meant to stand on its own.
> 

### Parts and wholes:

What are some examples of stocks? Are there important “sub-concepts” of stocks?

> Q. Name at least three examples of stock:
A. e.g. chicken, vegetable, mushroom, pork
> 
> 
> Q. Stock is rarely served directly; it’s best thought of as a ??? (construction metaphor)
> A. Building block.
> 

### Causes and effects:

What does stock do? What causes it to do that? What doesn’t it do? When is it used?

> Q. Why do restaurants use stock as a cooking medium instead of water? (name two reasons)
A. Adds flavor, improves texture.
> 
> 
> Q. Stocks are a common base for… (name at least two)
> A. e.g. sauces, soups, braises
> 
> Q. Restaurants often use stock as a cooking medium where home cooks might use ???.
> A. Water
> 

### Significance and implications:

Why does stock matter? What does it suggest? Make the concept personally meaningful.

> Q. What liquid building block explains why simple restaurant dishes are often tastier than home renditions?
A. Stock.
> 
> 
> Q. What should I ask myself if I notice I’m using water in savory cooking?
> A. “Should I use stock instead?”
> 

## Open lists:

---

> Q. Things to do with chicken stock:
> 
> - ???
> - wilt and steam hearty greens
> - make purée soups
> - deglaze pans
> 
> A. Cook grains in it
> 

Anything could reasonable go in that first slot. Order is not important. If you keep cooking, you’ll be adding to this list your whole life.

<aside>
💡 I like to think of open lists like *tags*
—like the tags you might use in a system for digital bookmarks.

</aside>

---

***How to deal with open lists? There is 3 ways:***

### prompts focused on each of the tagged items:

> Q. When puréeing vegetables to make soup, how can I produce a richer flavor without adding fat?
A. Thin the purée with chicken stock instead of water.
> 

### a prompt about a pattern in the tag:

> Q. What should I ask myself if I notice I’m using water in savory cooking?
A. “Should I use stock instead?”
> 

### a prompt which fuzzily links the tag to instances:

> Q. Name two ways you might use chicken stock.
A. e.g. cooking grains, steaming hearty greens, making purée soups, deglazing pans
> 

---

## BUT:

> Prompts like this usually *don’t work well without other prompts supporting it.* You’ll probably find yourself giving the same examples each time.
> 

> In the absence of additional prompts, you’ll likely forget about the other instances.
> 

### example-generating creative prompts:

> Q. Name a vegetable purée soup which you might try making with chicken stock (give an answer you haven’t given before)
A. e.g. potato, parsnip, celeriac, sunchoke, salsify, squash, carrot, pepper, lentil…
> 

*“give an answer you haven’t given before.” - that’s a trick.*

<aside>
💡 This isn’t really a retrieval prompt anymore. Creative prompts are more like a textbook exercise, asking you to apply what you’ve learned in a new way.

</aside>

> Unlike the other prompts we’ve seen, the goal here is to avoid retrieving an answer from memory: you’re meant to think creatively for a few moments. Since your answer’s different each time, retrieval practice won’t consistently reinforce your memory of any particular response. Instead, it will reinforce whatever knowledge you consistently use when ***generating*** an answer.
> 

## ****Salience prompts and the Baader-Meinhof phenomenon****

---

Have you ever heard about something for the first time, then suddenly noticed it everywhere? - it’s a *Baader-Meinhof Phenomenon.*

---

We’ve already written a few prompts which focus on salience:

> Q. What should I ask myself if I notice I’m using water in savory cooking?
A. “Should I use stock instead?”
> 
> 
> Q. What should I do with the carcass of a roast chicken?
> A. Freeze it and make chicken stock
> 
> Q. Name a vegetable purée soup which you might try making with chicken stock (give an answer you haven’t given before)
> A. e.g. potato, parsnip, celeriac, sunchoke, salsify, squash, carrot, pepper, lentil…
> 

<aside>
💡 It’s important to densely connect new ideas to old ones, as we did in the conceptual knowledge section: roughly speaking, more connections means more opportunities to trigger new knowledge.

</aside>

# Writing prompts, in practice.

---

### Iterative approach

On the first pass, aim to write a small number of prompts (say 5-10) about whatever seems most important, meaningful, or useful.

## Litmus test

---

*While you’re drafting prose, a spell checker and grammar checker can help you avoid some simple classes of error. Such tools don’t yet exist for prompt-writing, so it’s helpful to collect simple tests which can serve a similar function.*

### False positives:

*How might you produce the correct answer without really knowing the information you intend to know?*

- Discourage pattern matching: keep prompt simple, to not memorize the shape of that question and learn corresponding answer.
- Avoid binary prompts: with yes/no or this/that answer

### False negatives:

*How might you know the information the prompt intends to capture but fail to produce the correct answer? Such failures are often caused by not including enough context.*

Make prompts more precise, ***without alternative answers.***

---

### ****Revising prompts over time and editing them by the way****

Edit them by the review, if necessary delete them.

September 6, 2022 