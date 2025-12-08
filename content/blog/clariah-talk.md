---
title: "Rethinking Digital Infrastructure: What a Computational Historian Needs"
description: keynote at Clariah Community Event
date: 2025-12-08T12:14:05+01:00
draft: false
tags: []
---

__These are slightly edited speaking notes.__
_You can find the slides [here](https://hackmd.io/FqFJRmCWQfq9Tf3ZRRM4tQ?view)_


I have a confession. I've never successfully used a CLARIAH tool in my research.

And it's not because I don't do computational work, I do, constantly. Right now I'm using visual language models to transform archival collections from the Amsterdam City Archive into structured data. I'm analyzing bias in the National Archives' photo collections: thousands of images, examined with diversity metrics borrowed from ecology. I teach digital history courses where we critically examine Delpher.

## What I Actually Use

So what do I actually use for this work? SURF's Snellius supercomputer for compute. Hugging Face for models. Python libraries, such as Pandas, PyTorch, transformers. GitHub for version control. Jupyter notebooks for reproducible workflows.

This infrastructure exists. It works. Dutch researchers have access to compute through SURF.

But here's the problem: when I want to use these tools on Dutch heritage collections, I'm on my own. There's no bridge between the collections CLARIAH provides access to and the computational infrastructure I need to analyze them. I end up building everything from scratch, finding data, downloading it manually if I can, converting formats, writing my own pipelines.

CLARIAH and SURF exist in parallel universes. And that gap is where computational humanities research gets stuck.

Let me tell you what I've actually experienced.

## Three Problems

Three problems. Discovery, access, and compute.

**Discovery**. CLARIAH provides access to heritage collections through the Media Suite, but often only to metadata, not actual materials. I've tried DANS Dataverse repeatedly. Rarely do I get data in forms I can actually work with.

In preparing this talk, I searched Ineo—CLARIAH's discovery tool—for datasets I could use. Most links didn't work. Some datasets were too specific and small-scale. Others just pointed to archive inventory pages. It's a catalog telling me where things exist elsewhere, without access to them. That's not infrastructure—that's a phone book.

**Access**. Even when you find something, getting to work with it computationally is difficult. The Media Suite has API access. I requested it. Never received it. You can work with multiple collections—but the process of building a corpus is convoluted. Too many steps, too many interfaces, too much friction.

What I need is simple: data in formats I can work with. Downloadable. Documented. Standard formats. And—this is crucial—the ability to compare across multiple datasets easily. Real historical research requires comparison. The infrastructure should make that straightforward, not painful.

**Compute**. Beyond discovery and access, there's working at scale. Virtual Research Environments don't support the type of work I do. There's no way to run models over collections. I need to build my own corpora using sampling strategies. Assess representativity. Create custom visualizations. Validate results.

These are standard computational methods. But they require bulk data access, compute resources, and integration with tools researchers already use.

Now, I know there are copyright constraints. I've worked on this—I was part of a Tools2Data project with CLARIAH and KB, specifically trying to find ways to run code on copyrighted material and return only features and analytical results. Together with my colleague Thomas Smits, I've proposed a work package for CLARIAH Prime to make the KB's magazine collection accessible through document segmentation and multimodal search and analysis.

So I'm not just criticizing from the outside. I know people within SURF and CLARIAH are thinking about these issues. Solutions exist. API access with authentication. Working with embeddings rather than raw text. Secure computational environments. But progress is slow.

Here's what troubles me. If a computational historian working on Dutch collections has never successfully used CLARIAH infrastructure—what does that tell us about who it actually serves?

##  What Infrastructure Should Be

And let me be precise about what I mean by infrastructure. I'm not asking for more specialized tools. Another parser. Another annotator. Another visualization platform. I'm talking about infrastructure: access to data, access to compute, access to models and methods, ways to share knowledge.

Good infrastructure should be invisible. You shouldn't need to learn "CLARIAH tools" as a separate skillset. It should just enable you to use your own tools and methods on important collections.

## The Macroscope Opportunity

The Macroscope. This is both an extraordinary opportunity and a critical test case for how we build humanities infrastructure.
The numbers are impressive. €16.8 million from NWO's National Roadmap. Fourteen Dutch universities. Major partners—Statistics Netherlands, SURF, the eScience Center, KB, Sound and Vision, the KNAW Humanities Cluster. Coordinated by Erasmus University Rotterdam.

Four components: secure data vaults, unified data sources combining survey and archival materials, AI tools developed for research, and a public access portal.
The ambition? The world's first population-level research infrastructure. Researchers could link and analyze massive datasets spanning social, cultural, and digital domains—across the entire Dutch population.

###  The Big Questions

What excites me most is the collaboration between ODISSEI and CLARIAH. Social sciences and humanities, working together. That's genuinely new. But here's my concern: this collaboration only works if humanities researchers can engage with questions that require quantification. Modeling. Computational methods.

Social scientists bring established approaches. Network analysis with proper metrics. Topic modeling with statistical rigor. Causal inference. Theoretical frameworks for testing mechanisms. Humanities needs to be able to do this work too. Not instead of contextual interpretation—as a complement to it.

Look at the research questions in the announcement. How do ideas flow across communities? How does trust form between neighbors? How are collective memories shaped? How does misinformation ripple through conversations?

These are structural questions. They're asking about relationships, positions, configurations—not just content. You cannot answer these questions by reading individual texts, no matter how carefully. The structure only exists at aggregate scales.

### Scale Matters

Let me explain what I mean by that.

Think about temperature. Temperature doesn't exist in a single molecule. It's a property that emerges from molecular ensembles—from aggregation.

Historical phenomena work the same way. You cannot see how parliamentary debates fragment into specialized communities by reading individual speeches. That network modularity only becomes visible when you analyze thousands of speeches together. You cannot identify how information cascades through a network by examining single documents.

These are emergent properties. They exist only at particular scales. And that means for certain research questions, computational infrastructure isn't just convenient—it's epistemologically necessary.

### The Problem in DH

Now, I'll be honest about something uncomfortable.

In digital humanities, we don't always do this well. Some researchers do rigorous quantitative work. But too often, we eyeball network visualizations without calculating the metrics that would tell us what the structure actually means. We read topic models impressionistically without assessing coherence or validating whether they capture meaningful patterns.

And when challenged? We sometimes retreat to: "History is complicated. Context matters. Every case is unique." That sounds sophisticated. But it ends the conversation rather than deepening it.

The Macroscope collaboration with social sciences requires rigor. Baselines to assess whether changes are significant or just noise. Statistical frameworks. Proper validation. Not as a replacement for contextual understanding—as its foundation.

### The Risk

So here's my concern. If the Macroscope follows the pattern we've seen before—elaborate discovery systems, annotation tools, beautiful interfaces, but not the computational access that rigorous quantitative work requires—what happens to humanities?

We risk becoming the people who provide context. Interpretation. Color commentary. Not full partners in the computational research itself.

## What Research Actually Needs

Think about what these research questions actually require.

"How are collective memories shaped?" That might involve agent-based modeling—simulating how individual memory practices aggregate into collective narratives.

"How does misinformation ripple through conversations?" That requires diffusion modeling on social networks. Data on who talks to whom. Temporal analysis of when information spreads. Statistical models to distinguish viral spread from background noise.

We don't know yet which methods will prove most productive. That's what research is for. But we do know you can't explore these questions by clicking through search results. Researchers need programmatic access to experiment with different approaches. Compute resources to test models. Statistical frameworks to assess significance.

So my question is this:

Will the Macroscope be infrastructure for computational humanities research? Or will it be another discovery interface?

## What Works: Learning from Existing Infrastructure

I've spent a lot of time on what doesn't work. Let me show you what does. Not perfect solutions—but examples that demonstrate principles the Macroscope could adopt.

**Impresso**. The [Impresso project](https://www.impresso-project.ch) processes historical newspapers across Switzerland and Luxembourg. Their key innovation? Multiple access points to the same infrastructure. They have a web interface for exploration—fine, good. But they also have the Impresso Datalab: a Python library and public API. You can write code to query their corpus. Their trained models—word embeddings, named entity recognition, topic models—are published on Hugging Face. They share example Jupyter notebooks on GitHub showing complete workflows.

The principle: support the full research pipeline. Explore through the interface, export to notebooks for systematic analysis, access the underlying embeddings, integrate with your own tools. One infrastructure, many entry points.

**UCLOUD** in Denmark. [UCLOUD](https://cc.au.dk/en/cdmm/tools-and-tutorials/data-handling/ucloud) demonstrates something important: infrastructure isn't just technical resources. It's knowledge infrastructure. They provide compute designed for humanities scholars. NetLogo for agent-based modeling. VS Code for development. Jupyter notebooks. All through a web interface.

But—and this is crucial—they also provide training. Summer schools. Winter schools. Documentation that makes sense to humanities scholars. Example projects showing how others solved similar problems. Infrastructure only works if researchers know how to use it. That sounds obvious. It gets forgotten constantly.

**Hugging Face and Google Colab.** These platforms show what frictionless sharing looks like. [Daniel van Strien](https://huggingface.co/davanstrien) at Hugging Face is a good example. He's fine-tuned vision-language models for heritage collections. Made British Library digitized books accessible as datasets. Shared models for working with OCR text from historical sources.

Everything is immediately usable. You find the model, the paper explaining it, working code you can run. No request forms. No waiting for access. You can run it on their servers. There's some environment configuration, but with tools like UV it's become much easier.

Google Colab demonstrates accessibility without institutional barriers. My students in digital history can experiment with language models on historical texts without installing anything. Without requesting cluster access.

### The Pattern

So what's the pattern here? Programmatic access alongside interfaces. Trained models and embeddings shared as infrastructure. Workflows documented as working code. Integration with tools researchers already use. Minimal friction between discovering a method and actually using it.

The Macroscope doesn't need to replicate these platforms. It needs to adopt these principles.

### Building Around Capability, Not Questions

Now let me show you a contrasting pattern. One I hope the Macroscope avoids.

Too often, we build infrastructure around what's technically feasible rather than what research requires.

Take linked data. We've invested enormous effort in semantic webs and complex ontologies. This work has value—structured metadata matters. But sometimes we go too far. Elaborate ontologies proliferate while researchers still can't easily access the actual data to run analyses. We've focused on describing data rather than enabling computation with it.

Or take entity detection. We invest huge effort in identifying people, places, organizations in texts. Then we add these as filters to search interfaces. But why do we need this information? For what research questions? What hypotheses does it let us test?

### Discovery vs. Structure

Here's what I notice. We're building tools that help us find and describe things—entities, documents, structured metadata. But not infrastructure that reveals relationships. How concepts cluster. How information flows temporally. How network position shapes discourse. We're optimizing for discovery when many computational research questions require analyzing structure.

That's the fundamental choice the Macroscope faces: build around technical capabilities, or build around research questions.

## Five Recommendations for the Roadmap

You've been discussing the CLARIAH roadmap this morning. The Macroscope represents a major new direction. Let me offer five concrete recommendations.

**One**. APIs alongside interfaces. Every collection, dataset, and model should have robust programmatic access. The Media Suite shows you can build good interfaces. Now make sure every interface has an equally good API.


**Two**. Share models as infrastructure. When collections are processed, publish the models. Put them on Hugging Face. Share the embeddings. Share the training pipelines. When CLARIAH invests in processing a collection, that investment should become infrastructure for the whole field. Not just one project's output.

**Three**. Provide compute resources. If the Macroscope aims to bridge humanities and social sciences, researchers need compute for network analysis, statistical modeling, agent-based simulation. That means resources that integrate with scientific computing frameworks. Not just web interfaces.

**Four**. Document with working code. Alongside traditional documentation, provide example notebooks on GitHub. Complete workflows. Make them runnable in Colab or Binder so researchers can try them immediately. Don't just tell people what's possible. Show them.

**Five**. Integration over invention. Connect to existing platforms researchers already use. Snellius for compute. Hugging Face for models. Zenodo for datasets. GitHub for code. Don't make researchers choose between their workflows and CLARIAH data. Meet them where they are.

### What CLARIAH Has Built

Now, let me acknowledge what CLARIAH has built successfully. The [Media Suite](ttps://mediasuite.clariah.nl) provides access to important audiovisual collections. The linguistic tools serve their communities. Federated search is valuable. This is real infrastructure serving real needs.

I'm not here to tear that down. But as we build the Macroscope, we need to expand the vision.

From providing access to collections—to enabling computational research at scale.

From building specialized tools—to providing building blocks.

From creating platforms—to integrating with ecosystems.

This isn't about efficiency. It's about making certain kinds of research possible at all. Research that requires working at scales where structure becomes visible.

## Closing: Infrastructure for Whom?

The Macroscope is an extraordinary opportunity. The ambition is right. The collaboration between ODISSEI and CLARIAH is right. The focus on linking social, cultural, and digital data is right. But we need to be honest about who it's for. And how they actually work.
If it's for traditional humanities scholars who need better search and access to collections—build accordingly. But if it's for computational research—and the language about AI tools, population-level datasets, quantitative methods suggests it is—then it needs to work the way computational researchers work.

I've never successfully used CLARIAH infrastructure. Not because I don't care about Dutch collections. Not because I'm not doing computational humanities. But because it wasn't built for how I do research. The Macroscope could change that. But only if we rethink what humanities infrastructure means in a computational age.

- Collections as analyzable data.
- Integration with existing ecosystems.
- Shared models as infrastructure.
- Programmatic access as standard.
- Working code as documentation.

The afternoon sessions will explore concrete needs around learning, AI, and data flows. I hope we can have honest conversations—about who this infrastructure serves, and how it needs to work differently.

Thank you.
