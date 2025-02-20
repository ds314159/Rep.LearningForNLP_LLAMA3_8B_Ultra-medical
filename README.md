# Medical Article Summarization: Comparative Analysis of LLM Approaches

## Overview
This research evaluates methodologies for automated medical abstract generation using Large Language Models, comparing various summarization techniques across both observational studies and randomized controlled trials. The study utilizes LLaMA-3-8B-UltraMedical as the foundation model and implements multiple summarization strategies.

## Methodology
The research examines five distinct approaches: naive prompting, specialized medical prompting, LoRA fine-tuning, pure extractive summarization via embedding similarity, and hybrid extractive-abstractive methods. The evaluation framework employs ROUGE-2 scores as the primary metric for performance assessment.

## Results
Extractive summarization demonstrated superior performance with a ROUGE-2 score of 22.9%, significantly outperforming other methods. Naive prompting achieved 4-5%, while specialized prompting and LoRA fine-tuning reached 6-7%. The hybrid approach showed no significant improvement over basic abstractive methods.

## Implementation
Core dependencies:
```python
pip install rouge-score accelerate sentencepiece transformers
pip install bitsandbytes==0.43.1 vllm nltk spacy
pip install sacrebleu pycocoevalcap
```



## Future Research Directions
Future work should focus on refining similarity criteria, implementing multi-scale semantic analysis, and developing sophisticated importance classifiers. Integration of hybrid approaches leveraging both extractive and abstractive strengths warrants further investigation.



This project is licensed under the MIT License.
