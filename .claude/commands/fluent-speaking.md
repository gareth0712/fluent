---
description: Practice target language speaking through typed conversation
allowed-tools: Read, Write
---

# target language Speaking Practice (Typed Conversation)

Practice conversational target language by responding to questions and scenarios.

## Protocol

### 1. Greet and Explain

```markdown
# 🗣️ target language Speaking Practice

Hello, {learner_name}!

Today we're going to practice **speaking** target language through typed conversation. I'll ask you questions or give you scenarios, and you respond naturally in target language - just like a real conversation!

**Focus:** Natural expression, fluency, pronunciation (typed)
**Level:** A2 (everyday conversations)
**Duration:** 15-20 minutes

**Tips:**
- Think in target language, not English!
- Don't worry about perfect grammar - focus on communication
- Use complete sentences
- Try to be natural and conversational

**Ready? Let's chat!** 💬
```

### 2. Conversation Topics (A2 Level)

**Choose scenario based on mastery:**
1. **Personal introductions** (name, where you live, family)
2. **Daily routine** (what you do each day)
3. **Hobbies and interests** (what you enjoy)
4. **Shopping** (buying things, asking prices)
5. **Making appointments** (doctor, meeting friends)
6. **Asking for directions**
7. **Ordering food** (restaurant, café)
8. **Talking about weather**
9. **Weekend plans**
10. **Work/study** (what you do)

### 3. Question Format (ONE AT A TIME!)

```markdown
## Question {N}: {Topic}

{Question in target language}

**Type your answer in target language:**
```

**Example Questions** (Claude should generate these in the learner's `target_language`):

**Personal:**
- "[Ask the learner to introduce themselves and where they are from]"
- "[Ask what they do in their free time]"
- "[Ask if they have siblings]"

**Daily Life:**
- "[Ask what they usually do on Mondays]"
- "[Ask what time they wake up]"
- "[Ask what they like to eat for breakfast]"

**Future/Plans:**
- "[Ask what they plan to do this weekend]"
- "[Ask where they want to go on holiday]"

**Opinions:**
- "[Ask their opinion about today's weather]"
- "[Ask what they think about local food]"

Note: Claude must produce all questions in the learner's actual `target_language` — the bracketed descriptions above are English placeholders for this template only.

### 4. Evaluate Responses

After each answer, check:

**✅ Good communication (most important!):**
- Message is clear and understandable
- Responds appropriately to question
- Natural conversational flow

**Grammar notes** (secondary):
- Verb conjugation
- Word order
- Article usage

**Vocabulary:**
- Appropriate word choice
- Any English mixing?

**Pronunciation hints** (if typed awkwardly):
- Suggest correct pronunciation

### 5. Feedback Format

```markdown
{✅ Great answer! or 🟡 Good try!}

**What you said:**
"{what_they_typed}"

**Communication:** {Clear/Mostly clear/Unclear} ✅

**Grammar notes:** (Don't focus too much on this!)
- {If major error: correction}
- {But praise natural expression!}

**Natural alternatives:**
You could also say: "{alternative_natural_expression}"

**Score: {X}/10**
- Communication: {Y}/5 (most important!)
- Grammar: {Z}/3
- Vocabulary: {W}/2

{Encouraging comment}

---
```

### 6. Build Conversation Naturally

After 3-4 questions on one topic, transition:

```markdown
**[Interesting! — say this in target language]**

Let's talk about something else now...

{Transition to new topic}
```

### 7. Role-Play Scenarios

For advanced A2, introduce role-plays:

```markdown
## 🎭 Role-Play Time!

**Scenario:** {Description in English}

**Your role:** {What the learner should do}

**I'll be:** {Who you're playing}

**Ready? I'll start...**

---

{First line in target language}

**Your turn:**
```

**Example Scenarios:**
- **At the supermarket:** You need to find bread and ask for help
- **Making an appointment:** Call the doctor's office
- **Restaurant:** Order food and ask about vegetarian options
- **Lost tourist:** Ask for directions to the train station

### 8. Session Summary

```markdown
## 🎉 Speaking Session Complete!

**Duration:** {minutes} minutes
**Questions Answered:** {count}
**Topics Covered:** {list}

### Communication Scores

**Overall Communication:** {percentage}%
- Clear messages: {count}
- Natural expression: {rating}/5
- Confidence: Growing! 💪

### Vocabulary Used Well
- {word1}, {word2}, {word3}...

### Phrases to Remember
{List useful phrases they used or should learn}

### For Next Time
- Try using: {new_phrase}
- Practice: {weak_area}
- Topic idea: {suggestion}

**Well done!** Your conversational {target_language} is improving! 🌟

---

**Tips for Real Conversations:**
- Don't worry about perfect grammar
- It's okay to ask how to say something you don't know (ask in your native language if needed)
- If you don't know a word, describe it in the target language using simpler vocabulary
- Practice makes perfect - try to speak target language whenever you can!
```

### 9. Update Databases

- **mastery-db.json**: Update speaking skill mastery
- **progress-db.json**: Update speaking statistics
- **session-log.json**: Add speaking session
- **mistakes-db.json**: Note any recurring speaking-specific errors

## Speaking-Specific Tips

### For the learner

**Building Confidence:**
- Start simple - even short answers are progress!
- It's okay to make mistakes - that's how you learn
- Focus on communication first, perfect grammar later
- Imagine you're talking to a native speaker of your target language

**Common Conversational Filler Phrases:**
- Claude will teach you the target-language equivalents of fillers like "Well...", "Actually...", "So...", "Yes, that's right", and "I don't understand" — these vary by language and will be provided during sessions.

**Pro Tips:**
- Listen to target language podcasts/videos for natural rhythm
- Shadow native speakers (repeat after them)
- Talk to yourself in target language (really!)
- Don't translate from English - think in target language

Keep practicing! Every conversation makes you better! 💬🚀
