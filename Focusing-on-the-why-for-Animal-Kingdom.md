This page forms part of the [[Focusing on the Why]] series. It presents a comparison to the Animal Kingdom.

# Introduction

Note: In deciding which stage a particular animal / insect fits, I'm trying to answer a very specific question:
- What's the simplest architecture that could emulate the behaviours?
Thus, a fly, for example, may employ attention control, but it may not. So I will assume for now that it does not, until I find a strong reason to believe that it needs attention control and for what reason.


# Background

To discuss:
* sensor-adjustor-effector biologies
    * See https://journals.biologists.com/jeb/article/214/8/1215/10743/Do-jellyfish-have-central-nervous-systems, and https://www.sciencedaily.com/releases/1999/04/990415064510.htm, in note: "Biol. Summ. - Animals and Evolution"


# A Progression through the Biological Kingdom

## Plants

These use hormonal (ie: chemical) signalling. While there is a level of macro-scale feedback, it is via a sense-infer-act-outcome cycle, rather than a pre-action cognitive feedback. Thus, it is of the form of a feedforward-only network.
In other words, our current "state of the art" deep neural networks, are just scaled-out versions of plant-cognition.

## Plankton and single-celled organisms

Background:
- See note "Biology Summary - Animals"
These have extremely simple nervous systems, including cases where the sensory nerve directly controls the effector.

## Jellyfish

Background:
- See note "Biology Summary - Animals"
Classification:
- Box jellyfish hunt prey, which requires more complex behaviour. They also have multiple distinct overlapping networks, which could be examples of centralised control and/or predictive coding feedback loops.
- All other jellyfish seem to be pretty much very simple feedforward reactive machines.

## Flies

Background:
- See note  "Biology Summary - Animals"

Flies nervous system could be a very simple combination of the following main features:
- Primarily genetically hard-coded, with minimal post-birth learning.
- Examples of genetically hard-coded behaviours:
	- Olfactory sense triggering flight response towards smell for specific smells. The smell that draw flies are a fairly straightforward chemical signal that are consistent across time.
	- Vision of fast moving object comings towards fly triggering flight away (threat response).
- Main learning occurs via predictive-coding processes.
- Predictive-coding + afference copy to identify the difference between self-caused visual change versus external environmental changes.

The above can even cope with simple associative learning, eg: learning that one side of a chamber is too hot, and thus avoiding it. With reference to this study;
- Williams-Simon, P.A., Posey, C., Mitchell, S., Ng'oma, E., Mrkvicka, J.A., Zars, T., King, E.G. Multiple genetic loci affect place learning and memory performance in Drosophila melanogaster (2019) Genes, Brain and Behavior, 18 (7), art. no. e12581. https://doi.org/10.1111/gbb.12581

The next "why" question receives some answers from the following question:
- If a flies behaviour was entirely genetically hard-coded, with no learning even from birth, what would it be missing?
- What learning is required to support adaptation?
- What learning is required because it would be more efficient / accurate to learn post-birth rather than being genetically hard-coded?

However, I think I saw an article that found that flies have attention too.

Plus, while the behaviours of a fly may seem simple, the environment that they operate in is almost as complex as it is for humans. So in practice they may need many of the same systems.