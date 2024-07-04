# NetworkMathematics

A place to collect the work happening at the Hausdorff Institute of Mathematics 
[Prospects of Formal Mathematics](https://www.mathematics.uni-bonn.de/him/programs/current-trimester-program/him-trimester-program-prospects-of-formal-mathematics)
programme.

Talks given about it:
* At Topos Institute https://www.youtube.com/watch?v=DAuB6F90KtQ
* At Chapman University https://www.youtube.com/watch?v=Wiwm872T1Yk&list=PLhgq-BqyZ7i7oExXDr22w8lNdIC3tcRRW&index=1
* At Women in Logic Online https://www.youtube.com/watch?v=SE5vIeBEGWI

Work on mathematical text:

1. The prototype from the work with Jacob Collard and Eswaran Subrahmanian is at http://www.jacobcollard.com/parmesan2/ 
We have preprints:
https://arxiv.org/abs/2406.11577 Mathematical Entities: Corpora and Benchmarks,
https://arxiv.org/abs/2307.06699 Parmesan: mathematical concept extraction for education, 
https://arxiv.org/abs/2208.13830 Extracting Mathematical Concepts from Text

2. The prototype from the work with Lucy Horowitz on a glossary for undergraduate mathematics is at MathGloss https://mathgloss.github.io/MathGloss/database
   A newer prototype glossary dealing with Category Theory and built from textbooks from Leinster, Goldblatt and Riehl is at https://mathgloss.github.io/CatGloss/database.
    
The original preprint is https://arxiv.org/abs/2311.12649 MathGloss: Building mathematical glossaries from text.
Lucy also has some recent work with Ryan Hathaway at [Fine-Tuning BERTs for Definition Extraction from Mathematical Text](https://arxiv.org/abs/2406.13827)

3. The work with Larry Moss, Bert Gao, and Pavel Kovalev which produced the preprint [Extracting Mathematical Concepts with Large Language Models](https://arxiv.org/abs/2309.00642) has been a bit neglected recently because we're more interested in thinking about using LLMs for Natural Language Inference. But we should reconsider it in the light of the extraction of definitions using LLMS.

4. When we have the latex of a text we can be certain that what the author calls a definition, is one such. Deyan Ginev did an incredible amount of work trying to get the different kinds of latex in the arxiv into a common format ar5iv they call it. so he has a gigantic corpus of author-identified "definitions", which we can, in principle, tap for our own purposes. Frederik S is investigating the idea and has a 1% sample.

Josef Urban suggests instead using LLMS to extract definitions. I pointed him to our 'informal corpora' in 
   
# Implementing Dialectica

