# Classifying-GitHub-Issues-LLMs

![GitHub Issues Classification](Project_1_Image_Classification_Issue.png) 

A machine learning-based GitHub issue classifier that categorizes issues into Feature, Bug, or Question using Fine-tuned LLMs (GPT-3.5-turbo, Mistral 7B, Llama 3) with RAG (FAISS/BM25) for improved accuracy.

📝 Project Overview:

    🎯 Goal: Automatically classify GitHub issues using fine-tuned LLMs.
    🧠 Models Used: GPT-3.5-turbo-0125, Mistral 7B, Llama 3.
    🔍 Retrieval Augmented Generation (RAG): FAISS & BM25 used for contextual improvement.
    📊 Achievements:
        ✅ Precision: 87.51%
        ✅ Recall: 87.00%
        ✅ F1-score: 86.73%

## 🚀 Tech Stack

| Category         | Tools Used |
|-----------------|------------|
| 💻 Programming | Python |
| 📡 API | GitHub API |
| 🔎 Vector Search | FAISS, BM25 |
| 🧠 ML Frameworks | OpenAI, Hugging Face |
| 📂 Dataset | GitHub Issues (Feature, Bug, Question) |
| 🎯 Deployment |  Google Collab |



🚀 Setup & Installation
Follow these steps to run the project locally:

1️⃣ Clone the Repository
git clone https://github.com/Narayana27/Classifying-GitHub-Issues-LLMs.git
cd Classifying-GitHub-Issues-LLMs


2️⃣ Install Dependencies
pip install -r requirements.txt


3️⃣ Run the Model
python classify_issues.py


4️⃣ Fine-Tune GPT-3.5
python
from openai import OpenAI
client = OpenAI(api_key="YOUR_API_KEY")

ft_job = client.fine_tuning.jobs.create(
    training_file="issues_train.jsonl",
    model="gpt-3.5-turbo-0125"
)


📊 Model Performance
Metric	Value
Precision	87.51%
Recall	87.00%
F1-Score	86.73%


### 🔹 Confusion Matrix

| Actual \ Predicted | Feature | Bug | Question |
|-------------------|---------|-----|----------|
| **Feature**       | 94      | 16  | 6        |
| **Bug**           | 94      | 17  | 6        |
| **Question**      | 73      | 6   | 27       |


🛠️ Future Improvements
✅ Enhance question classification by increasing training data.
✅ Implement better context retrieval (RAG) for improved accuracy.
✅ Optimize training for lower computational cost.

💡 Contributions are welcome! If you’d like to enhance this project, feel free to submit a pull request.

---

## **⚙️ Setup & Installation**
Follow these steps to run the project locally:
1. **Edit Your README.md in VS Code**
   - Open `README.md` in **VS Code** and replace the content with the above Markdown.
   - Save the file (`Ctrl + S`).

2. **Push the Changes to GitHub**
   Run these commands in **VS Code Terminal**:
   ```bash
   git add README.md
   git commit -m "Updated README with project details"
   git push origin main
