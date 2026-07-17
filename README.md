

# 🚀 Zero-Shot vs Few-Shot Prompting Comparison


---

# 📖 Project Overview

This project demonstrates the difference between **Zero-Shot Prompting** and **Few-Shot Prompting** using three Large Language Models (LLMs):

- 🤖 ChatGPT
- 🧠 Claude
- ✨ Gemini

The task was to classify **10 customer support messages** into one of the following categories:

- ❌ Complaint
- ❓ Question
- ❤️ Praise

The objective was to compare how providing examples (Few-Shot) impacts the models' accuracy and consistency compared to using only instructions (Zero-Shot).

---

# 🎯 Objectives

- Understand Zero-Shot Prompting
- Understand Few-Shot Prompting
- Compare responses across different LLMs
- Analyze the impact of prompt design

---

# 📂 Repository Structure

```
zero-shot-vs-few-shot-prompting/
│
├── README.md
├── dataset/
│   └── customer_support_messages.csv
│
├── prompts/
│   ├── zero_shot_prompt.md
│   └── few_shot_prompt.md
│
├── results/
│   ├── chatgpt_zero_shot.md
│   ├── chatgpt_few_shot.md
│   ├── claude_zero_shot.md
│   ├── claude_few_shot.md
│   ├── gemini_zero_shot.md
│   └── gemini_few_shot.md
│
└── images/
    ├── chatgpt.png
    ├── claude.png
    └── gemini.png
```

---

# 📊 Dataset

The dataset contains **10 customer support messages**.

Each message belongs to exactly one category:

| Category | Description |
|-----------|-------------|
| ❌ Complaint | Customer reports a problem or expresses dissatisfaction |
| ❓ Question | Customer requests information |
| ❤️ Praise | Customer expresses satisfaction or appreciation |

---

# 📝 Prompting Techniques

## 🔹 Zero-Shot Prompting

The model receives only instructions without any examples.

📄 Prompt:

```
Classify each customer support message into exactly one category:

- Complaint
- Question
- Praise
```

---

## 🔹 Few-Shot Prompting

The model receives instructions along with three labeled examples before classifying the dataset.

Example:

```
Message: My order arrived broken.
Category: Complaint
```

This helps the model understand the expected pattern.

---

# 📈 Results

| Model | Zero-Shot | Few-Shot |
|--------|-----------|-----------|
| ChatGPT | ✅ 10/10 | ✅ 10/10 |
| Claude | ⚠️ 9/10 | ✅ 10/10 |
| Gemini | ⚠️ 9/10 | ✅ 10/10 |

---

# 🔍 Key Findings

- ✅ Few-Shot prompting produced more consistent predictions.
- ✅ Examples reduced ambiguity.
- ✅ Response formatting was more reliable.
- ✅ Providing examples helped models better understand the classification task.

---

# 🖼️ Screenshots

## 🤖 ChatGPT

![ChatGPT](images/chatgpt.png)

---

## 🧠 Claude

![Claude](images/claude.png)

---

## ✨ Gemini

![Gemini](images/gemini.png)

---

# 💡 Conclusion

This experiment demonstrates that **Few-Shot Prompting** generally improves the consistency and reliability of Large Language Models by providing clear examples before the actual task.

Although Zero-Shot Prompting performed well, Few-Shot Prompting reduced ambiguity and produced more predictable outputs across all three models.

---

# 🛠️ Tools Used

- ChatGPT
- Claude
- Gemini
- GitHub
- Visual Studio Code

---

# 📚 Concepts Covered

- Prompt Engineering
- Zero-Shot Prompting
- Few-Shot Prompting
- Text Classification
- Large Language Models (LLMs)

---

