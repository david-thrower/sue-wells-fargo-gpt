
# sue-wells-fargo-gpt

This project aims to create an expert Large Language Model (LLM) trained on every federal court civil lawsuit that Wells Fargo has lost over the last 25 years. The primary goal is to provide attorneys and pro se litigants with a valuable resource to draft prevailing complaints, briefs, motions, and other legal documents against Wells Fargo Bank, NA in US District Federal Court.

The project's objective is to create a Minimum Viable Product (MVP) or proof of concept fork of Gemma 2-2B-it, or if resources permit, to use larger models like Gemma 2-9B-it or Gemma 2-27B-it, fine-tuned with DoRA PEFT. This will enable the generation of consistently winning legal documents tailored to the arguments that have previously succeeded in similar cases against Wells Fargo Bank, NA.

In the future, this project could evolve into a for-profit Software as a Service (SAAS) product for the legal community.

## Current status

- The project is still in its early stages, with considerable work to be done on creating the dataset.
- We plan to use the DoRA-fine-tuning-gemma-2-2b-it template [GitHub - david-thrower/DoRA-fine-tuning-gemma-2-2b-it](https://github.com/david-thrower/DoRA-fine-tuning-gemma-2-2b-it) to fine-tune a model from the data.

## How to contribute

- **Data extraction:** Extract data from PACER and [CourtListener](https://www.courtlistener.com) for US District and Circuit federal courts where Wells Fargo's opposing party was the prevailing party.
- **Data packaging:** Package opinions and prevailing complaints, motions, briefs, and examples of prompts that an attorney or pro se litigant may write into the JSONl format needed to train the model.
- **Legal community review:** Legal community members are encouraged to review the training data to ensure its accuracy and relevance.
- **Donations:** Donations of High-Performance Computing (HPC) resources, GPU, TPU time, or any other form of contribution are highly appreciated.
