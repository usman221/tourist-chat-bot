# Smart Tourist: Multilingual Document-Based Question Answering System

## Overview

Smart Tourist is an advanced document-based question answering system designed to perform semantic search across multiple languages. It can seamlessly translate and interpret Arabic documents into English, Arabic, Spanish, and more. The system leverages cutting-edge multilingual embeddings and sophisticated search algorithms to deliver accurate and contextually relevant answers.

## Features

- **Semantic Search**: Utilizes advanced semantic search capabilities to find answers within documents.
- **Multilingual Support**: Translates and interprets documents in Arabic to multiple languages including English, Arabic, Spanish, and others.
- **Embedding Options**:
  - **Default Embedding**: Uses the `ada2` embedding model from OpenAI for robust language understanding.
  - **Optional Multilingual Embedding**: Integrates with Cohere for specialized multilingual embeddings, supporting dot product operations for enhanced search accuracy.
- **Search Metrics**:
  - **Euclidean Distance**: Measures the straight-line distance between two points in the embedding space.
  - **Cosine Similarity**: Evaluates the cosine of the angle between two vectors, indicating their similarity in terms of direction.
- **Framework**: Built on the Flask framework, ensuring a robust and scalable web application.
- **Document Support**: Handles a variety of document formats including PDF, DOCX, MD, and HTML.

## How It Works

1. **Document Processing**: The system ingests documents in supported formats and processes them for analysis.
2. **Embedding Generation**: Documents are embedded using either the default OpenAI `ada2` model or the optional Cohere multilingual model.
3. **Search Query Processing**: User queries are also embedded and compared against the document embeddings using either Euclidean distance or cosine similarity.
4. **Result Retrieval**: The system retrieves the most relevant documents or passages based on the search metrics.
5. **Translation and Interpretation**: If necessary, the system translates the retrieved content into the user's preferred language.

## Getting Started

To set up and run Smart Tourist locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/smart-tourist.git
   cd smart-tourist
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Embedding Models**:
   - Set up your OpenAI API key in the configuration file.
   - Optionally, configure the Cohere API for multilingual embeddings.

4. **Run the Application**:
   ```bash
   python app.py
   ```

5. **Access the Application**: Open your web browser and go to `http://localhost:5000`.

## Contributing

We welcome contributions to enhance Smart Tourist. Please read our [Contribution Guidelines](CONTRIBUTING.md) for details on how to contribute.

## Contact

For questions or support, please contact us at [contact@smart-tourist.com](mailto:contact@smart-tourist.com).

---

**Smart Tourist** is committed to enhancing the tourism experience through technology, providing accurate and multilingual information to travelers around the world.
