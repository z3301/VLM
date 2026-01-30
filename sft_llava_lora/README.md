---
library_name: peft
license: llama2
base_model: llava-hf/llava-1.5-7b-hf
tags:
- base_model:adapter:llava-hf/llava-1.5-7b-hf
- lora
- transformers
pipeline_tag: text-generation
model-index:
- name: sft_llava_lora
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft_llava_lora

This model is a fine-tuned version of [llava-hf/llava-1.5-7b-hf](https://huggingface.co/llava-hf/llava-1.5-7b-hf) on an unknown dataset.

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 2
- eval_batch_size: 8
- seed: 42
- distributed_type: multi-GPU
- gradient_accumulation_steps: 8
- total_train_batch_size: 16
- optimizer: Use OptimizerNames.ADAMW_TORCH_FUSED with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: cosine
- lr_scheduler_warmup_steps: 100
- num_epochs: 1

### Training results



### Framework versions

- PEFT 0.18.1
- Transformers 5.0.0
- Pytorch 2.9.1
- Datasets 4.5.0
- Tokenizers 0.22.2