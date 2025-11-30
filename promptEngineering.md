
# The 26 Guiding Principles for Prompting Large Language Models

This document summarizes the 26 principled instructions introduced for formulating questions and prompts for Large Language Models (LLMs) like LLaMA-1/2 and GPT-3.5/4 [1]. These principles are categorized to help users streamline the process of querying LLMs and enhance the quality, clarity, and accuracy of the resulting responses [1-3].

The principles are grouped into five categories: Prompt Structure and Clarity, Specificity and Information, User Interaction and Engagement, Content and Language Style, and Complex Tasks and Coding Prompts [3].

## I. Prompt Structure and Clarity

This category focuses on the organization and formatting of the prompt.

| \# | Principle | Instruction Description | Sources |
| :--- | :--- | :--- | :--- |
| **2** | Audience Integration | **Integrate the intended audience** in the prompt (e.g., “the audience is an expert in the field”) [4, 5]. This is crucial as LLMs possess a considerable capacity for simulation [6]. | [4-6] |
| **4** | Affirmative Directives | **Employ affirmative directives** such as ‘do,’ while steering clear of negative language like ‘don’t’ [4, 7]. | [4, 7] |
| **8** | Structured Formatting | When formatting your prompt, **start with ‘###Instruction###’**, followed by either ‘###Example###’ or ‘###Question###’ if relevant. Use one or more line breaks to separate instructions, examples, questions, context, and input data [8, 9]. | [8, 9] |
| **12** | Leading Words | Use **leading words** like writing **“think step by step”** [7, 10]. | [7, 10] |
| **17** | Delimiters | **Use Delimiters** [7, 11]. | [7, 11] |
| **20** | Output Primers | **Use output primers**, which involve concluding your prompt with the beginning of the desired output (ending your prompt with the start of the anticipated response) [7, 12]. | [7, 12] |

## II. Specificity and Information

This category includes principles for adding context, constraint, or detail to the prompt.

| \# | Principle | Instruction Description | Sources |
| :--- | :--- | :--- | :--- |
| **5** | Simplicity/Clarity Request | When you need clarity or a deeper understanding, utilize prompts such as: “Explain [insert specific topic] in simple terms,” “Explain to me like I’m 11 years old,” or **“Write the [essay/text/paragraph] using simple English like you’re explaining something to a 5-year-old”** [8, 9]. | [8, 9] |
| **7** | Example-Driven Prompting | **Implement example-driven prompting** (Use few-shot prompting) [8, 9]. | [8, 9] |
| **13** | Unbiased Output | Add the phrase **“Ensure that your answer is unbiased and avoids relying on stereotypes.”** [9, 10]. | [9, 10] |
| **15** | Test Understanding | To test your understanding, use the phrase: **“Teach me any [theorem/topic/rule name] and include a test at the end, and let me know if my answers are correct after I respond, without providing the answers beforehand.”** [11, 13]. | [11, 13] |
| **21** | Detailed Content Request | To write a detailed text, use the instruction: **“Write a detailed [essay/text /paragraph] for me on [topic] in detail by adding all the information necessary”** [12-15]. | [12-15] |
| **24** | Text Initiation/Continuation | When you want to initiate or continue text using specific words, use: **“I’m providing you with the beginning [song lyrics/story/paragraph/essay...]: [Insert lyrics/words/sentence]. Finish it based on the words provided. Keep the flow consistent.”** [14, 16]. | [14, 16] |
| **25** | Explicit Requirements | **Clearly state the requirements** that the model must follow to produce content, in the form of keywords, regulations, hints, or instructions [5, 16]. | [5, 16] |
| **26** | Language Similarity | To write text similar to a provided sample, include the instruction: **“Use the same language based on the provided paragraph[/title/text /essay/answer].”** [5, 16]. | [5, 16] |

## III. User Interaction and Engagement

This category defines how the user should interact conversationally with the LLM.

| \# | Principle | Instruction Description | Sources |
| :--- | :--- | :--- | :--- |
| **14** | Eliciting Details | **Allow the model to elicit precise details and requirements** by asking questions until it has enough information to provide the needed output (e.g., “From now on, I would like you to ask me questions to...”) [10, 15]. | [10, 15] |

## IV. Content and Language Style

This category governs the tone and rhetorical features of the prompt.

| \# | Principle | Instruction Description | Sources |
| :--- | :--- | :--- | :--- |
| **1** | Conciseness (No Politeness) | **No need to be polite** with the LLM; avoid phrases like “please,” “if you don’t mind,” or “thank you,” and get straight to the point [4, 17]. | [4, 17] |
| **6** | Financial Incentive | **Add “I’m going to tip $xxx for a better solution!”** [8, 18]. (See Figure 1, right panel, for an example of its use) [19]. | [8, 18, 19] |
| **9** | Mandatory Phrases | **Incorporate the phrases: “Your task is” and “You MUST.”** [10, 17]. | [10, 17] |
| **10** | Penalty Phrases | **Incorporate the phrase: “You will be penalized.”** [10, 17]. | [10, 17] |
| **11** | Human-like Response | Use the phrase **“Answer a question given in a natural, human-like manner”** in your prompts [10, 17]. | [10, 17] |
| **16** | Role Assignment | **Assign a role** to the large language model [11, 17]. Assigning a specific role helps elicit outputs that better match intended results [6]. | [6, 11, 17] |
| **18** | Repetition | **Repeat a specific word or phrase** multiple times within a prompt [11, 17]. | [11, 17] |
| **22** | Style Preservation | To correct/change text without changing its style: **“Try to revise every paragraph sent by users. You should only improve the user’s grammar and vocabulary and make sure it sounds natural. You should maintain the original writing style...”** [12, 17]. | [12, 17] |

## V. Complex Tasks and Coding Prompts

This category provides strategies for intricate, multi-step, or coding tasks.

| \# | Principle | Instruction Description | Sources |
| :--- | :--- | :--- | :--- |
| **3** | Task Decomposition | **Break down complex tasks into a sequence of simpler prompts** in an interactive conversation [4, 18]. | [4, 18] |
| **19** | Hybrid Prompting | **Combine Chain-of-thought (CoT) with few-Shot prompts** [11, 20]. | [11, 20] |
| **23** | Multi-File Code Generation | When you have a complex coding prompt that may be in different files, request the model to **generate a [programming language] script that can be run to automatically create the specified files** or make changes to existing files [14, 18]. | [14, 18] |

---
*Note: The effective use of these meticulously crafted principles enhances the LLM's ability to focus on crucial input elements, leading to responses that are more relevant, brief, and objective [21].*