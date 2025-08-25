---
# Introduction
• This project implements scalable Ray-based enrichment of datasets with CLIP embeddings to enable retrieval with image and text queries, cluster analysis,and deduplication.

• The notebook provides code to read in images, generate embeddings, and publish the dataset via Hugging Face.

---
# Sample search results

<img width="1171" height="890" alt="sample_!" src="https://github.com/user-attachments/assets/4ecbef4f-b83c-4a50-9e68-1fcac5a8732d" />

<img width="1171" height="890" alt="sample_2" src="https://github.com/user-attachments/assets/0525e998-7d09-400e-b2b0-71382fb835eb" />

<img width="1171" height="890" alt="sample_3" src="https://github.com/user-attachments/assets/f54fb85f-1a26-40d4-80e0-9a876e4e637c" />


---
# Dataset

## Source

All images were sourced from [Francesco/insects-mytwu](https://huggingface.co/datasets/Francesco/insects-mytwu).

## Link

https://huggingface.co/datasets/hkanade/insect_image_retrieval/

## Sample usage

```python
from datasets import load_dataset

ds_new = load_dataset("hkanade/insect_image_retrieval")
ds_new["train"][0]["image"]
```
