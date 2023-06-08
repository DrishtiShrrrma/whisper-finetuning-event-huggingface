## PEFT (Parameter Efficient Fine Tuning)

- PEFT employs various techniques, including LoRa, to efficiently fine-tune large language models.
- PEFT only fine-tunes a small number of (extra) model parameters while freezing most parameters of the pretrained model, thereby greatly decreasing the computational and storage costs.
- Need : As model sizes continue to increase, fine-tuning a model is computationally expensive and storage heavy. For example, a Whisper-large-v2 model requires ~24GB of GPU VRAM for full fine-tuning and requires ~7 GB of storage for each fine-tuned checkpoint. For low-resource environments --> a bottleneck and often near impossible to get meaningful results.


## LoRA (Low Rank Adaptation)
- A type of PEFT method
- LoRA freezes the pre-trained model weights and injects trainable rank decomposition matrices into each layer of the Transformer architecture. This greatly reduces the number of trainable parameters for downstream tasks.
- LoRA performs on-par or better than fine-tuning in model quality despite having fewer trainable parameters, a higher training throughput, and, unlike adapters, no additional inference latency.


## Vaibhav's Findings     (To be tested)

![image](https://github.com/DrishtiShrrrma/whisper-finetuning-event-huggingface/assets/129742046/27b49427-f9be-41a5-b4f4-77d895a81dc0)
