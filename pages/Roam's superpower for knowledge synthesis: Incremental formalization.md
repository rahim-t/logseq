---
title: Roam's superpower for knowledge synthesis: Incremental formalization
---

## Metadata::
### Author(s):: [[Joel Chan]]

### Type:: [[Blog post]]

### Abstract::
#### [[Joel Chan]] writes about incremental formalization and the potential that Roam has for structuring and synthesising knowledge.

### Topics:: [[Wissensmanagement]], [[_Exzerpte_Lektorat_fertig]]

### Date:: 2020

### Date added:: [[July 27th, 2020]]

### Zotero links:: [Local library](zotero://select/library/items/FSBLJP26), [Web library](https://www.zotero.org/users/4111725/items/FSBLJP26), [Chan_2020_Roam's superpow....pdf](zotero://open-pdf/library/items/IANZKQ5M)

### URL:: [https://www.roambrain.com/knowledge-synthesis/](https://www.roambrain.com/knowledge-synthesis/)

### tag:: #[[Exzerpt]], #[[ZoteroImport]]

## Notes::
### **[[Red Annotations]] (7/30/2020, 9:23:09 AM)**
#### "Formality Considered Harmful: Experiences, Emerging Themes, and Directions on the Use of Formal Representations in Interactive Systems (Shipman & Marshall, 1999)." ([Chan 2020:3](zotero://open-pdf/library/items/IANZKQ5M?page=3))

#### "there is now a Literature Reviewing channel on the Roam Slack team" ([Chan 2020:6](zotero://open-pdf/library/items/IANZKQ5M?page=6))

#### "Joel Chan provides a tour of his Roam database and describes his knowledge management processes in this very interesting video - www.youtube.com/watch?v=A6PIrVZoZAk" ([Chan 2020:7](zotero://open-pdf/library/items/IANZKQ5M?page=7))

### **[[Yellow Annotations]] (7/30/2020, 9:23:09 AM)**
#### "Synthesis is fundamental to knowledge work. […] synthesizers need to be able to compose individual ideas (evidence, hypotheses, concepts, claims) into a larger conceptually integrated understanding, such as a theory or argument. […] A typical form that scholarly/scientific synthesis takes is a literature review, but there are other more visual representations like causal models or diagrams […] synthesis representations: they go quite a bit further than simply grouping or associating things (though that is an important start). They have some kind of formal semantic structure (otherwise known as formality) that specifies what entities exist, and what kinds of relations exist between the entities." ([Chan 2020:2](zotero://open-pdf/library/items/IANZKQ5M?page=2))
:PROPERTIES:
:ID:999e2588-3448-49c4-86b0-d8feb5a14434
:END:

#### "Formal structures unlock powerful forms of reasoning like conceptual combination, analogy, and causal reasoning. This is a key part of the vision of projects like the Semantic Web. Judea Pearl makes this point quite emphatically, sketching out a "Ladder of Causation" that puts mere associationist reasoning at the bottom, and sophisticated counterfactual causal reasoning at the top, which requires a rich causal model (one kind of formal structure). […] How can we synthesize "raw" unstructured inputs like papers/observations into complex structured representations?" ([Chan 2020:2](zotero://open-pdf/library/items/IANZKQ5M?page=2))
:PROPERTIES:
:ID:effb1582-ecb3-4f59-a54b-d3f435df864f
:END:

#### "It's devilishly tricky to make systems that support formalism which users will actually use (without a gun to their head). Tools for synthesis that attempt to incorporate formalism typically have an extremely high barrier to entry and are an ongoing burden on the user. […] Formality Considered Harmful: Experiences, Emerging Themes, and Directions on the Use of Formal Representations in Interactive Systems (Shipman & Marshall, 1999). In brief, this paper identifies four classes of difficulties: 1. Cognitive Overhead (aka Cognitive Load): often the task of specifying formalism is extraneous to the primary task, or is just plain annoying to do. 2. Tacit Knowledge: if relevant information for developing formalism is tacit, asking people to formalize it will interrupt the task, with serious consequences for the quality of the work. 3. Enforcing Premature Structure: people don't want to commit until they're sure what formalism is actually useful for their task (and what's extraneous and only annoying). 4. Situational Structure: Useful structures and formalisms vary significantly across people, situations, and tasks" ([Chan 2020:3](zotero://open-pdf/library/items/IANZKQ5M?page=3))

#### "a powerful design pattern that can help address the problem of formality: incremental formalization. […] users enter information in a mostly informal fashion, and then formalize only later in the task when appropriate formalisms become clear and also (more) immediately useful." ([Chan 2020:4](zotero://open-pdf/library/items/IANZKQ5M?page=4))

#### "1. In the Hyper-Object Substrate system, users enter mostly informal text initially, and the system recognizes patterns in the textual information to suggest possible formal attributes or relations for the underlying knowledge base, which the user can then accept/modify/reject as they wish (p. 347). 2. Infoscope is a news reader system that suggests filters based on users' reading patterns; this helps them make their goals explicit which can facilitate formalization after it emerges from their task behaviors (p. 347-348). 3. VIKI is a spatial hypertext system that includes heuristic algorithms to find recurring visual/spatial patterns in layout of objects; users can use these to specify schemas if they wish. Another more recent example comes from Van Kleek et al (2007): their Jourknow system includes a variety of features that can recognize formal structure (e.g., location, time, meeting information) from (relatively) unstructured notes in pidgin or more lightweight entry format, such as Notation3" ([Chan 2020:4](zotero://open-pdf/library/items/IANZKQ5M?page=4))

#### "Incremental formalization addresses the cognitive overhead problem by spreading it throughout the task a bit more evenly, as well as removing it mostly from the earlier parts of the task, where minimal friction is needed to maximize exploration. It also helps with the premature and situational structure problems, since you don't have to commit early on to a structure that may not serve you well (or even hurt your performance) later on." ([Chan 2020:4](zotero://open-pdf/library/items/IANZKQ5M?page=4))

#### "[[Roam]] has the beginnings of (and high potential for powerful) incremental formalization […] The features in Roam that enable incremental formalization include: Unlinked references: initially write informally before you know a term is important, later turn into a formal link to a page Easily updated pages: don't worry about precisely naming something at first. Let the meaning emerge over time and easily change it (propagating through all references). Connected to this are Andy Matuschak's comments about contextual backlinks bootstrapping new concepts before explicit definitions come into play. More generally, in Roam, text is mixed with code (similar to Literate Programming, the paradigm from which Jupyter and other code-notebook systems have been inspired), but with a much deeper potential integration than simply interspersing text and code: each block is computable from the start. A simple example of this is the calc command, which grabs numbers from a block and makes them available for computation." ([Chan 2020:5](zotero://open-pdf/library/items/IANZKQ5M?page=5))
:PROPERTIES:
:ID:894b994c-5617-456c-9e46-46b542ad7134
:END:

#### "Formal propagation of belief values can be enabled in a lightweight way after the fact, using calc and block references. […] adding in page tags (or adding them later via unlinked references) to claim blocks can enable powerful structured aggregation of queries not just by association but involving particular kinds of relationships. Importantly, these can be added later!" ([Chan 2020:6](zotero://open-pdf/library/items/IANZKQ5M?page=6))

#### "A lot of this power is still not yet fully realized; for example, attributes still can't be used in as powerful a way as we want. But the potential is really there! I'm already experiencing the value of formally tagging some claims and stitching them together into synthesis notes via block references and filtering." ([Chan 2020:6](zotero://open-pdf/library/items/IANZKQ5M?page=6))
:PROPERTIES:
:ID:66c897d5-d173-46de-8380-34948966e400
:END:

#### "core to the magical experience of Roam: you don't have to commit to a structure in the beginning (what file/cabinet does this go into? How should I tag it?). You simply write, and then formalize/link as you go to incrementally build your knowledge graph." ([Chan 2020:7](zotero://open-pdf/library/items/IANZKQ5M?page=7))
:PROPERTIES:
:ID:ff03cb02-12b3-439b-b866-e669b3e29107
:END:

#### "Little features like the data in sliders could become part of Bayesian belief networks. We could reason over the network structure in terms of the density/distribution of links, etc. But the sky (and apparently dev time) is the limit!" ([Chan 2020:7](zotero://open-pdf/library/items/IANZKQ5M?page=7))
:PROPERTIES:
:ID:91cda7d6-52e8-4f3c-821b-dd43b1c27a80
:END:
