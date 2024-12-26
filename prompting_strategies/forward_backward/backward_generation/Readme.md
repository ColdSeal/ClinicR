# Forward-Backward Generation Prompt

## Overview
This project aims to generate backward results using:
- **Codex Prompt** 
- **ClinicR Prompt (with options)** 
- **Llama2-7B Chat Model**

## Objectives
1. Leverage forward-backward reasoning approaches for question answering.
2. Utilize the model for:
   - **Reward Modeling**: Fine-tuning model outputs by assigning scalar rewards based on quality.
   - **Binary Classification Training**: Distinguishing between correct and incorrect responses.

## Research Goals
- **Assess Knowledge:** Determine if the model inherently possesses sufficient domain knowledge to tackle complex questions effectively.
- **Evaluate Reasoning Ability:** Test the model's reasoning and answer-generation capabilities under forward-backward setups.

## Key Features
- Backward reasoning integrates multiple output options to verify and finalize the most accurate response.
- Reward modeling is used to enhance the model's ability to prioritize better answers.