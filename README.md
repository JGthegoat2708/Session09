# Session 09: Building Web Pages with AI

**Author:** Jainam Golechha (25BCON1659)
**Course:** Prompt Engineering for C and C++ (BCO610A)
**Institution:** JECRC University, Jaipur
**Module:** 3 (Creating Web Pages with AI)

## 📌 Overview
This repository contains my personal portfolio website, generated using AI and rigorously audited for structural integrity and absolute truthfulness. The core philosophy of this project is **"Zero Errors, Zero Lies"**[cite: 35]. While AI was used to generate the initial HTML structure and CSS boilerplate[cite: 45], every placeholder and hallucinated claim was manually replaced or deleted to ensure that every word on the page is a truthful claim about myself[cite: 43, 44]. 

## 🏗️ Architecture & Separation of Concerns
Following the principle that "looking right is not being right", the portfolio strictly separates structure and appearance.
*   **HTML (`index.html`):** Defines the semantic structure of the page (headings, sections, lists, and links). No inline style attributes are used[cite: 45]. If CSS is removed, the page remains completely understandable[cite: 41].
*   **CSS (`assets/style.css`):** Defines the appearance, spacing, typography, and interactive hover effects.

## 🎨 The Deliberate Colour System
Instead of hardcoding color hex values throughout the stylesheet, I implemented a deliberate three-color CSS scheme (Background, Main Text, and Accent) using `:root` variables[cite: 42, 46]. 
*   **One Source of Truth:** Editing the variables in the `:root` pseudo-class instantly changes the entire page's color scheme[cite: 42].
*   **Dark Mode (Homework Extension):** Utilizing these variables, I successfully inverted the entire theme to a Dark Mode palette without having to modify individual HTML elements or CSS classes[cite: 35, 42]. 
*   **Contrast:** Ensure readable contrast across all sections[cite: 42].

## ✅ Quality Validation (Zero Errors)
Few errors is not the target; **zero errors is the target**[cite: 40]. The HTML markup was validated using the W3C Nu HTML Checker[cite: 40].
*   **Current Status:** 0 Errors, 0 Warnings[cite: 40].

## 📱 Responsive Testing
The portfolio was tested using browser Developer Tools at a narrow width of roughly `375px`[cite: 38]. 
*   **Result:** The layout is fully responsive. Content is readable, clickable, and contained without any horizontal overflow or unreadable text[cite: 38].

## 🔍 Content Audit & Peer Review
Generated does not mean ready[cite: 44]. I conducted a thorough content audit (`AUDIT-page.md`) to verify every AI-generated claim[cite: 39]. 

| Section Analyzed | Truthful? | Action Taken / Evidence |
| :--- | :--- | :--- |
| **About Section** | Yes | Replaced AI generic text with my actual B.Tech CSE details at JECRC University. |
| **Skills List** | Yes | Deleted hallucinated advanced frameworks; inserted truthful skills (Python, C++, HTML/CSS, Testing)[cite: 46]. |
| **Projects** | Yes | Replaced fake blog links with my verified Session 07 and Session 08 GitHub repository URLs[cite: 46]. |
| **Added Sections (HW)** | Yes | Added truthful `Experience` and `Education` sections to expand the portfolio[cite: 35]. |

During peer review, my partner clicked every link, verified the narrow-width rendering, ran the validator, and successfully challenged my listed skills[cite: 37]. 

### 🤔 Reflection on AI Hallucinations
When the AI generated my initial profile, it confidently invented projects (e.g., "How AI is Transforming Education Blog") and skills I did not possess. This exercise demonstrated that while AI is incredibly fast at scaffolding layout and writing CSS variables, it fundamentally lacks context about my real-world identity. A polished page can still be completely wrong. Inspecting before praising and enforcing strict content audits is essential before deploying any AI-generated code to a public space[cite: 34, 44].
