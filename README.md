

# Project Title: Innovative Multi-Modal Image Generation and Captioning with Advanced Vision Models 

### Image-to-prompt

## Description:
Welcome to this exceptional repository showcasing a remarkable solution for the Kaggle competition centered around Multi-Modal Image Generation and Captioning. We are proud to present an ingenious approach that blends advanced vision models, data curation strategies, and optimization techniques for efficient image generation. While another talented individual crafted the solution, we are thrilled to provide an overview of their exceptional work.

## Solution Highlights:
This solution commenced with an impressive feat – generating approximately 10.6 million images from around 8.6 million prompts. To expedite this process, a suite of innovative strategies was employed, ranging from transformer-based techniques and mixed-precision training to optimizing image size and generation steps.

The crux of this solution lies in three key vision models: ViT-Large, ConvNeXt-XXLarge, and BLIP-2. These models were meticulously trained and fine-tuned in two stages. The first phase involved pretraining on the curated "PROMPTS_LQ" dataset, while the second phase focused on finetuning using the refined "PROMPTS_HQ" dataset. The result was a potent ensemble of these models, synergistically combining their predictive power.

## Datasets and Data Curation:
Central to this solution's success was the emphasis on diverse and high-quality data. A meticulous curation process led to the creation of a dataset comprising approximately 2 million high-quality prompts, referred to as "PROMPTS_HQ." Multiple datasets were strategically utilized, including DiffusionDB_2M, COCO Captions, VizWiz, Open Image, ADE20K, Flickr30K, and TextCaps. Through the application of stringent rules and the removal of duplicates, the integrity of the dataset was upheld. Additionally, two images were generated per prompt using distinct random seeds, further enriching the dataset.

The expansive COYO-700M dataset played a role in pretraining, even though it did not directly enhance the final performance. Its utilization showcased resourcefulness and a keen understanding of dataset dynamics.

## Model Selection and Modifications:
The solution's architect underwent an exhaustive model selection process, experimenting with various options such as SWIN and DinoV2. Ultimately, ViT-Large, ConvNeXt-XXLarge, and BLIP-2 emerged as the models of choice due to their demonstrated effectiveness and alignment with the competition's objectives.

A noteworthy innovation was the removal of the Large Language Model (LLM) component from the BLIP-2 model. This strategic modification was driven by the unique nature of the task, where grammar and prompt sequence had limited relevance. Additionally, the incorporation of LORA (Layer-wise Relevance Adaptive Fine-Tuning) for model refinement showcased a sophisticated approach.

## Notable Achievements:
An unexpected breakthrough was achieved by introducing an additional large fully connected layer before the output layer in the CLIP model. This seemingly minor tweak yielded substantial score improvements, underscoring the power of iterative refinement.

The solution revealed a correlation between larger image sizes and higher scores, prompting strategic decisions about resource allocation.

## Acknowledgments:
I extend gratitude to the original solution creator and Kaggle for hosting this enriching competition. The Kaggle community's vibrant exchange of ideas and code-sharing played a pivotal role in shaping this solution.

In conclusion, this repository stands as a testament to the fusion of advanced vision models, meticulous data curation, and creative adaptations in the realm of multi-modal image generation and captioning. We invite you to explore the original solution, dive into the code, and celebrate the innovation that led to success in the Kaggle competition.
