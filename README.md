---
library_name: transformers
language:
- en
pipeline_tag: image-feature-extraction
license: cc-by-nc-4.0
inference: false
---

# nomic-embed-vision-v1.5: Expanding the Latent Space

`nomic-embed-vision-v1.5` is a high performing vision embedding model that shares the same embedding space as [nomic-embed-text-v1.5](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5).

All Nomic Embed Text models are now **multimodal**!

| Name                             | Imagenet 0-shot | Datacomp (Avg. 38) | MTEB      |
| :-------------------------------:| :-------------- | :----------------- | :------:  | 
| `nomic-embed-vision-v1.5`        | 71.0            | 56.8               | 62.28     | 
| `nomic-embed-vision-v1`          | 70.7            | 56.7               | 62.39     |
| OpenAI CLIP ViT B/16             | 68.3            | 56.3               | 43.82     |
| Jina CLIP v1                     | 59.1            | 52.2               | 60.1      |

