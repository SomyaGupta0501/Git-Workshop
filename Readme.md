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

## 2.2 Initializing a Repo

### Create a folder:
```bash
mkdir my-first-repo
cd my-first-repo
```

### Initialize Git:
```bash
git init
```

### Add a file:
```bash
echo "# My First Commit" >> README.md
```

### Stage & commit:
```bash
git add .
git commit -m "Initial commit"
```

---

## 2.3 Cloning and Pushing Changes

### Clone an existing repo:
```bash
git clone https://github.com/your-username/sample-repo.git
```

### Make a change:
```bash
echo "I'm learning Git!" >> notes.txt
git add .
git commit -m "Added notes"
```

### Push it:
```bash
git push origin main
```

---

## 2.4 Branching

### Create a new branch:
```bash
git checkout -b feature/cool-idea
```

### Make some changes and commit:
```bash
echo "Cool idea in progress" >> feature.txt
git add .
git commit -m "Added feature"
```

### Switch back to main:
```bash
git checkout main
```

---

## 2.5 Handling Merge Conflicts

### Simulate a conflict:

- On `main`, add a line to `conflict.txt` and commit.
- On `feature`, edit the same line and commit.

### Merge:
```bash
git checkout main
git merge feature/cool-idea
```

### Conflict appears!  
Open the file and manually resolve:
```text
<<<<<<< HEAD
this is from main
=======
this is from feature
>>>>>>> feature/cool-idea
```

### Replace with what you want and then:
```bash
git add conflict.txt
git commit -m "Resolved merge conflict"
```

---

## 3. 🎮 Game Engines 101

### 3.1 Why Use a Game Engine?

Without one, you’d have to:
- Write your own rendering code
- Handle physics from scratch
- Do cross-platform builds manually

**Game engines handle:**
- Graphics + Input
- Physics
- UI
- Asset handling

---

### 3.2 Popular Engines Compared

| Engine | Language | Strength | Weakness |
|--------|----------|----------|----------|
| Unity  | C#       | Lightweight, cross-platform, beginner friendly | UI bugs, heavy editor |
| Unreal | C++ / Blueprints | AAA visuals, cinematic quality | Heavy, complex for beginners |
| Godot  | GDScript / C# | Free & open-source, light builds | Small ecosystem |

---

### 3.3 Why We’ll Use Unity

- Simpler learning curve for beginners
- Widely used in both indie & mobile dev
- C# is easier to write and debug than Unreal’s C++
- Massive community + great asset store

> “Unreal is Thor’s hammer. Unity is dual pistols—lighter, faster, more agile.”
