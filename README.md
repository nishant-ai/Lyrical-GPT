# Lyrical GPT

Lyrical GPT is a fine-tuned version of OpenAI's GPT-2 model, specifically trained to generate song lyrics in the style of various artists. Leveraging a dataset of song lyrics sourced from Kaggle, this project aims to explore the creative potentials of GPT-2 in the domain of music and text generation.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Fine-Tuning Process](#fine-tuning-process)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributors](#contributors)
- [License](#license)

## Introduction

Generative Pre-Trained Transformer 2 (GPT-2) is an autoregressive language model that uses deep learning to produce human-like text. By fine-tuning GPT-2 on specific datasets, we can tailor its text generation capabilities to particular domains or styles. In this project, we fine-tuned GPT-2 on a collection of song lyrics to create "Lyrical GPT," a model capable of generating lyrics resembling those of various artists.

## Dataset

The dataset used for fine-tuning comprises song lyrics from various artists, sourced from Kaggle. This dataset provided a diverse range of lyrical styles and themes, essential for training a model capable of generating versatile song lyrics.

- Kaggle Dataset: [Song Lyrics Dataset](https://www.kaggle.com/datasets/deepshah16/song-lyrics-dataset)

## Fine-Tuning Process

The fine-tuning process involved several key steps:

1. **Data Preparation**: The lyrics were preprocessed to ensure compatibility with the GPT-2 tokenizer, including cleaning and formatting the text.

2. **Model Selection**: We utilized the 124M parameter version of GPT-2, balancing performance and computational requirements.

3. **Training Configuration**: The model was fine-tuned using the Adam optimizer, with hyperparameters adjusted for our specific dataset and objectives.

4. **Training Execution**: The fine-tuning was conducted over multiple epochs, with periodic evaluation to monitor the model's performance and adjust training parameters as necessary.

For a comprehensive guide on fine-tuning GPT-2, consider reviewing this tutorial: [Fine-Tuning GPT-2 on the IMDb Dataset](https://medium.com/@AyushmanPranav/fine-tuning-gpt-2-on-the-imdb-dataset-a-comprehensive-guide-with-code-implementation-e9452aa5a85b)

## Installation

To utilize Lyrical GPT, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/nishant-ai/Lyrical-GPT.git
   cd Lyrical-GPT
   ```

2. **Create a Virtual Environment**:

   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

   Ensure that the `transformers` and `torch` libraries are included in your `requirements.txt`.

## Usage

To generate song lyrics using Lyrical GPT:

1. **Load the Fine-Tuned Model**:

   Ensure that the fine-tuned model is saved in the `models/` directory.

2. **Run the Text Generation Script**:

   ```bash
   python generate_lyrics.py --prompt "Your song lyric prompt here"
   ```

   Replace `"Your song lyric prompt here"` with a seed text to inspire the generated lyrics.

3. **Adjust Generation Parameters**:

   The script allows for optional parameters such as `--length`, `--temperature`, and `--top_p` to control the creativity and length of the generated lyrics.

## Results

Lyrical GPT demonstrates the ability to generate coherent and stylistically relevant song lyrics based on the input prompt. While the model captures various lyrical themes and structures, further fine-tuning and dataset expansion could enhance its creativity and adherence to specific artist styles.

## Contributors

- **Nishant**: [GitHub Profile](https://github.com/nishant-ai)
- **Madhvan Tyagi**: [GitHub Profile](https://github.com/madhvan97)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For any questions or collaborations, please contact [Nishant](https://github.com/nishant-ai).
