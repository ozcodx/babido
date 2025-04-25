# The Babel Library: Ido Section Generator

A collaborative linguistic-literary project by **Oscar Bernal** (Systems Engineering graduate, Universidad Tecnológica de Pereira) and **Luis David Cardona** (aspiring graduate in Linguistics, Universidad Tecnológica de Pereira).

---

## 📚 Introduction

This project is inspired by the short story *La Biblioteca de Babel* (The Library of Babel) by **Jorge Luis Borges**, originally published in 1941. In Borges' story, an infinite library contains every possible combination of characters in every possible book, rendering most of them nonsensical. Yet, hidden among them, lie books of unimaginable clarity, wisdom, and coherence.

Our goal is to imagine a *structured section* of that mythical library—a wing in which the texts are **not entirely random**, but bound by the constraints of a **constructed language** (specifically, *Ido*—a derivative of Esperanto), **grammatical rules**, and eventually, **semantic meaning**.

> "The universe (which others call the Library) is composed of an indefinite and perhaps infinite number of hexagonal galleries…" — *Jorge Luis Borges*

---

## 🎯 Project Goals

- **Linguistic Generation**: Generate grammatically correct and human-readable sentences in Ido using predefined grammatical structures and categorized vocabulary.
- **Procedural Text Construction**: Use pseudo-random algorithms to create deterministic and reproducible "books" or "hexes" without the need to store them physically.
- **Structural Classification**: Allow classification and referencing of generated structures using hashes or identifiers for modular combination and reuse.
- **Scalability**: Design a system that can grow naturally as the dictionaries and rules evolve through linguistic study and research.
- **Semantic Expansion** *(future phase)*: Explore Natural Language Processing (NLP) and Artificial Intelligence techniques to:
  - Evaluate **semantic coherence** between sentences.
  - Generate longer texts with **contextual consistency**.
  - Simulate **cohesive books** with themes, characters, or logical progression.

---

## 🧠 Why Ido?

Ido is a constructed international auxiliary language derived from Esperanto. Its regular grammar and small but expressive vocabulary make it a perfect candidate for computational linguistic projects and experimental generation. Its simplicity allows:

- Fast prototyping of grammatical rules.
- Easier syntax-parsing logic.
- Broad linguistic accessibility, independent of natural language biases.

Unlike Esperanto, Ido lacks special characters such as circumflexes (ĉ, ĝ, ĥ, ĵ, ŝ) and other diacritics, using only standard ASCII characters. This characteristic:
- Eliminates the need for unicode handling and normalization in computational implementations
- Simplifies character encoding and processing
- Ensures compatibility across all computing environments and platforms
- Reduces complexity in pattern matching and text manipulation algorithms

Additionally, Ido's grammar follows strict, fixed rules with virtually no exceptions:
- All verbs conjugate following the same pattern, without irregular forms
- Noun pluralization follows a single consistent rule
- Adjective agreement has clear, unambiguous patterns
- Word formation through affixes follows predictable rules

These characteristics make Ido an ideal testbed for linguistic experimentation, as its deterministic nature allows for perfect reproducibility and systematic exploration of language structure without the noise of irregularities found in natural languages or even other constructed languages.

---

## ⚙️ How It Works

1. **Word Categories (`words.yaml`)**  
   Words are organized by grammatical function: nouns, verbs, adverbs, etc.

2. **Phrase Structures (`structures.yaml`)**  
   Each phrase structure defines a generative *template* such as:  
   `{artikoloj?} {adjetivos?} {sustantivos} {verbos} {adverbios?}`  
   Optional elements are marked using a custom mini-regex syntax.

3. **Grammar Rules (`grammar.yaml` or Python module)**  
   This module defines rules for pluralization, verb conjugation, adjective agreement, etc.

4. **Sentence Generator (`sengen.py`)**  
   A deterministic generator that uses a seed (like a hash or book address) to generate reproducible sentences based on the rules and structures provided.

---

## 🧪 Future Directions

We envision integrating NLP models and semantic parsers to:
- **Evaluate generated text** for syntactic and semantic cohesion.
- **Construct entire procedurally generated books** with thematic unity.
- Use **machine learning classifiers** to tag sentences by tone, genre, or emotion.

Additionally, future phases may include:
- A full **graph of interconnected phrases** and topics.
- Tools for **interactive exploration** of "hexes" within this structured section of Babel.
- Export formats like PDF or EPUB for generated texts.

---

## 📍 Academic Context

This project is developed within the context of interdisciplinary research at the **Universidad Tecnológica de Pereira (UTP)** in Colombia, bringing together expertise from the fields of **Systems Engineering** and **Linguistics**. It reflects a shared passion for language, literature, artificial intelligence, and experimental computation.

---

## 🔬 Research Justification

This project serves as a foundational experiment in procedural linguistics and computational creativity, merging constructed language theory, linguistic formalism, and systems engineering. By choosing Ido as the base language, we leverage a simplified, regular, and fully ASCII-compatible syntax, making it highly suitable for:

- Computational processing, parsing, and phrase construction.
- Rule-based natural language generation (NLG).
- Cross-linguistic structural modeling.

Unlike Esperanto, which includes accented characters and some irregularities, Ido's consistent morphology and lack of special characters allows deterministic tokenization and grammar rule enforcement, without pre-processing steps or unicode normalization—ideal for algorithmic manipulation and large-scale sentence generation.

### Broader Academic Vision

The long-term goal of this work is to establish a scalable methodology for:

- Designing linguistically valid sections of the Library of Babel.
- Generating semantic, grammatical and contextually coherent texts using algorithmic rules.
- Exploring the limits of meaning within constrained symbol spaces (e.g., Ido, Esperanto, Toki Pona, Lojban, or natural languages).

This opens the door to a diverse range of linguistic and computational research topics, such as:

- Formal complexity analysis of sentence structures across languages.
- Studying combinatorial language saturation: how many meaningful sentences can be generated under specific rules.
- Development of semantic validation models using AI or symbolic logic.
- Training AI agents in constructed languages as low-noise environments for testing generalization.
- Modeling emergent discourse from generative language systems.
- Building tools to explore or visualize linguistic phase space—all grammatically possible outputs under given constraints.

Ultimately, this is a platform for linguistic experimentation that blends human creativity, literary imagination, and machine logic.

---

## 🧾 References

- Borges, Jorge Luis. *Ficciones*. Buenos Aires: Editorial Sur, 1944.
- [La Biblioteca de Babel — Full Text (English)](https://libraryofbabel.info/Borges.html)
- UTP Official Website: [https://utp.edu.co](https://utp.edu.co)
- Ido Language Resources: [https://en.wikipedia.org/wiki/Ido_language](https://en.wikipedia.org/wiki/Ido_language)

--- 