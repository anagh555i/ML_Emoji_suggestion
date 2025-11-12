# ML_Emoji_suggestion
A machine‑learning based system to suggest emojis for text. Developed by Anagh.

## 🚀 Project Overview
This project aims to help users automatically generate relevant emoji suggestions for a given piece of text. By analyzing sentiment, context and keywords, the model proposes emoji(s) that best match the emotional tone or meaning of the text.

### Why this?
- Adds fun and expressiveness to text communication.
- Bridges the gap between plain text and emotional cues in messaging.
- Demonstrates application of NLP + classification/regression techniques.
- Great for chat apps, social platforms, or enhancing UX with emoji assistance.

## 📁 Repository Structure
```
├── .gitignore
├── README.md
├── modelTraining.ipynb        ← Notebook for training the model
├── main.ipynb                 ← Notebook for running inference / testing other implementations
├── Testing.ipynb              ← Notebook for evaluation / experimenting
```

Make sure you have Python installed (version 3.7+ recommended). Required libraries include:

- `pandas`  
- `numpy`  
- `scikit-learn`  
- `tensorflow` or `keras` 
- `jupyter` / `jupyterlab`  
- `customtkinter` (optional, for UI)

## 🧠 How it Works
1. **Data preprocessing**: Clean and normalize text, remove noise, tokenize, possibly embed.
2. **Word vectorization**: embedd each token to word vector
3. **Model training**: Train a classifier/regressor (or multi‑label classifier) that maps text → emoji(s).
4. **Evaluation**: Validate model performance using appropriate metrics (accuracy, F1, etc.).
5. **Inference/demo**: Provide text input and get back suggested emoji(s).

## 🔧 Getting Started
### Prerequisites
- Python 3.x
- Jupyter Notebook
- Major libraries: `numpy`, `pandas`, `scikit‑learn`, possibly `tensorflow` or `pytorch` (depending on your implementation)
- Any additional dependencies listed in a future `requirements.txt`
- Dataset required: `tweeteval-a-multi-task-classification-benchmark`
- pre-trained word vectors : `Twitter (2B tweets, 27B tokens, 1.2M vocab, uncased, 25d, 50d, 100d, & 200d vectors, 1.42 GB download)`

### Instructions
1. Clone the repo:
   ```bash
   git clone https://github.com/anagh555i/ML_Emoji_suggestion.git
   cd ML_Emoji_suggestion
   ```
2. Download and extract Dataset into the same folder:
    ```
   https://www.kaggle.com/datasets/thedevastator/tweeteval-a-multi-task-classification-benchmark/data
    ```
3. Download and extract the pretrained word vector models:
   ```
   https://nlp.stanford.edu/projects/glove/
    ```
4. Open the training notebook:
   ```bash
   jupyter notebook modelTraining.ipynb
   ```
   - Run through the data preprocessing steps, feature engineering, model training and saving the model.
5. To test/infer: open `main.ipynb` and supply sample texts to generate suggested emojis.
6. Use `Testing.ipynb` to evaluate and experiment with different model architectures or parameters.

## 📊 Sample Usage
In `main.ipynb`, provide input like:
> _“Just finished my final exams – feeling free!”_
and the system might suggest: 🥳 🎉 😎
*(Actual suggestions depend on model training & emoji mapping.)*

## ✅ Next Steps & Improvements
- Expand dataset: include more diverse text and emoji mappings for better generalization.
- Upgrade model architecture: try deep‑learning based approaches (LSTM, Transformer) for context understanding.
- Multi‑label output: suggest multiple relevant emojis rather than a single one.

## 📝 Contributing
Contributions are welcome! If you find bugs, have ideas for improvement or want to add new emoji‑mappings, feel free to fork the repository, make your changes and submit a pull request.
Please include clear description of your changes and ensure notebooks run without errors.

## 📄 License
This project is open‑source — feel free to use, modify and distribute.

---

Thank you for checking out the project! If you have any feedback or questions, please reach out via GitHub issues or contact me (Anagh).
Happy coding and emoji‑suggesting! 🎉