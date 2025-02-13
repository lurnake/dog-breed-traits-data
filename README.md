# Dog Breed Traits Dataset

This repository contains a comprehensive dataset of dog breeds and their characteristics, along with AI-generated similarity scores and embeddings. The data can be used for research, analysis, and creating new representations of breed-trait relationships.

## Dataset Contents

The repository includes the following JSON files:

- `dog-breeds.json`: Comprehensive list of dog breeds categorized by traditional groups
- `breed-characteristics.json`: Curated list of dog traits and characteristics covering temperament, behavior, and living compatibility
- `trait-breed-similarity.json`: AI-generated similarity scores (0-100) indicating how strongly each trait applies to each breed
- `breed-trait-similarity.json`: Alternative view of the similarity data organized by breeds
- `breed-characteristics-with-embeddings.json`: OpenAI text-embedding-3-large embeddings for breed characteristics
- `dog-breeds-with-embeddings.json`: OpenAI text-embedding-3-large embeddings for breed names and descriptions

## Methodology

The similarity scores in this dataset were generated using two different approaches:

1. Initial Approach: Cosine similarity between OpenAI text-embedding-3-large embeddings of breeds and traits
2. Final Approach: Direct scoring by Google's Gemini-2.0-Pro-Experimental (02-05) model, rating each breed-trait combination on a scale of 0-100

The final approach (Gemini scoring) was chosen for the production system as it produced more accurate and nuanced results compared to the embedding-based approach.

## Data Format Examples

```json
// breeds.json example
{
  "sporting_dogs": [
    "Labrador Retriever",
    "Golden Retriever",
    // ...
  ],
  // ...
}

// characteristics.json example
{
  "temperament_personality": [
    "independent and self-reliant",
    "stubborn and strong-willed",
    // ...
  ],
  // ...
}

// trait-breed-similarity.json example
{
  "retrieves from water eagerly": {
    "Labrador Retriever": 95,
    "Golden Retriever": 92,
    // ...
  }
}
```

## Usage

This dataset is freely available for research, analysis, and derivative works. You can use it to:

- Study breed-trait relationships
- Create visualizations of breed characteristics
- Train machine learning models
- Develop dog breed recommendation systems
- Conduct research on AI understanding of dog breeds

## License and Attribution

This dataset is available under open-source principles with the following requirements:

1. Attribution must be given to:
   - The project: "Dog Breed Traits Dataset"
   - The author: Joona Heino
2. If you use this data in research, publications, or applications, please include appropriate citations
3. Any derivative works should maintain these attribution requirements

## Contributing

If you'd like to contribute to improving the dataset or have suggestions, please:

1. Open an issue to discuss proposed changes
2. Submit pull requests with improvements
3. Share research findings using the dataset

## Contact

For questions or collaboration opportunities, contact Joona Heino on X (Twitter): [@joonaheino](https://x.com/joonaheino)

## Citation

When using this dataset in academic or research contexts, please cite:

```
Heino, J. (2024). Dog Breed Traits Dataset. [https://github.com/lurnake/dog-breed-traits-data](https://github.com/lurnake/dog-breed-traits-data)]
```
