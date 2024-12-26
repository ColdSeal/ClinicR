# Project: Few shot chain-of-thought driven reasoning to prompt LLMs for open-ended medical question answering

This repository implements and demonstrates advanced prompting strategies and reward modeling techniques for NLP tasks, particularly using Llama2 models and LoRA finetuning.

---

## Directory Structure

### 1. `prompting_strategies/`
This directory contains the implementation of various prompting strategies and their associated resources.

- **`forward_backward/`**: Implements forward-backward reasoning techniques.
  - `forward_backward.py`: Main script for forward-backward generation.
  - `backward_generation/`: Resources for backward generation, including:
    - Scripts for backward reasoning (`backward_generation.py`).
    - Results generated using Llama2-70B-chat and other models.
    - Prompt files for Eliminative and ClinicR strategies.

- **`reasoning_verifier/`**: Contains scripts and datasets for training the reasoning verifier.
  - `reward_modeling_llama70bchat.py`: Main script for training the reward model.
  - `dataset/`: Includes training and test data generation scripts and sample data.

### 2. `Demo_notebooks/`
This folder contains Jupyter notebooks showcasing the following strategies:
- `ClinicR.ipynb`: ClinicR strategy demo.
- `Eliminative.ipynb`: Eliminative strategy demo.
- `ClinicR_MCQ-Eliminative.ipynb`: Combined ClinicR and MCQ Eliminative strategy.
- `ClinicR_Verifier.ipynb`: Demo for ClinicR with a trained verifier.

### 3. `chatbot_demo/`
A chatbot demo implemented using **Streamlit** to interactively showcase the pipeline.
- `chatbot_demo_hf.py`: Main chatbot script.
- `reward_model/`: Includes LoRA-finetuned checkpoints for reward modeling.

### 4. `data_annotator_stats/`
Includes evaluation results and annotations from human evaluators.
- `intern_responses/`: Responses and reasoning from medical experts on various datasets.

---

## Usage

### Setting Up the Environment
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_name>

2. Install dependencies:
   ```bash
   pip install -r requirements.txt

### Running Examples
1. Forward-Backward Reasoning:
   - Navigate to the prompting_strategies/forward_backward/ directory:
   ```bash
   cd prompting_strategies/forward_backward
   python forward_backward.py
2. Training Reward Models:
   - Refer to the reasoning_verifier/README.md for detailed instructions on training.
3. Chatbot Demo:
   - Navigate to chatbot_demo/ and run the Streamlit demo:
   ```bash
   streamlit run chatbot_demo_hf.py

## Highlights
- Prompting Strategies: Includes ClinicR, Eliminative, and hybrid strategies.
- Reward Modeling: LoRA-finetuned models for improved reasoning.
- Interactive Chatbot: Explore the pipeline through a Streamlit-based chatbot.
- For additional details, refer to the README files in respective subdirectories.

## Acknowledgement
- This `README.md` provides a clear overview, usage instructions, and navigation for the repository. Let us know if you'd like any additional details or modifications!
