# Semantic Book Recommender with LLMs

This project implements a **Semantic Book Recommender System** using **Large Language Models (LLMs)**. It allows users to find books based on semantic similarity, classify books as fiction or non-fiction, analyze sentiment, and interact with a **Gradio-based web application** for recommendations.

## Project Components

The project is divided into the following modules:

### Data Preprocessing (`Data_Preprocessing.ipynb`)

- Cleans and processes book text data.
- Prepares the dataset for further analysis.

### Vector Search (`vector_search.ipynb`)

- Implements **semantic search** using vector databases.
- Uses **Hugging Face embeddings** (`sentence-transformers/all-MiniLM-L6-v2`) for vector representation.
- Enables book retrieval based on natural language queries (e.g., "a thrilling detective story").

### Category Classification (`category_classifiction.ipynb`)

- Performs **zero-shot classification** to label books as **fiction** or **non-fiction**.
- Helps users filter books based on category.

### Sentiment Analysis (`sentiment_analysis_for_Book_Recommender.ipynb`)

- Extracts emotions from book descriptions using **LLMs**.
- Allows sorting books based on tone (e.g., suspenseful, joyful, sad).

### Gradio Dashboard (`Book_Recommender_Gradio (1).ipynb`)

- Builds an interactive **Gradio-based web app** for book recommendations.
- Provides an intuitive UI for users to search and explore books.

## Dependencies

Install the necessary dependencies manually:

```bash
pip install kagglehub pandas matplotlib seaborn langchain-community langchain-opencv langchain-chroma transformers gradio notebook ipywidgets
```

## Setup Instructions

1. Clone this repository:

   ```bash
   git clone https://github.com/Dikshitharyana/LLM---Book-Recommender
   cd LLM---Book-Recommender
   ```

2. Download the dataset from Kaggle (instructions provided in the course/tutorial).

3. Run the notebooks in the following order:

   - `Data_Preprocessing.ipynb`
   - `vector_search.ipynb`
   - `category_classifiction.ipynb`
   - `sentiment_analysis_for_Book_Recommender.ipynb`
   - `Book_Recommender_Gradio (1).ipynb`

4. Start the Gradio web application:

   ```bash
   python Book_Recommender_Gradio (1).ipynb
   ```

## Features

- **Natural Language Book Search**: Find books using semantic similarity.
- **Genre Classification**: Filter books by fiction/non-fiction.
- **Sentiment-Based Sorting**: Sort books by emotional tone.
- **Interactive UI**: Use Gradio to explore book recommendations.

---

Enjoy exploring books with AI-powered recommendations!

