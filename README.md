# Contextual News Analyser

**Contextual News Analyser** is a Python-based tool that provides meaningful insights from raw news content by summarizing articles, classifying topics, and analyzing sentiment—all without the need for labeled training data. The project leverages advanced NLP techniques such as TextRank for summarization, zero-shot learning with BART-large-MNLI for topic classification, and sentiment analysis. The entire workflow is implemented in Jupyter Notebooks for ease of exploration and reproducibility.

## Features

- **Automated News Summarization:** Uses TextRank to generate concise summaries from raw news articles.
- **Topic Classification:** Employs zero-shot learning (BART-large-MNLI) to classify articles into relevant topics without labeled data.
- **Sentiment Analysis:** Analyzes the sentiment of news content to provide further insights.
- **No Labeled Data Needed:** All models operate in an unsupervised or zero-shot manner.
- **Interactive UI:** Final output can be accessed through a simple Tkinter-based graphical user interface.

## Project Structure

- The project is organized as a series of Jupyter Notebook kernels, with each kernel focusing on a major step in the news analysis pipeline:
    1. **Preprocessing & Input:** Load and preprocess news articles.
    2. **Summarization:** Apply TextRank to produce article summaries.
    3. **Topic Classification:** Use zero-shot learning with BART-large-MNLI for topic labeling.
    4. **Sentiment Analysis:** Perform sentiment scoring on the articles.
    5. **UI Integration (Final Kernel):** Bring all results together and create a Tkinter-based graphical interface for end users.

- To obtain the complete output and use the UI, run each kernel sequentially in the provided order, with the final kernel combining all previous steps and launching the Tkinter GUI.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python packages (see individual notebooks for specific requirements):
    - transformers
    - torch
    - nltk
    - scikit-learn
    - tkinter
    - others as specified

### Usage

1. **Clone the Repository**
    ```bash
    git clone https://github.com/jaita005/Contextual-News-Analyser.git
    ```
2. **Install dependencies**  
   Refer to the import cells in each notebook and install the required packages (typically with `pip install package-name`).
3. **Run the Notebooks**
    - Open each Jupyter Notebook kernel in order.
    - Execute all cells in each notebook, as each step builds upon the previous.
4. **Run the Final Kernel**
    - The last notebook integrates the summarization, classification, and sentiment analysis, and launches the Tkinter GUI for interactive use.

## Example Links to Test

You can use the following example news URLs to paste into the tool and test its functionality:

- https://edition.cnn.com/2025/04/12/science/milky-sea-ocean-glow-mystery-database/index.html
- https://edition.cnn.com/2025/04/12/weather/why-storms-have-been-so-bad/index.html

## Customization

- Modify the topic candidate list for zero-shot classification to suit your use case.
- Adjust summarization or sentiment parameters as needed in the respective notebooks.

## License

This project is open source and available under the MIT License.

---

**Explore, analyze, and understand news content—no labeled data required!**
