# MedGPT — AI-Powered Medical Question Answering Chatbot

## Project Overview

MedGPT is an AI-powered medical question answering chatbot developed as a CS 156 academic project. It uses a fine-tuned BioGPT language model trained on the MedQuAD medical question-answering dataset to generate responses to health-related questions.

The application supports both text and voice interaction through a user-friendly Gradio interface.

The goal of this project is to explore how natural language processing (NLP) and machine learning can be applied to medical question answering, making health-related information more accessible through conversational AI.

## Technologies Used

- **Programming Language:** Python
- **Deep Learning Framework:** PyTorch
- **NLP Library:** Hugging Face Transformers
- **Language Model:** Microsoft BioGPT
- **Dataset:** MedQuAD
- **Speech Recognition:** OpenAI Whisper
- **User Interface:** Gradio
- **Data Processing:** Pandas
- **Visualization:** Matplotlib
- **Development Environment:** Jupyter Notebook

## Key Features

- **Medical Question Answering:** Generates responses to medical questions using a fine-tuned BioGPT model.
- **Text-Based Interaction:** Allows users to enter health-related questions through a chatbot interface.
- **Voice Input:** Converts spoken questions into text using OpenAI Whisper.
- **Interactive Interface:** Provides a chatbot application built with Gradio.
- **User Profile Interface:** Includes a basic user profile and demonstration login interface.
- **Chat History:** Supports viewing recent conversations.
- **Model Fine-Tuning:** Uses the MedQuAD dataset to adapt BioGPT for medical question answering.
- **Model Evaluation:** Includes evaluation metrics and visualizations to analyze model performance.

## Project Files

- `MedGPT.ipynb` — Main implementation, model fine-tuning, evaluation, and chatbot application code.
- `MedGPT_Report.pdf` — Detailed project report, including methodology, implementation, and results.
- `MedGPT_Demo.mp4` — Video demonstration of the MedGPT chatbot.
- `requirements.txt` — Python dependencies required for the project.
- `README.md` — Project documentation and instructions.
- `.gitignore` — Files and directories excluded from Git tracking.

## Dataset

This project uses the **MedQuAD (Medical Question Answering Dataset)** to fine-tune BioGPT for medical question answering.

**Original dataset:** [MedQuAD — GitHub](https://github.com/abachaa/MedQuAD)

The project uses a processed CSV file named `medquad.csv` containing 16,412 question-answer records.

The CSV contains the following columns:

- `question` — Medical questions.
- `answer` — Corresponding medical answers.
- `source` — Source information.
- `focus_area` — Medical topic or focus area.

### Dataset Setup

1. Obtain the original MedQuAD dataset from the GitHub link above.
2. Convert the original XML question-answer records into CSV format with the columns `question`, `answer`, `source`, and `focus_area`.
3. Save the processed CSV as `medquad.csv`.
4. Place `medquad.csv` in the notebook's working directory.
5. Run `MedGPT.ipynb`.

**Note:** The processed CSV is not included in this repository and is excluded using `.gitignore`. The XML-to-CSV conversion script is not currently provided, so dataset preparation must be completed separately.

## How to Run the Project

### 1. Clone the Repository

Open a terminal and run:

```bash
git clone https://github.com/AfrinHossai/MedGPT-Medical-Chatbot.git
```

### 2. Open the Project

Navigate to the project directory:

```bash
cd MedGPT-Medical-Chatbot
```

Open `MedGPT.ipynb` using Jupyter Notebook or Google Colab.

### 3. Install Dependencies

Install the required Python libraries using:

```bash
python -m pip install -r requirements.txt
```

The project uses PyTorch, Hugging Face Transformers, Microsoft BioGPT, OpenAI Whisper, and Gradio.

**Note:** OpenAI Whisper also requires FFmpeg for audio processing. Additional setup may be needed depending on your operating system and hardware. The dependency versions have not been pinned or validated in a fresh environment.

### 4. Prepare the Dataset

Follow the instructions in the **Dataset Setup** section above.

Make sure the `medquad.csv` file is available in the notebook's working directory before running the dataset-loading cells.

### 5. Run the Notebook

Execute the notebook cells in sequence to:

1. Load and preprocess the dataset.
2. Initialize the BioGPT model and tokenizer.
3. Fine-tune the model on medical question-answer pairs.
4. Evaluate the model's performance.
5. Launch the Gradio chatbot application.

Model training may require GPU acceleration and sufficient memory.

The repository does not include fine-tuned model checkpoints, so users may need to complete training before testing the chatbot.

## Project Demonstration

A video demonstration of the chatbot is available here:

**[Watch MedGPT Demo](MedGPT_Demo.mp4)**

The demonstration showcases the chatbot's user interface and functionality.

## Project Report

For detailed information about the methodology, implementation, and results, see:

**[View MedGPT Project Report](MedGPT_Report.pdf)**

## Limitations

- Generated medical answers may be inaccurate, incomplete, or outdated.
- Model performance depends on the training data and fine-tuning process.
- The application is an academic prototype, not a clinically validated medical system.
- The demonstration login interface does not provide secure authentication.
- Dataset preparation and model training may be necessary before running the application.
- The full installation and execution workflow has not been independently verified in a clean environment.

## Future Improvements

- Improve response accuracy with additional medical datasets.
- Introduce retrieval-augmented generation (RAG) to support more reliable answers.
- Expand voice-based interaction capabilities.
- Implement secure user authentication.
- Improve evaluation using additional medical question-answering benchmarks.
- Provide an automated dataset preparation script.
- Pin and test dependency versions for reproducibility.
- Deploy the chatbot as an accessible web application.

## Medical Disclaimer

**MedGPT is an educational and research project only.**

It is not intended to provide professional medical advice, diagnosis, or treatment. Generated responses should not be used as a substitute for consultation with qualified healthcare professionals.

## Author

**Afrin Hossain**

CS 156 — Academic Machine Learning Project

**GitHub:** [AfrinHossai](https://github.com/AfrinHossai)

## Acknowledgments

- Microsoft Research — BioGPT
- MedQuAD dataset contributors
- Hugging Face — Transformers ecosystem
- OpenAI — Whisper
- Gradio — Interactive machine learning interfaces
