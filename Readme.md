### Hands-on Workshop: Git Basics + Game Engine Intro  

---

## 📋 Table of Contents
1. [Intro: Why Version Control?](#1-intro-why-version-control)
2. [Git Basics (Hands-On)](#2-git-basics-hands-on)
   - [Git Installation](#21-git-installation)
   - [Initializing a Repo](#22-initializing-a-repo)
   - [Cloning and Pushing Changes](#23-cloning-and-pushing-changes)
   - [Branching](#24-branching)
   - [Merge Conflicts](#25-handling-merge-conflicts)
3. [Game Engines 101](#3-game-engines-101)
   - [Why Use a Game Engine](#31-why-use-a-game-engine)
   - [Popular Engines Compared](#32-popular-engines-compared)
   - [Why We’ll Use Unity](#33-why-well-use-unity)
4. [Post-Session Challenges](#4-post-session-challenges)

---

## 1. ✨ Intro: Why Version Control?

Imagine rewriting a whole game mechanic only to realize you broke something critical.  
**Git** gives you:
- A **time machine** (revert to any version)
- Safe team collaboration
- Experimentation (branches)

> Think of it like **save states in a video game**—but for code.

---

## 2. 🧰 Git Basics (Hands-On)

### 2.1 Git Installation

1. **Download Git**:  
   - Windows: [git-scm.com](https://git-scm.com/download/win)  
   - Linux/macOS: Use your package manager (e.g., `sudo apt install git`)

2. **Set it up:**
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
