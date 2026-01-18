---
title: Claude Code and my customizations
date: 2026-01-18 10:00:00 +0530
categories: [Technology, AI]
tags: [ai, development, claude]     # TAG names should always be lowercase
---

### 🚀 Finding My Tool

I started using Claude Code somewhere around October 2025. Since then, I've become a fan and never wanted to switch ships. I've stopped paying attention to what everyone else is shipping. I trust Anthropic a lot the way people trust their coffee brands 😅. I'd rather spend my time building workflows on top of this highly customizable super product than chasing the new shiny stuff. From a product perspective as well I love a hacky product.

Below I'm documenting the different ways I've customized Claude Code to get more out of it. I hope I write a Part 2 as well that'll mean that I did some cooler stuff.

### 🌳 Love Nature, Embrace Work-trees

I work across multiple git work-trees. Currently I'm at 3 and I don't think I'm smart enough to push that number up.

So I have different branches, different contexts, different tasks running on them but I want the same Claude behaviour everywhere since they are from the same repo. So I created a `CLAUDE.local.md` file in my main repository and symlinked it to all my worktrees.

### 📝 CLAUDE.md, Commands and Skills

These are kind of the building blocks of customisation that comes out of the box. Define your own commands and skills. I have skills defined for tasks that I do frequently like checking logs and metrics, writing a TDD.

### 🔧 Claude Know It All, Do It All

Not just code. You can ask Claude to edit Grafana boards, Confluence docs, and useful scripts directly with Claude and keep them in my repo filesystem. These go into personal folders that I add to `.git/info/exclude` so they don't mess with my org's repo but remain accessible to Claude across all work-trees by symlinks. Context about these different folders are also provided via `CLAUDE.local.md` file.

### 📍 Line Numbers in Implementation Plans

The credit for this goes to a coworker of mine. When Claude references code in a plan as `<filename>:<line_number>` instead of just the `<filename>`, it helps with preserving exhaustion of context window of the model.

### 💬 Interactive Planning Over Static Checklists

Again something borrowed from the smart people I work with. I switched from static bullet-point plans to interactive Q&A sessions. I think Claude itself does this more after some recent update.

### 🔔 Multitasking with Hooks

For a long time, I believed multitasking destroys quality work. I still believe that. But when you've got background AI agents working for you, you can actually achieve parallel execution without fragmenting your own focus. I have configured hooks that alert me when they have done their work and require my input.

### 🎯 The Philosophy

I love the line "Use tools that adapt to you and not the other way round". That's the essence of what I'm trying to do right from Obsidian to Claude Code.

The moment you stop treating AI assistants as fixed products and start treating them as customizable workflows, everything changes. You're no longer constrained by what the tool thinks you should do. You're orchestrating it to match how you already work.

---

*My workflow for writing this blog post was dump notes → get first draft in → refine. I should turn this into a command soon if I want to write posts frequently*
