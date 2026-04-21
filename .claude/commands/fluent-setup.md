---
description: Interactive onboarding - Set up your personalized language learning profile
allowed-tools: Read, Write
---

# Language Learning Setup

Welcome! Let's set up your personalized language learning system.

## Step-by-Step Onboarding

Important: Use all questions with a AskUserQuestion, grab all questions needed, and create AskUserQuestion blocks for all questions.

### Step 1: Welcome Message

```markdown
# 🌍 Welcome to Your Personal Language Learning System!

This AI-powered system will help you learn any language through:
- 📊 Systematic progress tracking
- 🧠 Spaced repetition (scientifically proven)
- 🎮 Gamification (streaks, achievements)
- 📈 Adaptive difficulty
- 🎯 Personalized to YOUR goals

**Let's get you set up!** (This takes ~5 minutes)

Press Enter to continue...
```

### Step 2: Collect Basic Information

**Ask ONE question at a time:**

**Question 1: Name**
```markdown
## Question 1: What's your name?

(We'll use this to personalize your experience)

**Type your name:**
```

Wait for answer, then store in variable.

**Question 2: Target Language**
```markdown
## Question 2: What language do you want to learn?

Examples: Spanish, French, German, Italian, Japanese, Korean, Arabic, Dutch, etc.

**Type the language:**
```

**Question 3: Native Language**
```markdown
## Question 3: What's your native language?

(This helps us provide better translations and explanations)

**Type your native language:**
```

**Question 4: Other Languages**
```markdown
## Question 4: Do you speak any other languages?

(Optional - this can help us make connections between languages)

**Type languages separated by commas, or "none":**

Example: English, Spanish
```

### Step 3: Assess Current Level

```markdown
## Question 5: What's your current level in {target_language}?

Choose one:
- **A1** - Complete beginner (little to no knowledge)
- **A2** - Elementary (basic phrases, simple conversations)
- **B1** - Intermediate (can handle most situations)
- **B2** - Upper intermediate (comfortable in most contexts)
- **C1** - Advanced (fluent, few errors)
- **C2** - Mastery (near-native level)
- **Not sure** - I'll help you find out!

**Type your level (A1, A2, B1, B2, C1, C2, or "not sure"):**
```

If they choose "not sure", offer quick assessment:

```markdown
### Quick Level Assessment

I'll ask you 5 simple questions to determine your level.

**Ready?** Type "yes" to start the assessment.
```

**Assessment questions** (if chosen):
1. Basic vocabulary recognition (A1 level)
2. Simple sentence construction (A2 level)
3. Past tense usage (B1 level)
4. Complex sentence with subordinate clauses (B2 level)
5. Idiomatic expression or nuance (C1 level)

Score their answers and determine level automatically.

### Step 4: Set Goals

**Question 6: Target Level**
```markdown
## Question 6: What level do you want to reach?

Current level: {current_level}

Target level:
- **A2** - Elementary
- **B1** - Intermediate
- **B2** - Upper intermediate
- **C1** - Advanced
- **C2** - Mastery

**Type your target level:**
```

**Question 7: Timeline**
```markdown
## Question 7: When do you want to reach {target_level}?

This helps us create a realistic study plan.

Choose one:
- **3 months** - Intensive (requires ~60 min/day)
- **6 months** - Fast track (requires ~30 min/day)
- **12 months** - Steady pace (requires ~15 min/day)
- **2+ years** - Relaxed (requires ~10 min/day)
- **Custom** - I'll specify my own timeline

**Type your choice:**
```

**Question 8: Daily Study Time**
```markdown
## Question 8: How much time can you dedicate daily?

Be realistic - consistency matters more than duration!

Examples:
- 10 minutes (maintenance mode)
- 15 minutes (steady progress)
- 30 minutes (recommended)
- 60 minutes (intensive)
- Custom (specify minutes)

**Type minutes per day:**
```

**Question 9: Learning Goal**
```markdown
## Question 9: Why are you learning {target_language}?

This helps us personalize content to your needs.

Examples:
- Travel
- Work/business
- Exams (specify: DELE, DELF, TestDaF, etc.)
- Living in {target_language} country
- Academic study
- Family/relationships
- Personal interest
- Other

**Type your main goal:**
```

### Step 5: Preferences

**Question 10: Learning Style**
```markdown
## Question 10: How do you prefer to learn?

Choose your preferred style:
- **Conversational** - Focus on speaking and listening
- **Academic** - Grammar rules and structured learning
- **Immersive** - Jump in, learn by doing
- **Balanced** - Mix of all approaches (recommended)

**Type your preference:**
```

**Question 11: Gamification**
```markdown
## Question 11: Do you want gamification features?

Gamification includes:
- 🔥 Daily streaks
- 🏆 Achievement unlocking
- 📊 Progress charts
- ⭐ Skill levels (0-5 stars)
- 🎯 Milestone celebrations

**Type "yes" or "no":**
```

### Step 6: Generate Profile & Plan

After collecting all information:

```markdown
## 🎉 Setup Complete!

**Your Learning Profile:**
- 👤 Name: {name}
- 🌍 Learning: {target_language}
- 📚 Native: {native_language}
- 📊 Current Level: {current_level}
- 🎯 Target Level: {target_level}
- 📅 Timeline: {timeline}
- ⏱️ Daily Time: {daily_minutes} minutes
- 💡 Goal: {learning_goal}

**Generating your personalized learning plan...**
```

Calculate and show:

```markdown
## 📋 Your Personalized Learning Plan

### Timeline to {target_level}

**Estimated time:** {calculated_months} months
**Daily practice:** {daily_minutes} minutes
**Total study hours needed:** ~{total_hours} hours

### Recommended Weekly Schedule

**Daily (Every day):**
- 🔄 `/fluent-review` - Spaced repetition ({X} min)
- 📚 `/fluent-vocab` - New vocabulary ({Y} min)

**Alternating Days:**
- 📝 `/fluent-writing` - Writing practice (Mon/Wed/Fri)
- 🗣️ `/fluent-speaking` - Conversation (Tue/Thu/Sat)
- 📖 `/fluent-reading` - Reading comprehension (Sun)

**Weekly:**
- 📊 `/fluent-progress` - Check your stats (5 min)

### Key Milestones

**Month 1:** {milestone_1}
**Month 3:** {milestone_2}
**Month 6:** {milestone_3}
**Target date ({timeline}):** Reach {target_level}!

### Next Steps

1. **Start now:** Type `/fluent-learn` to begin your first lesson
2. **Daily habit:** Start with `/fluent-review` each day
3. **Track progress:** Check `/fluent-progress` weekly
4. **Stay consistent:** Even 10 minutes daily beats 2 hours weekly!

**Your journey to {target_language} fluency starts now!** 🚀

Type `/fluent-learn` to start practicing!
```

Ask any other questions needed, based on the information we need to fill in `data-examples/learner-profile-template.json`, then move this file to `data/learner-profile.json`.

### Step 7: Save Profile

Create/update `data/learner-profile.json` based on the `data-examples/learner-profile-template.json` (or `data/learner-profile.json` if already exist) :


Also initialize other database files if they don't exist (you can find templates in `data-examples/`):
- `progress-db.json`
- `mistakes-db.json`
- `mastery-db.json`
- `spaced-repetition.json`
- `session-log.json`

### Step 8: Optional - First Lesson

```markdown
## 🎓 Want to start your first lesson now?

I can guide you through a quick introductory session (5-10 minutes) to:
- Learn your first 10 words
- Practice basic phrases
- Get familiar with the system

**Type "yes" to start now, or "later" to begin on your own time:**
```

If yes, launch `/learn` with beginner-friendly content.

---

## Profile Updates

If user runs `/fluent-setup` again with existing profile:

```markdown
# 👋 Welcome back, {name}!

I see you already have a learning profile.

What would you like to do?

1. **Update profile** - Change your goals, timeline, or preferences
2. **View current plan** - See your learning schedule
3. **Reset progress** - Start fresh (⚠️ this will erase your progress!)
4. **Cancel** - Keep everything as is

**Type 1, 2, 3, or 4:**
```

---

## Tips for Accurate Setup

**For the user:**

✅ **Be honest about your level** - We'll adjust as you progress
✅ **Set realistic time goals** - 15 min daily > 2 hours weekly
✅ **Choose specific learning goal** - Helps us personalize content
✅ **Pick a target date** - Creates accountability

**The system will:**
- Adapt to your actual performance over time
- Adjust difficulty automatically
- Update your plan as you progress
- Celebrate milestones along the way

---

## Formula for Calculations

**Months to target level:**
```
Level gaps:
A1 → A2: ~100 hours
A2 → B1: ~150 hours
B1 → B2: ~200 hours
B2 → C1: ~300 hours
C1 → C2: ~400 hours

Months = Total hours needed ÷ (Daily minutes ÷ 60) ÷ 30 days
```

**Adjust based on:**
- Learning style efficiency
- Native language similarity to target
- Number of other languages known (boost: +10% speed)

---

Ready to help someone start their language learning journey! 🌍✨
