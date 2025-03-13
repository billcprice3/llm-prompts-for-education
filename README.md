# llm-prompts-for-education

I am an educator. This is a repository of prompts I have developed for use in curricula I have taught.

Students have used LLMs of their choice (such as ChatGPT, Gemini, Copilot, etc.) to run these prompts.

---

# General materials creation

- [Generate Textbook Unit](prompts/Generate_Textbook_Unit.md) - see also [Writing Textbook Project Synopsis](prompts/Writing_Textbook_Project_Synopsis.md)
- [Generate Lesson From Text](prompts/Generate_Lesson_From_Text.md)
- [Generate Vocabulary List](prompts/Generate_Vocabulary_List.md)
- [Generate Vocabulary Images](prompts/Generate_Vocabulary_Images.md)
- [Generate Vocabulary Texts/Sentences](prompts/Generate_Vocabulary_Sentences.md)
- [Generate Vocabulary Dictation](prompts/Generate_Vocabulary_Dictation.md)
  - [Example output](prompts/Generate_Vocabulary_Dictation_Example.md)
- [Summarize Scientific Journal Article](prompts/NotebookLM_Summarize_Article.md)
- [Generate Song Lyrics](prompts/Generate_Song_Lyrics.md)
- [Trying Claude 3.5 Sonnet's "Artifact" view for creating an OER](prompts/Claude_3.5_Sonnet_Draft_OER_Using_Artifact.md)

---

# Citing and licensing AI-assisted work

- [AI Attribution Scenarios](prompts/AI_Attribution_Scenarios.md)

---

# Securely assessing student work offline
- [Assessing real student reflections on a lecture](prompts/Assess_Real_Student_Reflections_On_A_Lecture.md)
- [Assessing real student argumentative essays](prompts/Assess_Real_Student_Argumentative_Essays.md)

---

# Prompts designed for specific curricula

## Technical Communication for Information Science

[Index Page for INFSCI 2205](prompts/INFSCI_2205_Index.md)

- [Writing coach](prompts/INFSCI_2205_Writing_Coach.md)
- [Library catalog search query suggestions](prompts/INFSCI_2205_Search_Query_Suggestions.md)
- [Introduction Hook Suggestions](prompts/INFSCI_2205_Introduction_Hook_Suggestions.md)
- [Make flashcards from an article](prompts/INFSCI_2205_Make_Flashcards_From_Article.md)
- [Paraphrase Assistant](prompts/INFSCI_2205_Paraphrase_Assistant.md)
- [Argumentative Essay Outline Feedback](prompts/INFSCI_2205_Argumentative_Essay_Outline_Feedback.md)
- [Argumentative Essay Draft Feedback](prompts/INFSCI_2205_Argumentative_Essay_Feedback.md)

## Writing 5

- [Essay Feedback Questions](<prompts/Writing_5_Essay_Feedback_Questions.md>)

---

# Recommended offline LLMs

I have had great success with these models on a 2023 model year MacBook Pro with the M2 Pro chipset, presented here from most recent to oldest model:

### Recent
- March 2025: [Gemma 3 12b](https://huggingface.co/lmstudio-community/gemma-3-12b-it-GGUF)

### Older
- Circa June 2024: [Qwen2-7B-Instruct-GGUF](https://huggingface.co/MaziyarPanahi/Qwen2-7B-Instruct-GGUF) run via LM Studio
- Circa May 2024: [Meta-Llama-3-8B-Instruct-GGUF](https://huggingface.co/lmstudio-community/Meta-Llama-3-8B-Instruct-GGUF) run via LM Studio
- Circa March 2024: [Nous-Hermes-2-Mistral-7B-DPO](https://huggingface.co/NousResearch/Nous-Hermes-2-Mistral-7B-DPO) run via GPT4All

---

# Presentations

## 2024

- 2024-03-28: [Let's Demystify AI and Take Initiative](presentations/2024/Let’s_Demystify_AI_and_Take_Initiative.md). Workshop, English Language Institute Curriculum Meeting.
- 2024-04-12: [Three Concepts for Generative AI in Language Education](presentations/2024/Three_Concepts_for_Generative_AI_in_Language_Education.md). Panel presentation, Technology in Language Teaching Forum.

---

# Additional Resources

## Prompt engineering and repositories

- [How to Write Better ChatGPT Prompts](https://www.xelplus.com/chatgpt-prompts-for-best-results/): Article and video by Leila Gharani with specific tips and examples for writing more effective prompts

- [LLM Prompts for Education](README.md): Bill Price's repository of prompts.

- [Fabric](https://github.com/danielmiessler/fabric/tree/main/patterns): A repository of prompts by Daniel Miessler. They are not specific to education, but provide excellent examples of what an engineered prompt can look like. See some of Miessler's examples below:

    - [Create Keynote](https://github.com/danielmiessler/fabric/blob/main/patterns/create_keynote/system.md) prompt that instructs the AI to create a slide-by-slide plan for a presentation

    - [Extract Wisdom](https://github.com/danielmiessler/fabric/blob/main/patterns/extract_wisdom/system.md) prompt that instructs the AI to "extract surprising, insightful, and interesting information from text content"

## Chat-Based Generative AI Tools (as of March 2024)

### Commercial (online)

- [ChatGPT](https://chat.openai.com/): A conversational AI developed by OpenAI, capable of generating human-like text responses. It's known for its wide range of applications, from answering questions to writing creative content.

- [Google Gemini](https://gemini.google.com): A conversational AI developed by Google, designed to provide information and perform tasks through natural language understanding.

- [Microsoft Copilot](https://copilot.microsoft.com/): Microsoft's conversational AI assistant that integrates with various Microsoft products to enhance productivity by automating tasks, generating content, and providing insights based on natural language prompts.

### Open-Source (offline)

- [GPT4All](https://gpt4all.io/): A free program for downloading and running open-source conversational AIs locally on your own computer. As of March 2024, I recommend using the model called Nous Hermes 2 Mistral DPO.

- [LM Studio](https://lmstudio.ai/): Similar to GPT4All, but considered to be less user-friendly and more advanced.

## Image-Based Generative AI Tools

- [DALL·E 3](https://openai.com/dall-e-3/): Powers the image creation of ChatGPT and Microsoft Copilot.

- [Midjourney](https://www.midjourney.com/)

- [Stable Diffusion](https://stability.ai/stable-image)
