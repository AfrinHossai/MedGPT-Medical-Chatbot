# MedGPT — AI-Powered Medical Question Answering Chatbot

## Project Overview

MedGPT is an AI-powered medical question answering chatbot developed as a CS 156 project. It uses a fine-tuned BioGPT language model trained on the MedQuAD medical question-answering dataset to generate responses to health-related questions.

The application supports both text and voice interaction through a Gradio-based user interface.

## Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Microsoft BioGPT
- MedQuAD Dataset
- OpenAI Whisper
- Gradio
- Pandas
- Matplotlib

## Key Features

- Medical question answering using a fine-tuned BioGPT model
- Text-based chatbot interface
- Voice-to-text question input using Whisper
- User profile interface
- Recent chat history
- Model training and evaluation
- Visualization of training loss and model evaluation metrics

## Project Files

- `CS156_Project@Afrin.ipynb` — Main implementation, fine-tuning, evaluation, and application code
- `Final Report_Afrin.pdf` — Detailed project report
- `Project Presentation_Afrin.pdf` — Project presentation
- `demo.mp4` — Application demonstration

## How to Run

1. Open the Jupyter notebook in a Python environment.
2. Install the dependencies specified in the notebook, including Gradio and Whisper.
3. Obtain the MedQuAD dataset and provide the expected `medquad.csv` file.
4. Execute the preprocessing and training cells, or load an existing compatible fine-tuned checkpoint.
5. Run the Gradio application cells to launch the chatbot.

**Note:** The fine-tuned model checkpoint and the MedQuAD CSV file are not included in this repository.

## Limitations

MedGPT is an educational research prototype. Generated answers may be inaccurate or incomplete. The login screen is a demonstration interface and does not implement secure user authentication.

**Medical Disclaimer:** MedGPT does not provide professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare professional for medical concerns.

## Author

Afrin Hossain

CS 156 — Academic Project
