---
title: AI Coding Guidelines - Navigating Development in the LLM Era
date: 2025-06-14 18:30:00
categories: [Technology, Development, AI]
tags: [ai, development]     # TAG names should always be lowercase
---

### 🤖 How AI Changed Everything for Developers

I remember the day OpenAI released ChatGPT, and I was testing it. A chat window could generate code in minutes that used to take me hours to write going over loads of documentation, stack overflow threads, and other resources. 

That day divided the world into two groups: people who think AI is going to replace all software developers and people who think it changes nothing. Over the years we've come to realize that reality lies somewhere in the middle.

No matter which group you've supported, I'm pretty sure your workflow has changed, and you do use LLMs to code now. In my opinion someone would have to be stupid not to use them. But it would be better to not use it if you're going to use it stupidly.

### ⚠️ MCP: Your Double-Edged Sword

**The Golden Rule**: Treat MCP like a chainsaw - powerful but requiring extreme caution.

### 🔄 Commit Early, Commit Often

- **Commit after every meaningful change** ideally after each prompt that produces a diff
- **Use descriptive commit messages** that explain what the change contains
- **Create checkpoints** whenever you reach a stable, working state

Why this matters: Easy rollback when AI goes off track, better understanding of changes, helps identify AI hallucinations, and creates a clear audit trail.

### 📚 The Documentation Trap

AI loves to over-document everything. Keep it minimal. The best code is one that doesn't need any documentation.


### 🔍 The Scaling Challenge

As your project grows, AI becomes less reliable and makes more mistake. You'll have to get more hands on and break your vision into smaller changes then.

### 👻 Hunt for Ghost Files

AI creates "ghost code" - functions, classes, or files that exist but are never used identify and remove them continuously.

### 🧪 Regression Testing is Non-Negotiable

Accept that you won't have a bird's eye view of all changes. Your tests are now more important than ever.

### 💰 ROI Reality Check

Sometimes coding with AI is counterproductive. Recognize when to step back and do it the old way.

### 🏁 Conclusion

In the last few months I've seen multiple PRs that reiterate in me the importance of right and cautious way of using LLMs to write code.

It's like the brush is as good as the painter that holds it. Hope this article helps you. I would love to hear your techniques of wielding the brush better myself :) 
