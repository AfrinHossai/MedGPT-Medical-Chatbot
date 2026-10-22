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
- **Interactive Interface:** Provides a user-friendly chatbot application built with Gradio.
- **User Profile Interface:** Includes a basic user profile and demonstration login interface.
- **Chat History:** Supports viewing recent conversations.
- **Model Fine-Tuning:** Uses the MedQuAD dataset to adapt BioGPT for medical question answering.
- **Model Evaluation:** Includes evaluation metrics and visualizations to analyze model performance.

## Project Files

- `MedGPT.ipynb` — Main implementation, model fine-tuning, evaluation, and chatbot application code.
- `MedGPT_Report.pdf` — Detailed project report, including methodology, implementation, and results.
- `MedGPT_Demo.mp4` — Video demonstration of the MedGPT chatbot.
- `README.md` — Project overview, features, technologies, and instructions.
- `.gitignore` — Specifies files and folders excluded from Git tracking.

## Dataset

This project uses the **MedQuAD (Medical Question Answering Dataset)**, which contains medical questions and answers collected from trusted health information sources.

The dataset is used to fine-tune BioGPT for generating responses to medical questions.

**Dataset Source:** [MedQuAD — GitHub](https://github.com/abachaa/MedQuAD)

**Note:** The notebook references `medquad.csv`, which is not included in this repository. Users must obtain and prepare the dataset in the expected format before running the notebook.

## How to Run the Project

### 1. Clone the Repository

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

Install the Python libraries required by the notebook:

```bash
pip install torch transformers datasets pandas matplotlib gradio openai-whisper
```

Additional dependencies may be required depending on the execution environment and notebook configuration.

### 4. Prepare the Dataset

Download and prepare the MedQuAD dataset, then provide the expected `medquad.csv` file in the location referenced by the notebook.

### 5. Run the Notebook

Execute the notebook cells in sequence to:

1. Load and preprocess the dataset.
2. Initialize the BioGPT model and tokenizer.
3. Fine-tune the model on medical question-answer pairs.
4. Evaluate the model's performance.
5. Launch the Gradio chatbot application.

Model training may require GPU acceleration and sufficient memory.

The repository does not include pretrained fine-tuned checkpoints, so users may need to complete training before testing the chatbot.

## Project Demonstration

A video demonstration of the chatbot is available in:

**[Watch MedGPT Demo](MedGPT_Demo.mp4)**

The demonstration showcases the user interface and chatbot functionality.

## Project Report

For detailed information about the methodology, implementation, and results, see:

**[View MedGPT Project Report](MedGPT_Report.pdf)**

## Limitations

- Generated medical answers may be inaccurate, incomplete, or outdated.
- Model performance depends on the training data and fine-tuning process.
- The application is an academic prototype, not a clinically validated medical system.
- The demonstration login interface does not provide secure authentication.
- Dataset preparation and model training may be necessary before running the application.

## Future Improvements

- Improve response accuracy with additional medical datasets.
- Introduce retrieval-augmented generation (RAG) to support more reliable answers.
- Expand voice-based interaction capabilities.
- Implement secure user authentication.
- Improve evaluation using additional medical question-answering benchmarks.
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
