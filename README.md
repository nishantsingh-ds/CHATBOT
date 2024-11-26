# Intelligent QnA Chatbot for Hotel Reservations

This project implements an intelligent chatbot designed to handle hotel reservation queries using deep learning models. The chatbot evolves from simple Recurrent Neural Networks (RNNs) to more advanced architectures like LSTM, BRNN, Encoder-Decoder networks, and concludes with the integration of BERT using HuggingFace Transformers for state-of-the-art natural language understanding.

## Key Features
- **Custom RNN:** Implemented from scratch for basic intent classification.
- **Sequential RNN:** Built using prebuilt Sequential API to improve model efficiency.
- **LSTM & BRNN:** Advanced RNNs that handle long-term dependencies and bidirectional context for better understanding of input queries.
- **Encoder-Decoder Models:** Used to handle longer sequences with attention mechanisms.
- **BERT Integration:** Fine-tuned BERT with HuggingFace Transformers for highly accurate contextual question answering.

## Technologies Used
- **Deep Learning Models:** RNN, LSTM, BRNN, Encoder-Decoder, BERT
- **Frameworks:** TensorFlow, Keras, HuggingFace Transformers
- **Programming Language:** Python
- **Data Preprocessing:** Tokenization, Text Cleaning, NLP techniques
- **Hardware:** NVIDIA RTX 3090 GPU for training

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Intelligent-QnA-Chatbot.git
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## How It Works

### Step 1: Data Preprocessing
- The input queries are preprocessed using tokenization, padding, and cleaning techniques.
- Training datasets are prepared for different models, such as `intents.json` for basic tasks and the CoQA dataset for BERT fine-tuning.

### Step 2: Model Development
- **Custom RNN:** Built from scratch to classify intents and map to responses.
- **Sequential RNN:** Implemented using TensorFlow/Keras Sequential API for better performance and efficiency.
- **LSTM & BRNN:** Used to enhance context comprehension and handle long-range dependencies.
- **Encoder-Decoder:** Further improved model performance by using attention mechanisms for better sequence handling.

### Step 3: BERT Integration
- Fine-tuned the BERT model using HuggingFace Transformers for extractive question answering on the CoQA dataset.
- Integrated BERT to achieve domain-agnostic question answering with high contextual accuracy.

### Step 4: Evaluation
- Each model is evaluated on its ability to handle hotel reservation queries with varying complexity and context. BERT outperforms all other models in terms of response accuracy and contextual understanding.

## Results
- **Custom RNN:** Basic accuracy with limited context comprehension.
- **Sequential RNN:** Improved accuracy and efficiency over the custom RNN.
- **LSTM & BRNN:** High performance with strong contextual understanding.
- **BERT:** State-of-the-art results with excellent natural language understanding and generalization across different queries.

## Future Improvements
- **Real-time Deployment:** Optimize BERT model for faster inference to enable real-time usage.
- **Multi-turn Dialogue:** Enhance the chatbot's ability to handle multi-turn conversations for a more dynamic user experience.
- **Domain-Specific Tuning:** Fine-tune models for specific domains (e.g., hotel reservations, customer support).

## Contributing
Feel free to fork this repository and submit pull requests. Contributions are always welcome!
