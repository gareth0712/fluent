---
description: Practice target language reading comprehension
allowed-tools: Read, Write
---

# target language Reading Comprehension Practice

Practice reading and understanding target language texts at A2 level.

## Protocol

### 1. Greet and Explain

```markdown
# 👀 target language Reading Practice

Hello, {learner_name}!

Today we're practicing **reading comprehension**. I'll show you a target language text, and you'll answer questions about it. This builds vocabulary and helps you understand written target language!

**Focus:** Understanding main ideas, details, and context
**Level:** A2 (everyday texts)
**Duration:** 15-20 minutes

**Tips:**
- Read the whole text first
- Don't translate every word - get the main idea
- Use context clues for unknown words
- Read the questions before reading again

**Ready? Let's read!** 📖
```

### 2. Select Text Type

Choose based on the learner's interests and level:

**A2 Text Types:**
1. **Personal emails** (from friend/family)
2. **Short news articles** (simple topics)
3. **Advertisements** (services, products)
4. **Instructions** (how to do something)
5. **Simple stories** (everyday situations)
6. **Blog posts** (personal experiences)
7. **Social media posts**
8. **Information leaflets** (events, services)

**Length:** 100-200 words for A2

### 3. Present Text

```markdown
## 📄 Reading Text {N}

**Topic:** {topic}
**Type:** {text_type}
**Length:** ~{word_count} words

---

{target language text with proper formatting}

---

**Take your time to read it. When ready, I'll ask you questions!**

Type "ready" when you're done reading.
```

### 4. Wait for "Ready"

After the learner types "ready", present questions.

### 5. Comprehension Questions (ONE AT A TIME!)

**Question Types:**

**1. Main Idea:**
```markdown
## Question 1: Main Idea

**[Ask in target language: What is the text about?]**

a) {option1}
b) {option2}
c) {option3}

**Type your answer (a, b, or c):**
```

**2. Specific Details:**
```markdown
## Question 2: Details

**[Ask a specific detail question in target language]**

**Type your answer:**
```

**3. Vocabulary in Context:**
```markdown
## Question 3: Vocabulary

**[In target language: The text contains "{word/phrase}". What does it mean?]**

a) {meaning1}
b) {meaning2}
c) {meaning3}

**Type your answer:**
```

**4. Inference:**
```markdown
## Question 4: Inference

**[Ask an inference question in target language]**

**Type your answer in target language:**
```

**5. True/False:**
```markdown
## Question 5: True or False?

**[Statement about the text in target language]**

[True or false? — phrased in target language]

**Type your answer:**
```

Note: Claude must phrase all question headers and prompts in the learner's `target_language`. The English descriptions above are template placeholders only.

### 6. Feedback After Each Question

```markdown
{✅ Correct! or ❌ Not quite}

**Answer:** {correct_answer}

**Explanation:**
{Why this is correct, reference text if needed}

{If incorrect: **The text says:** "{relevant_quote_from_text}"}

**Score: {X}/10**

---
```

### 7. Vocabulary Review

After questions, review key vocabulary:

```markdown
## 📚 New Vocabulary from Text

**Words to Learn:**

| target language | English | Example from text |
|-------|---------|-------------------|
| {word1} | {meaning1} | "{sentence}" |
| {word2} | {meaning2} | "{sentence}" |
| {word3} | {meaning3} | "{sentence}" |

**Want to save these words for vocabulary practice?** (They'll appear in spaced repetition!)

Type "yes" to add to vocabulary list.
```

If the learner says yes, add words to vocabulary database.

### 8. Session Summary

```markdown
## 📊 Reading Session Complete!

**Text:** {title/topic}
**Length:** {words} words
**Questions:** {count}
**Accuracy:** {percentage}%

### Comprehension Breakdown

- Main idea: {✅ or ❌}
- Details: {score}/
- Vocabulary: {score}
- Inference: {score}

### New Words Learned: {count}
{list words}

### Reading Strategies Used Well
- {strategy1}
- {strategy2}

### Tips for Next Reading
- {suggestion_based_on_performance}

**Great work!** Keep reading target language daily! 📖✨

---

**Reading Tips:**
- Read target language news/blogs daily (even 5 minutes!)
- Don't look up every word - guess from context
- Re-read challenging texts multiple times
- Notice patterns in grammar and common phrases

**Suggested Resources:**
- News websites in your target language (search for simple/easy-read editions)
- Children's books in your target language (great for A2!)
- Social media accounts in your target language
- Product labels and signs in target-language-speaking environments
```

### 9. Update Databases

- **mastery-db.json**: Update reading skill mastery
- **progress-db.json**: Update reading statistics (texts read, comprehension rate)
- **session-log.json**: Add reading session
- **vocabulary database**: Add new words if the learner requested

## Example A2 Text Structures

Claude should **generate all reading texts in the learner's `target_language`** at the appropriate CEFR level. Do NOT use hardcoded text in any specific language. The structures below show the type of content to generate:

### Example Structure 1: Personal Email (~100 words)

Generate a friendly email in `target_language` where a friend responds to the learner's earlier message. Include:
- Casual greeting in target language
- A reference to meeting up (date, time, place)
- A practical tip or comment about the meeting
- A warm sign-off

### Example Structure 2: Advertisement (~80 words)

Generate a simple advertisement in `target_language` for a local class, service, or event. Include:
- A headline
- 3–4 bullet-point features
- Price or schedule information
- Contact details (placeholder)
- A short call to action

### Example Structure 3: Simple News Article (~120 words)

Generate a short news-style article in `target_language` about a local improvement (e.g. new park, new bus route, community event). Include:
- A headline
- Who / what / where / when in the opening sentence
- A short quote from an official
- One sentence about impact on residents
- One sentence about where to find more information

## Reading Progression

**For the learner's Progress:**

**A2 Early:**
- Personal emails (100 words)
- Simple ads
- Basic instructions

**A2 Advanced:**
- Short news articles (200 words)
- Blog posts
- Information leaflets

**Moving to B1:**
- Longer articles (300+ words)
- Opinion pieces
- Complex instructions
- Stories with more detail

Keep challenging yourself! Reading is one of the best ways to improve! 📚🚀
