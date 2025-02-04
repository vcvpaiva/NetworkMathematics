(A place to collect the work happening at the Hausdorff Institute of Mathematics (HIM)
[Prospects of Formal Mathematics](https://www.mathematics.uni-bonn.de/him/programs/current-trimester-program/him-trimester-program-prospects-of-formal-mathematics)
programme.)

# NetworkMathematics

Talks given about the project:
* At HIM (June 2024) [AI Tools for Better Math](https://www.youtube.com/watch?v=C7NBGlJb2DQ&list=PLul8LCT3AJqQgcJYiC0CycjFLcrhM2fRg&index=4)
* At Topos Institute (Oct 2023) [Network Mathematics for Beginners](https://www.youtube.com/watch?v=DAuB6F90KtQ) thanks Dana for the support!
* At Chapman University (May 2024) [Network Mathematics for all](https://www.youtube.com/watch?v=Wiwm872T1Yk&list=PLhgq-BqyZ7i7oExXDr22w8lNdIC3tcRRW&index=1) 
* At Women in Logic Online (Mar 2024) [Network Mathematics](https://www.youtube.com/watch?v=SE5vIeBEGWI)

Work on mathematical text:

1. The [Parmesan prototype](http://www.jacobcollard.com/parmesan2/) a math learning assistant, work with Jacob Collard and Eswaran Subrahmanian
    
We have preprints:
*  [Mathematical Entities: Corpora and Benchmarks](https://arxiv.org/abs/2406.11577), presented at COLING2024 and [Workshop MathNLP](https://sites.google.com/view/2nd-mathnlp)

*  [Parmesan: mathematical concept extraction for education](https://arxiv.org/abs/2307.06699) 

*  [Extracting Mathematical Concepts from Text](https://arxiv.org/abs/2208.13830), Proceedings of the Eighth Workshop on Noisy User-generated Text (W-NUT 2022)

2. The [MathGloss prototype](https://mathgloss.github.io/MathGloss/database) with Lucy Horowitz, a glossary for undergraduate mathematics semi-automatically created from open source freely available resources.
   
   A newer prototype glossary dealing with Category Theory [CatGloss](https://mathgloss.github.io/CatGloss/database) and building from Leinster, Goldblatt, and Riehl's textbooks.
    
   The original preprint on MathGloss is [Building mathematical glossaries from text](https://arxiv.org/abs/2311.12649).

Lucy also has some recent work with Ryan Hathaway [Fine-Tuning BERTs for Definition Extraction from Mathematical Text](https://arxiv.org/abs/2406.13827)

Given the big push for Lean formalization going on, we would like to extend our Lean mappings. How should we go about it? Discussed with Mario how to tap the expertise of Lean developers for that. They have a mental map of which concepts are where in the library. We want that mental map written down.
    
    We are also thinking which other datasets would be useful to connect. LFMDB? Isabelle math? 
    
3. The [work with Larry Moss, Bert Gao, and Pavel Kovalev produced the preprint [Extracting Mathematical Concepts with Large Language Models](https://arxiv.org/abs/2309.00642) has been a bit neglected recently. For this we repurposed a text annotator [MathAnnotator](https://gaoq111.github.io/math_concept_annotation/). Now we're more interested in thinking about using LLMs for Natural Language Inference.

4. I'm applying the work of Katerina Kalouli on [Hy-NLI: a Hybrid System for Natural Language Inference](http://hynli.nlitoolkit.de/), GKR and [XplaiNLI: eXplainable Natural Language Inference](http://xplainli.nlitoolkit.de/) to informal mathematics. This comes with several challenges, including the need for definitions and dealing with formulas.

5. A preliminary laundry list of tasks is available  [Network Mathematics: Projects and Problems](https://docs.google.com/document/d/1XihAI2fhHvE9Gg-CemXo7rK9Q3jRVwS3A4L2xpqozos/edit#heading=h.dkqktuuv2bds)
 


   # Work at Hausdorff

1. When we have the latex of a text we can be certain that what the author calls a definition, is one such. Deyan Ginev did an incredible amount of work trying to get the different kinds of latex in the arxiv into a common format ar5iv as he calls it. He has a gigantic corpus of author-identified "definitions", which we can, in principle, tap for our own purposes.
Frederik Schaefer is investigating the idea and has a 1% sample. (more below)

 Josef Urban suggested  using LLMS to extract definitions. I pointed him to our 'informal corpora' in
* [TAC abstracts](https://github.com/vcvpaiva/NLIMath/blob/main/3000_sentences_extracted.jsonl) ~3K sentences in. [433 'clean' sentences](https://github.com/vcvpaiva/NLIMath/blob/main/Experiment436/Experiment2.txt) from above.

* [nLab 2020](https://github.com/ToposInstitute/nLab2024-corpus) and 2024 (~15K, ~19K pages) in json format. [nLab `clean' sentences](https://raw.githubusercontent.com/ToposInstitute/nlab-corpus/main/nlab_examples.csv) ~50K 

But TAC abstracts do NOT contain many definitions (I should've known, given Lucy and Ryan's work) and nLab is not producing good results (don't know why). 
So we're now using Deyan Ginev's data modified by Frederik Schaefer,  consisting of arxiv math.CT papers. https://github.com/JUrban/extract-defs
Have 3377 math.CT papers in Deyan's 2020 dataset, this gives us 16K 'definitions', considered as such by the authors in the arxiv latex files.

5. Together with Stefania Dumbrova and Lucy Horowitz we're considering alignments between definitions in provers Lean, Mizar, Agda, etc. Bauer, Petkovic, and Todorovski constructed the dataset MLFMF "machine learning for mathematical formalization" (https://arxiv.org/pdf/2310.16005), using Lean's mathlib and Agda's libraries unimath, standard, and TypeTopology. We wondered if we could simply use their definitions, as they say their nodes `represent library entries (theorems, lemmas, axioms, and definitions)'. Stefania is leading the effort to build a knowledge graph of freely available mathematical concepts.

   Questions/examples of what we wanted to use a knowledge graph for https://docs.google.com/document/d/1bg5ISacYtHqvqmw6uNr4d59s1LjtO6zItNK2SL8nkp8/edit

7. Some notes on this effort,  started in Dagstuhl 1-6 October 2023.

  
   
# Formalizing Dialectica Categories

A different project, arising from my doctoral work on an internal categorical characterization of Kurt Gödel's "Dialectica Interpretation". 
I want to formalize Dialectica categories, because there are several instances of the construction and it would be good to do them once and for all.
Also several applications of these ideas have been uncovered over the years and it would be nice to know how the different instances relate to each other.
Some non-formalized discussions can be found at https://github.com/vcvpaiva/DialecticaCategories/blob/master/README.md.

1. I first talked  to Reed Mullanix about it. Reed came up with an [interesting idea](https://gist.github.com/TOTBWF/e946b99a6770d7bd53fdebe5f9064657)
   But  we didn't have time to develop it, as it was his last week here and he was more interested in formalizing the tripos-to-toposes construction.

2. Then I talked to Maximilian Dore about it. Maximilian likes cubical Agda very much.
   Since Harley Eades has an old preliminary implementation of Dialectica categories in Agda (see https://github.com/heades/dialectica-spaces/tree/master) trying to use Agda made sense.
   But Harley did not implement the relations, an essential component. Max now thinks he would prefer to work on Chu spaces.

3. I talked to Cyril Cohen, who thought Rocq  would make sense.

4. Then I talked to Mario Carneiro and the [Dialectica category construction is now in Lean](https://github.com/leanprover-community/mathlib4/pull/14274/files), already proven symmetric monoidal closed. Still need to get the bang operator and products and coproducts though, which I thought would be easier. Then we can generalize to polynomials and more.
  
5. Mario Carneiro formalization of the original Dialectica construction in Lean  completes a kind of third 'deliverable' from the [MRC on Applied Category Theory](https://www.ams.org/programs/research-communities/2022MRC-Categories) in 2022.

The first deliverable was  on the relationship between Dialectica and polynomials and at least the arxiv preprint  [Monoidal structures on generalized polynomial categories](https://arxiv.org/abs/2305.05655), Joseph Dorta, Samantha Jarvis, and Nelson Niu. May 2023. Presented at ACT 2023 and JMM 2023.

The second deliverable was [On a fibrational construction for optics, lenses, and Dialectica categories](https://arxiv.org/abs/2403.16388)
Matteo Capucci, Bruno Gavranović, Abdullah Malik, Francisco Rios, Jonathan Weinberger. Presented at MFPS 2024, Oxford.

Another deliverable would be the connection to games pursued by Jeremie, Colin and Jan.

   

