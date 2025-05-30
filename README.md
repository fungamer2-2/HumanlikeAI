# 💖 Amorelia: Your Friendly, Empathetic Virtual Companion

![GitHub commit activity](https://img.shields.io/github/commit-activity/m/fungamer2-2/HumanlikeAI)
![GitHub last commit](https://img.shields.io/github/last-commit/fungamer2-2/HumanlikeAI)
![GitHub License](https://img.shields.io/github/license/fungamer2-2/HumanlikeAI)


Amorelia is a humanlike AI companion with thoughts, feelings, beliefs, and memories. Its goal is not simply to assist, but to truly form connections with users on a deeper level. 💖

Currently uses [Mistral AI](https://mistral.ai) models. To use this project, you'll need a Mistral AI API key, and store it under `MISTRAL_API_KEY` in a `.env` file.

## 💭 Thought system

Amorelia is designed to think before responding. These thoughts are treated as the AI's "inner monologue." This helps make it a bit more realistic, and think as if it truly had its own personality.

For complex or nuanced queries, Amorelia may decide to continue thinking so it can carefully consider the query before responding.

Periodically, Amorelia will reflect and gather insights to add to its memory, in order to gain a higher-level understanding of the user.

## 😊 Emotion system

The emotion system is based on the PAD (Pleasure-Arousal-Dominance) state model. Interactions with Amorelia will elicit emotions, which affect its mood.

Amorelia's mood is updated based on its emotions it experiences in the conversation. If no emotions have been invoked recently, its mood will gradually return to its baseline mood.

## 📝 Memory system

Amorelia also has a long-term memory system to recall relevant memories and insights from previous conversations. It includes two types of memory: short-term and long-term.

- Short-term memory: Memories that Amorelia has either experienced recently or recalled recently. This is always available in-context, but has a limited capacity, and any memories that get flushed out of short-term memory are sent to long-term memory.
- Long term memory: Stores the memories and experiences to be retrieved whenever they become relevant. Recalled memories return to short-term memory.

## ⚙️ How to use

1. Download this project
2. Make sure that [Python](https://python.org) is installed
3. Obtain a Mistral API key at <https://console.mistral.ai/>
4. Store the API key in a `.env` file in the project directory
5. Make sure to install the requirements: `pip install -r requirements.txt` 
6. Run `main.py`

If you find a bug or have a feature request, feel free to [open an issue](https://github.com/fungamer2-2/HumanlikeAI/issues/new/choose)!
