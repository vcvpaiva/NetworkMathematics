# Network Mathematics: AI Tools for Better Math

**Valeria de Paiva**  
Topos Institute  
*Date: [April 2025]*

## Abstract
Network Mathematics is an ambitious effort to use modern AI tools to uncover, structure, and represent the latent knowledge in mathematics. By building knowledge graphs and leveraging AI-powered tools for question-answering, argument mapping, and summarization, this work aims to enhance mathematical discovery, education, and research.

## 1. Introduction
Mathematics, as a highly formalized and abstract discipline, has a deep underlying structure that is not always easily accessible to modern computational tools. In recent years, natural language processing (NLP) and machine learning (ML) have shown promise in helping bridge this gap. Network Mathematics seeks to leverage these tools to not only extract mathematical knowledge from existing literature but to also make this knowledge more accessible and usable.

## 2. Extracting the Structure of Mathematical Knowledge
Mathematics is built on precise definitions and intricate relationships between concepts. In order to uncover these relationships, we must first extract mathematical concepts from existing literature and identify the relationships between them.

### MathGloss as a Foundational Layer
MathGloss is an ongoing project that focuses on building a comprehensive glossary of fundamental mathematical concepts. These concepts will be extracted from textbooks, research papers, and other open-access sources. MathGloss aims to connect definitions, contexts, and relationships, providing a foundational layer for more advanced mathematical exploration.

### Challenges and Limitations in Concept Extraction
Despite recent advances in large language models (LLMs) such as ChatGPT and GPT-4, extracting mathematical concepts with sufficient quality remains a challenge. In particular, the absence of gold-standard datasets means that LLM-based extraction is prone to errors, such as generating non-sensical entities. This is a key challenge in automating mathematical research.

## 3. Building and Using Mathematical Knowledge Graphs
Mathematical knowledge graphs (KGs) represent structured connections between mathematical entities, such as definitions, theorems, and objects. These graphs enable both human and machine navigation of mathematical concepts.

### Interoperability with Existing Mathematical Repositories
MathGloss and other knowledge graphs can be linked to external resources such as Wikidata, OEIS, and the Stacks Project. This creates a more unified network of mathematical knowledge that can be accessed and explored through semantic interfaces.

### Applications of Knowledge Graphs
The potential applications of mathematical knowledge graphs are vast, including:
- Educational tools that adapt to a learner's progress
- Semantic search engines for mathematics
- AI-assisted proof generation and reasoning
- Collaborative platforms for sharing mathematical knowledge

## 4. AI-Augmented Mathematical Research
AI tools are poised to transform mathematical research by augmenting human expertise. In particular, we propose the creation of specialized question-answering datasets and the use of argument mapping tools for uncovering the structure of mathematical reasoning.

### Mathematical Question-Answering Datasets
There is a need for datasets focused specifically on mathematical question-answering (QA), akin to the SQuAD dataset used in natural language research. These datasets will be vital for training AI systems capable of answering complex mathematical questions.

### Argument Mapping and Reasoning Tools
Mathematical reasoning often involves intricate dependencies and logical chains. AI tools designed for argument mapping will help make these relationships explicit, enabling more advanced reasoning and exploration.

### Classification of mathematical statements
The mathematical literature can be classified into different types of statements: definitions, results (lemmas, theorems, corollaries, facts, remarks), examples, and narration, for example. To do this classification automatically, we need a gold dataset.

### Identifying logical dependencies
Apart from syntactic dependency (a theorem mentions definitions that it depends on) there is logical dependencies between propositions that we also need to detect.

### Summarization of Mathematical Content
With the increasing volume of mathematical literature, summarization tools will allow researchers to quickly understand and engage with new papers. We propose creating an infrastructure for summarizing open-access mathematical texts and linking these summaries to structured knowledge graphs.

## 5. Vision and Roadmap
The vision for Network Mathematics is to build a robust, machine-readable network of mathematical knowledge, supported by AI tools for discovery and reasoning. The roadmap for achieving this includes the following phases:

### Short-Term Goals (1–2 years)
- Expand MathGloss and integrate with external repositories
- Build the Mathoscope knowledge graph for Category Theory
- Develop and benchmark concept extraction pipelines
- Begin the creation of QA datasets for mathematics
  

### Mid-Term Goals (3–5 years)
- Launch a pilot summarization tool for math texts
- Develop semantic tools for navigating and querying mathematical graphs
- Collaborate with publishers to expand math-related corpora

### Long-Term Vision (5–10 years)
- A fully interoperable network of mathematical knowledge graphs
- AI systems that propose new research directions and assist in theorem proving
- A semantic index of all open-access mathematics
- Revolutionizing math education through interactive AI-assisted exploration

## 6. Call to Action
Mathematics is the foundation of scientific progress, yet its complex, interconnected nature is still difficult to navigate. By supporting Network Mathematics, you are contributing to the next stage of mathematical research and education—one where AI tools amplify human reasoning and enable faster, deeper insights into the structure of mathematics itself.

## 7. Acknowledgments
This project is supported by the collaboration of many researchers and institutions across mathematics, AI, and linguistics. Special thanks to the close collaborators in chronological order: Brendan Fong, Jacob Collard, Eswaran Subrahmanian, Lucy Horowitz, Larry Moss, Qiyue Gao, Pavel Kovalev,  Hai Hu, Yikang Liu, Zhiheng. Thanks to  the open-access community, including platforms like Wikipedia, Wikidata, nLab, and OEIS, for providing the foundational data. We also thank early contributors to MathGloss and Mathoscope for their feedback and annotations.

## 8. References
1. "MathGloss: Building Mathematical Glossaries from Text." Lucy Horowitz, Valeria de Paiva [arXiv:2311.12649](https://arxiv.org/abs/2311.12649)
2. "Extracting Mathematical Concepts with Large Language Models." Valeria de Paiva, Qiyue Gao, Pavel Kovalev, Lawrence Moss [arXiv:2309.00642](https://arxiv.org/abs/2309.00642)
3. "Mathematical Entities: Corpora and Benchmarks." [ACL Anthology (LREC 2024)](https://aclanthology.org/2024.lrec-main.966/)
4. "Parmesan: A Prototype for Category-Theoretic NLP." [arXiv:2208.13830](https://arxiv.org/abs/2208.13830)
5. "From Parmesan to Mathoscope: Extracting Structure in Mathematical Text." [arXiv:2307.06699](https://arxiv.org/abs/2307.06699)
6. Rajpurkar et al., "SQuAD: 100,000+ Questions for Machine Comprehension of Text." [arXiv:1606.05250](https://arxiv.org/abs/1606.05250)
7. Lo et al., "TLDR: Extreme Summarization of Scientific Documents." [arXiv:2004.15011](https://arxiv.org/abs/2004.15011)

