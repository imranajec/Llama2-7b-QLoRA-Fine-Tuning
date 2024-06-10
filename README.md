# Llama2-7b-QLoRA-Fine-Tuning

This repository contains the code and resources for fine-tuning the Llama-2-7b-chat-hf model using QLoRA (Quantized Low-Rank Adaptation). The project demonstrates how to fine-tune the model on a dataset and generate text based on the fine-tuned model.

## Description

Fine-tuning Llama-2-7b-chat-hf using QLoRA for efficient text generation.

## Original Llama-2 Model Parameters

- **Model Name**: NousResearch/Llama-2-7b-chat-hf
- **Parameters**: 7 billion
- **Architecture**: Transformer-based language model
- **Layers**: 32
- **Hidden Size**: 4096
- **Attention Heads**: 32
- **Vocabulary Size**: 50,257
- **Context Size**: 2048 tokens

## QLoRA Fine-Tuning Parameters

- **LoRA Rank (r)**: 64
- **LoRA Alpha**: 16
- **LoRA Dropout**: 0.1
- **4-bit Quantization**: True (nf4)
- **Training Batch Size**: 4
- **Number of Epochs**: 1
- **Learning Rate**: 2e-4

## Setup and Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/imranajec/Llama2-7b-QLoRA-Fine-Tuning.git
    cd Llama2-7b-QLoRA-Fine-Tuning
    ```

2. **Install the required packages**:
    ```bash
    pip install -q accelerate==0.21.0 peft==0.4.0 bitsandbytes==0.40.2 transformers==4.31.0 trl==0.4.7
    ```

3. **Run the Jupyter notebook to fine-tune the model and generate text**:
    ```bash
    jupyter notebook Fine-Tuning_Llama-2_with_QLoRA.ipynb
    ```

## Results

The fine-tuned model can be used to generate text based on given prompts. Here is an example of text generation:

**Prompt**: How do I install Firefox and set it as default on Windows 10?
**Generated Text**: ...

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

Special thanks to the Hugging Face community and the developers of the transformers and bitsandbytes libraries for their invaluable tools and resources.

---

Feel free to reach out if you have any questions or suggestions!
