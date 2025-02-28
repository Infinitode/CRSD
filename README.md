# CRSD (Customer Review Sentiment Dataset)

## Overview

The **CRSD (Customer Review Sentiment Dataset)** is a synthetic dataset designed for sentiment analysis tasks. It consists of approximately **6,500** customer reviews, each labeled with a sentiment category: **positive**, **neutral**, or **negative**. These reviews were generated using a variety of AI language models to ensure diversity and realism in language style and content. The inclusion of multiple models enhances the dataset's robustness and provides insights into the performance of different generative AI systems.

> [!TIP]
> This dataset is also publicly available on Hugging Face: https://huggingface.co/datasets/InfinitodeLTD/CRSD

## Contents

- `data.csv`: The main dataset file in CSV format.

## Data Structure

The dataset CSV file includes the following columns:

- **`review`**: The text of the customer review.
- **`sentiment`**: The sentiment label corresponding to the review (`positive`, `neutral`, `negative`).
- **`model`**: The AI model used to generate the review.

### Example Entries

| review                                                       | sentiment | model                     |
|--------------------------------------------------------------|-----------|---------------------------|
| "Absolutely fantastic product! Exceeded all my expectations."| positive  | GPT-4o-Mini               |
| "It's okay, nothing extraordinary but does the job."         | neutral   | GPT-4o-Mini               |
| "Terrible experience. Would not recommend to anyone."        | negative  | GPT-4o-Mini               |

## Data Generation Process

The reviews were synthetically generated using a selection of advanced AI language models, including:

- **Google's Gemini 1.5-Flash**
- **Google's Gemini 2.0-Flash-Lite**
- **OpenAI's GPT-4o-Mini**
- **Meta's Llama 3-8b-T**
- **Mistral AI's Mixtral 8x7b**

Prompts were crafted to elicit reviews of varying sentiments. For example:

- **Positive**: "Write a positive review for a product, be descriptive and human-like."
- **Neutral**: "Write a neutral review for a product, be descriptive and human-like."
- **Negative**: "Write a negative review for a product, be descriptive and human-like."

The generated reviews were then labeled accordingly, and the model used for generation was recorded in the `model` column.

## Dataset Statistics

- **Total reviews**: Approximately 6,500
- **Models used**:
  - Gemini 1.5-Flash
  - Gemini 2.0-Flash-Lite
  - GPT-4o-Mini
  - Llama 3-8b-T
  - Mixtral 8x7b

> [!NOTE]
> Models were not used equally to generate equal amounts of reviews. During inference, most models struggle to keep track of the amount of reviews already generated.

## Usage

### Potential Applications

- **Training and evaluating sentiment analysis models**: Ideal for developing machine learning models that classify customer reviews based on sentiment.
- **Natural Language Processing (NLP) research**: Useful for tasks like text classification, language understanding, and generation.
- **Educational purposes**: Suitable for teaching concepts in data science, machine learning, and NLP courses.
- **Benchmarking AI models**: Can be used to assess model performance on synthetic data generated by different AI systems.

## Limitations

- **Synthetic Nature**: The dataset is artificially generated and may not capture all the complexities and nuances of real customer reviews.
- **Biases**: Potential biases inherent in the AI models used for generation may be present in the dataset.
- **Model Artifacts**: The language style and structures may reflect tendencies of the generating models rather than authentic human expression.
- **Limited Domains**: The reviews are generic and not focused on any specific product categories or industries.

## Out-of-Scope Uses

The dataset should **NOT** be used for:

- **NSFW (Not Safe For Work) Applications**: Content involving explicit, offensive, or inappropriate material.
- **Medical or Legal Advice Systems**: Applications requiring professional advice or that could impact health and legal rights.
- **Defamation**: Creating content that could harm the reputation of individuals or organizations.
- **Any form of malicious activities**: Including but not limited to spam generation, harassment, or disinformation campaigns.

## Ethical Considerations

- **Responsible Use**: Users should ensure that the dataset is used ethically and in compliance with applicable laws and regulations.
- **Bias Mitigation**: Be aware of and address potential biases when using the dataset in model training and evaluations.
- **Transparency**: When publishing results or deploying models trained on this dataset, disclose the synthetic nature of the data.

## License

This dataset is provided under the **MIT License**. You are free to use, modify, and distribute the dataset, provided you include the original license and attribution.

## Citation

If you use this dataset in your research or project, please cite it as follows:

```bibtex
@dataset{crsd_2025,
  author       = {Infinitode},
  title        = {{CRSD}: Customer Review Sentiment Dataset},
  year         = {2025},
  publisher    = {Hugging Face},
  url          = {https://github.com/Infinitode}
}
```

## Acknowledgements

This dataset was generated using various AI models, with contributions from the Hugging Face community and the developers of OpenAI's GPT series, Google's Gemini, Meta's Llama, and Mistral AI's Mixtral.

## Contact Information

For questions, feedback, or contributions, please contact:

- **GitHub**: [Infinitode](https://github.com/Infinitode)
- **Website**: https://infinitode.netlify.app/forms/contact

## Contribution Guidelines

Contributions to improve the dataset are welcome. Please submit a pull request or open an issue or discussion.

## Frequently Asked Questions (FAQ)

**Q1: Can I use this dataset for commercial purposes?**

Yes, the dataset is licensed under the MIT License, which permits commercial use, provided you include the original license and attribution.

**Q2: Are there any real customer data in this dataset?**

No, all reviews are synthetically generated using AI models and do not contain any real customer data.

**Q3: How can I contribute to improving the dataset?**

You can contribute by submitting pull requests with enhancements or by opening issues to discuss potential improvements.