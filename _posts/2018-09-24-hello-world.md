---
layout: post
title: "Measuring Semantic Coherence of a Conversation"
tagline: "ISWC 2018"
category: 
tags: []
---
{% include JB/setup %}

Imagine: you sit in a train, in which many different conversations are going on at the same time. A couple next to the window is planning their honey-moon trip; the girls at the table are discussing their homework; a granny is in a call with her great-grandson. You close your eyes and try to recover who is talking to whom by paying attention to the content of the conversations and not to the origin of the sound waves:

- Mhm .. and then we add the two numbers from the Pythagoras’ equation?
- … but I am not quite sure about that hotel you booked on-line… Don’t you think we should stick with the one we found on Airbnb?
- All right, sweetheart, kiss your mum for me! I will be back before the Disney movie starts, I promise.
- I think it is the one we did on the blackboard on Monday or was it the one with Euclidean distance?
- For me both options are really fine as long as it is on Bali.

It is relatively easy to tell the three conversations apart. We hypothesize that this is due to certain semantic relations between utterances from the same dialogue that make it meaningful, or <b>coherent</b>, which brought us to the following set of questions:

    1. What are the relations between the words in a dialogue (or rather the concepts they represent) that make a dialogue semantically coherent, i.e. making sense? and
    2. Can we use available knowledge resources (e.g. a knowledge graph) to tell whether a dialogue makes sense?

The later is particularly important for dialogue systems that need to correctly interpret (model) the dialogue context and produce meaningful responses.


![Illustration (c)[Zvisno](https://twitter.com/zvisno)](/assets/iswc18.png)


To study these two questions we cast semantic coherence measurement task as a classification problem with the learning objective to distinguish real (mostly) coherent dialogues from artificially generated dialogues incoherent by design. Intuitively, the classifier shall be trained to assign a higher score to the coherent dialogues and a lower score to the incoherent (corrupted) dialogues.

We extend the [Ubuntu Dialogue Corpus](https://github.com/rkadlec/ubuntu-ranking-dataset-creator) by generating negative samples to provide a benchmark for evaluation of different approaches. We implement and evaluate three approaches using this benchmark. Two of them are based on a neural network classifier (Convolutional Neural Network) using word or, alternatively, Knowledge Graph embeddings; and the other one is using the original Knowledge Graph (Wikidata+DBpedia converted to HDT) to induce and analyse a semantic subgraph representation for each of the dialogues.


## Resources


The paper is presented in the [International Semantic Web Conference (ISWC’18) on October 10 at 2pm in the Fred Farr Forum room](http://iswc2018.semanticweb.org/sessions/measuring-semantic-coherence-of-a-conversation/)

The preprint is available online: <https://arxiv.org/pdf/1806.06411.pdf>
and the code is open-sourced: <https://github.com/svakulenk0/semantic_coherence>



This research is a product of collaboration between the University of Amsterdam (UvA), Fraunhofer Institute in Sankt Augustin and WU Wien. I am grateful to all my co-authors for the valuable inputs, which enabled this publication.

## Reference

Svitlana Vakulenko, Maarten de Rijke, Michael Cochez, Vadim Savenkov, and Axel Polleres. Measuring semantic coherence of a conversation. In Proceedings of the 17th International Semantic Web Conference (ISWC 2018), Lecture Notes in Computer Science (LNCS), Monterey, CA, October 2018. Springer. to appear.

```
@inproceedings{Vakulenko2018MeasuringSC,
  title={Measuring semantic coherence of a conversation},
  author={Svitlana Vakulenko and Maarten de Rijke and Michael Cochez and Vadim Savenkov and Axel Polleres},
  booktitle={The Semantic Web - {ISWC} 2018 - 17th International Semantic Web Conference, Monterey, California, USA, October 8-12th, 2018, Proceedings},
  year={2018}
}
```
