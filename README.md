# DPO vs. RLHF: Generalizability vs. Diversity

This repository explores the concepts of generalizability and diversity in the context of **Direct Preference Optimization (DPO)** and **Reinforcement Learning from Human Feedback (RLHF)**. The experiments and analyses aim to compare these two approaches to better understand their respective strengths and weaknesses in generating diverse yet generalizable outputs.

![Visualization 1](https://github.com/PranavGrandhi/DPO_RLHF/assets/39693342/4c7b63fa-5804-4edc-9985-7df3c39ce813)
![Visualization 2](https://github.com/PranavGrandhi/DPO_RLHF/assets/39693342/3ffa2b75-d138-46d8-a0df-4a57d7a9a6ff)

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The goal of this project is to provide a comprehensive comparison between Direct Preference Optimization (DPO) and Reinforcement Learning from Human Feedback (RLHF). While both methods are commonly used in machine learning to fine-tune language models, they have distinct differences that impact their performance in terms of output generalizability and diversity. This repository includes:

- Analysis notebooks that cover various aspects of generalizability and diversity.
- Scripts for reproducing experiments.
- Results and visualizations that illustrate the performance of DPO and RLHF across different benchmarks.

## Project Structure

- `DPO_Training.ipynb`: Notebook for training models using Direct Preference Optimization.
- `dpo.ipynb`: Supplementary notebook for DPO-related experiments.
- `SFT_Diversity_Gaps.ipynb`: Analyzes gaps in diversity when using Supervised Fine-Tuning (SFT).
- `SFT_Inference_Generalizability_CNN.ipynb`: Evaluates the generalizability of SFT models using a CNN architecture.
- `SFT_Inference_Generalizability.ipynb`: Generalization analysis for SFT models.
- `SFT_Inference.ipynb`: Core inference analysis notebook.
- `GPT4Responses_Generalization.jsonl` and `GPT4Responses_Generalization_cnn.jsonl`: Data files containing responses and generalization metrics.
- `SFT_Summaries.jsonl`: Summaries of SFT experiments.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook
- Required Python packages (listed in `requirements.txt`)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/DPO_RLHF.git
    cd DPO_RLHF
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Open the Jupyter notebooks in your preferred environment:

    ```bash
    jupyter notebook
    ```

2. Run the notebooks to reproduce the results and visualizations. Start with `DPO_Training.ipynb` and follow the instructions within each notebook.

## Results

The results of our experiments show:

- **DPO**: Tends to offer more robust generalizability across varied datasets but may sacrifice some degree of diversity in outputs.
- **RLHF**: Often achieves greater diversity in outputs, particularly when tuned with diverse human feedback, but may lack in generalizability across datasets not seen during training.

Visualizations of these results can be found in the provided figures and notebooks.

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
