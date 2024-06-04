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


## Hosted Inference API

The easiest way to get started with Nomic Embed is through the Nomic Embedding API.

Generating embeddings with the `nomic` Python client is as easy as 
```python
from nomic import embed
import numpy as np

output = embed.image(
    images=[
        "image_path_1.jpeg",
        "image_path_2.png",
    ],
    model='nomic-embed-vision-v1.5',
)

print(output['usage'])
embeddings = np.array(output['embeddings'])
print(embeddings.shape)
```
For more information, see the [API reference](https://docs.nomic.ai/reference/endpoints/nomic-embed-vision)

## Data Visualization
Click the Nomic Atlas map below to visualize a 100,000 sample CC3M comparing the Vision and Text Embedding Space!


[![image/webp](https://cdn-uploads.huggingface.co/production/uploads/607997c83a565c15675055b3/pjhJhuNyRfPagRd_c_iUz.webp)](https://atlas.nomic.ai/data/nomic-multimodal-series/cc3m-100k-image-bytes-v15/map)