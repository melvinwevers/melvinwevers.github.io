---
title: "Deterministic code, probabilistic meaning: on translating research back and forth with LLMs"
description: "Why LLM-mediated research makes theory and explicitness more important, not less"
date: 2026-11-15
author: Melvin Wevers
tags: [computational history, LLMs, reproducibility, theory, methodology]
draft: false
---

Recently I had a conversation about how large language models are changing the way we do research, and one distinction kept coming back. Code is deterministic. Language, and the conceptual thinking we do in it, is probabilistic. Code runs. Language has to be interpreted. I have come to think this distinction is useful but slightly wrong, and the way in which it is wrong matters.

In computational history we constantly move between these two registers. I write a script that counts words in digitized newspapers, classifies photographs or extracts fields from housing registration cards. Given the same input, it produces the same output. Then I look at the result and have to decide what it means. Is a spike in a word frequency a shift in public discourse, or a change in how a newspaper was digitized? The first step is mechanical. The second is interpretation.

## Working one level up

Until recently, getting from a research question to working code meant writing the code yourself. This was slow, but it forced every decision into the open. You cannot tell a for-loop to "find the relevant passages." You have to define what relevant means.

Now I increasingly describe what I want in natural language and let a model write the code, or do the classification directly. This is very productive. But the model still has to decide what relevant means. It just no longer asks me.

This is where the opposition between deterministic and probabilistic stops being helpful. Randomness is the smaller problem: I can fix the settings so that a model returns more or less the same labels every time. A model that always gives the same answer has still made an interpretive decision that I cannot read anywhere. What code gave us was never only determinism. It was explicitness: the decision is written down, and someone else can disagree with it. The distinction that matters is between what is explicit and what stays implicit.

## The missing piece: theory

If writing code becomes cheap, the bottleneck moves to knowing what to ask. This is where theory comes in. By theory I mean a framework from which we derive hypotheses that we test against data, in our case historical data. A theory defines its concepts sharply enough to say what counts as an instance, what counts as evidence, and what would count against you.

History has an uneasy relationship with theory in this sense. Historians work with plenty of concepts, interpretive traditions and narratives, but rarely with explicit frameworks that generate testable expectations. Most historical work is inductive: we read, we notice patterns, we interpret. That has real strengths, and I am not arguing against exploration. But in a workflow that runs through language models it has a cost.

The concepts in a prompt effectively become the program. If they are vague, the model fills the gap with the average, present-day meaning of a category in its training data. Gadamer argued that we never read a source without such a horizon of our own, and that understanding happens when the source puts our expectations at risk. A model cannot put its horizon at risk. We can, but only if we know what we expected. This is what I want from theory: not a method that replaces interpretation, which Gadamer distrusted, but our expectations written down so that the sources can contradict them.

## The lossy return trip

The movement between code and interpretation runs in two directions, and they are not equally hard. The first runs from computational output to meaning: deciding what a spike in word frequencies, a cluster of images or a set of model labels tells us about the past. Historians are trained to read sources critically, not model outputs, so even this step requires a new kind of source criticism.

The second direction, from interpretation back to code, is harder. Once I have an insight, a better understanding of a category or a sense that a pattern means something, I can only partly translate it back into code. That a source is ironic, or that a term carried a specific political charge in a specific decade, does not reduce neatly to a rule or a prompt. Every time an interpretation becomes an operation, something is lost.

If the translation is always partial, why insist on it?

## Why we still have to do it

Because of reproducibility. But we have to be precise about what that means. It cannot mean that someone else arrives at exactly the same interpretation. It means that our decisions can be inspected: what we decided a category meant, which sources we included, which thresholds we set. And the loss in translation is no reason to skip it. Only by attempting the translation do we find out what resists it. That remainder is not a failure. It is where the interpretive work of the historian happens, and it should be described, not hidden inside a prompt.

In practice, this asks three things of computational historians. Say before you test what you expect and what would count against it; explore freely, but do not present what exploration turned up as if it were a test. Store the prompts, the model version and the outputs themselves, because the model you used may not exist next year. And read a sample of the sources yourself, compare your reading with the model's labels, and report the disagreement. That number is the loss in translation made visible. None of this requires better models. It requires being explicit about exactly those parts of our work that LLMs make it easy to leave implicit.
