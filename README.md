# Attribute value extraction with OpenAI GPT-3

## Overview

The repository contains accompanying code for the Weights & Biases
report : [Attribute-Value Extraction with GPT-3 and Weight & Biases](https://wandb.ai/parambharat/mave/reports/Attribute-Value-Extraction-with-GPT-3-and-Weight-Biases--VmlldzoyNzg1Njg0)

The notebook contains code to prepare the dataset and finetune OpenAI GPT-3 on
the [mave dataset](https://github.com/google-research-datasets/MAVE) and run evaluations.
The sweeps.py file contains code to run hyperparameter sweeps to the finetuned model.
The sweeps.yaml file contains the hyperparameter sweep configuration.

to run the sweeps, run the following command:

```bash
wandb sweep -p "<YOUR_PROJECT_NAME>" -e "<YOUR_WANDB_ENTITY>" --name "<NAME_OF_THE_SWEEP>" sweeps.yaml
```

## Setup

You will need an OPENAI_API_KEY to run the notebook. You can get one from [here](https://openai.com/api/)
You will also need to install the wandb and openai libraries. You can install it using pip:

```bash
pip install openai wandb
```

Other libraries used in sweeps.py can be installed with the following command:

```bash
pip install pandas scikit-learn numpy dotenv
```

To run the notebook you will also need jupyter. To install run:

```bash
pip install jupyter
```



