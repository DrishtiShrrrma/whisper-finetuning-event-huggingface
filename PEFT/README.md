## PEFT (Parameter Efficient Fine Tuning)

- PEFT employs various techniques, including LoRa, to efficiently fine-tune large language models.
- PEFT only fine-tunes a small number of (extra) model parameters while freezing most parameters of the pretrained model, thereby greatly decreasing the computational and storage costs.


## LoRA (Low Rank Adaptation)
- A type of PEFT
- LoRA freezes the pre-trained model weights and injects trainable rank decomposition matrices into each layer of the Transformer architecture. This greatly reduces the number of trainable parameters for downstream tasks.
