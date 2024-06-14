---
language:
- en
license: apache-2.0
size_categories:
- 10K<n<100K
pretty_name: CharacterCodex
dataset_info:
  features:
  - name: media_type
    dtype: string
  - name: genre
    dtype: string
  - name: character_name
    dtype: string
  - name: media_source
    dtype: string
  - name: description
    dtype: string
  - name: scenario
    dtype: string
tags:
- language model
---

# Dataset Card for Character Codex

![image/png](https://cdn-uploads.huggingface.co/production/uploads/6317aade83d8d2fd903192d9/2qPIzxcnzXrEg66VZDjnv.png)

## Dataset Summary

The Character Codex is a comprehensive dataset featuring popular characters from a wide array of media types and genres. Each entry includes detailed information about the character, the media source, and a unique scenario involving the character. This dataset is valuable for synthetic data, RAG for generative AI, writers, game developers, and fans who want to explore and utilize rich character descriptions for various creative projects.

## Dataset Structure

### Data Fields

- **media_type**: The type of media the character originates from (e.g., Webcomics, Novels, Movies, TV Shows).
- **genre**: The specific genre of the media type (e.g., Fantasy Webcomics, Martial Arts Fiction).
- **character_name**: The name of the character.
- **media_source**: The title of the media source where the character is from.
- **description**: A detailed description of the character, including their role and significance in the story.
- **scenario**: A creative scenario involving the character that can be used for interactive storytelling or role-playing purposes.

### Example Data

```json
[
    {
        "media_type": "Webcomics",
        "genre": "Fantasy Webcomics",
        "character_name": "Alana",
        "media_source": "Saga",
        "description": "Alana is one of the main characters from the webcomic \"Saga.\" She is a strong-willed and fiercely protective mother who is on the run with her family in a war-torn galaxy. The story blends elements of fantasy and science fiction, creating a rich and complex narrative.",
        "scenario": "You are a fellow traveler in the galaxy needing help, and Alana offers her assistance while sharing stories of her family's struggles and triumphs."
    },
    {
        "media_type": "Novels",
        "genre": "Martial Arts Fiction",
        "character_name": "Yilin",
        "media_source": "The Smiling, Proud Wanderer",
        "description": "Yilin is a young nun from the Hengshan Sect in Jin Yong's novel \"The Smiling, Proud Wanderer.\" Known for her innocence and kindness, she becomes friends with the protagonist Linghu Chong. Her gentle nature often puts her at odds with the violent world of martial arts.",
        "scenario": "You are a fellow disciple of the Hengshan Sect seeking Yilin's comfort and advice after a particularly brutal conflict. Her gentle demeanor and compassionate words provide solace in a harsh world."
    }
]
```

# Usage
## Accessing the Data
To load the dataset in your project, you can use the following code snippet:
```python
from datasets import load_dataset

dataset = load_dataset("NousResearch/CharacterCodex")
```

## Use Cases
- Seed Data: Useful for generating synthetic data or use in interactive experiences with generative AI.
- Creative Writing: Use the detailed character descriptions and scenarios to inspire creative writing projects.
- Educational: Study character development and storytelling techniques from various genres and media types.

# Dataset Creation
## Data Collection
The characters in this dataset were meticulously selected from a diverse range of media, ensuring a rich and varied collection. The descriptions and scenarios were crafted to provide insightful and engaging context for each character.

## Annotations
Each character entry includes:

- The media type (i.e. Novel, Magazine, Anime), the genre (i.e. action, historical), and the specific source/title of the media they are from (i.e. Pokemon)
- A detailed description highlighting the character's role, traits, and significance.
- A scenario designed to stimulate interactive and immersive experiences.

# Citation
```bibtex
@dataset{character_codex_2024,
  title={Character Codex},
  author={"Teknium"},
  year={2024},
  note={https://huggingface.co/datasets/NousResearch/CharacterCodex}
}
```