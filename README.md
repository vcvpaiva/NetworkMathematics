(A place to collect the work happening at the Hausdorff Institute of Mathematics 
[Prospects of Formal Mathematics](https://www.mathematics.uni-bonn.de/him/programs/current-trimester-program/him-trimester-program-prospects-of-formal-mathematics)
programme.)

# NetworkMathematics

Talks given about it:
* At Topos Institute https://www.youtube.com/watch?v=DAuB6F90KtQ (Oct 2023)
* At Chapman University https://www.youtube.com/watch?v=Wiwm872T1Yk&list=PLhgq-BqyZ7i7oExXDr22w8lNdIC3tcRRW&index=1 (May 2024)
* At Women in Logic Online https://www.youtube.com/watch?v=SE5vIeBEGWI (Mar 2024)

Work on mathematical text:

1. The Parmesan prototype from the work with Jacob Collard and Eswaran Subrahmanian is at http://www.jacobcollard.com/parmesan2/
    
We have preprints:
* https://arxiv.org/abs/2406.11577 Mathematical Entities: Corpora and Benchmarks, presented at COLING2024 and Workshop

* https://arxiv.org/abs/2307.06699 Parmesan: mathematical concept extraction for education, 

* https://arxiv.org/abs/2208.13830 Extracting Mathematical Concepts from Text (Proceedings of the Eighth Workshop on Noisy User-generated Text (W-NUT 2022))

2. The MathGloss prototype with Lucy Horowitz, a glossary for undergraduate mathematics semi-automatically created, is at MathGloss https://mathgloss.github.io/MathGloss/database
   
   A newer prototype glossary dealing with Category Theory and building from Leinster, Goldblatt, and Riehl's textbooks is at https://mathgloss.github.io/CatGloss/database.
    
   The original preprint on MathGloss is https://arxiv.org/abs/2311.12649 MathGloss: Building mathematical glossaries from text.

Lucy also has some recent work with Ryan Hathaway at [Fine-Tuning BERTs for Definition Extraction from Mathematical Text](https://arxiv.org/abs/2406.13827)

3. The work with Larry Moss, Bert Gao, and Pavel Kovalev which produced the preprint [Extracting Mathematical Concepts with Large Language Models](https://arxiv.org/abs/2309.00642) has been a bit neglected recently because we're more interested in thinking about using LLMs for Natural Language Inference. But we should reconsider it in the light of the extraction of definitions using LLMS.

4. When we have the latex of a text we can be certain that what the author calls a definition, is one such. Deyan Ginev did an incredible amount of work trying to get the different kinds of latex in the arxiv into a common format ar5iv they call it. so he has a gigantic corpus of author-identified "definitions", which we can, in principle, tap for our own purposes.
Frederik Schaefer is investigating the idea and has a 1% sample.

5. Josef Urban suggests instead using LLMS to extract definitions. I pointed him to our 'informal corpora' in
   1. TAC abstracts ~3K sentences in
https://github.com/vcvpaiva/NLIMath/blob/main/3000_sentences_extracted.jsonl. 433 'clean' sentences from above
https://github.com/vcvpaiva/NLIMath/blob/main/Experiment436/Experiment2.txt
   2. nLab 2020 and 2024 (~15K, ~19K pages) in json in
https://github.com/ToposInstitute/nLab2024-corpus. nLab `clean' sentences ~50K in
https://raw.githubusercontent.com/ToposInstitute/nlab-corpus/main/nlab_examples.csv
But TAC abstracts do NOT contain definitions (I should've known) and nLab is not producing good results (don't know why). So we're now using Frederik Schaefer's data.

6. Bauer, Petkovic, and Todorovski constructed the dataset MLFMF "machine learning for mathematical formalization", using Lean's mathlib and Agda's unimath, standard, and TypeTopology libraries. We wondered if we could simply use their definitions, as they say their nodes `represent library entries (theorems, lemmas, axioms, and definitions)'.

   
# Implementing Dialectica Categories

A different project, arising from my doctoral work on an internal categorical characterization of Kurt Gödel's "Dialectica Interpretation".

1. I first to Reed Mullanix about it. Reed came up with an interesting idea https://gist.github.com/TOTBWF/e946b99a6770d7bd53fdebe5f9064657
But  we didn't have time to develop it, as it was his last week here.

2. Then I talked to Maximilian Dore about it. Maximilian likes cubical Agda very much much.
   Since Harley Eades has an old preliminary implementation of Dialectica categories in Agda (see https://github.com/heades/dialectica-spaces/tree/master) this made sense.
   But Harley did not implement the relations. Max now thinks he would prefer to work on Chu spaces.

3. I talked to Cyril Coen, who thought Rocq or Coq would make sense.
   

