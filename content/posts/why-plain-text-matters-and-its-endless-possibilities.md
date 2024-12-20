---
title: "Why Plain Text Matters and Its Endless Possibilities"
date: 2024-12-20T15:57:02+01:00
draft: false
toc: true
images:
tags: 
  - noorg
  - rust
---

**Why Plain Text Matters: A Deep Dive into Endless Possibilities**p

Explore [Noorg](https://noorg.dev). The following is a deep dive into the endless possibilities of plain text and how it forms the foundation of tools like Noorg.

In the digital age, where note-taking tools are abundant and varied, plain text remains a cornerstone of simplicity, adaptability, and freedom. Why does plain text still matter, and how does it empower us to think beyond traditional paradigms? Let’s explore the endless possibilities of plain text and how it forms the foundation of innovative tools like Noorg.

---

**Plain Text: Simplicity Meets Power**

Plain text is not just a format—it’s a philosophy. It’s about embracing the fundamental nature of data as readable, writable, and universally accessible.

- **Universality:** Plain text can be opened, read, and edited by any text editor on any operating system. From `notepad.exe` to Vim, from Visual Studio Code to nano, the options are endless.
- **Longevity:** Proprietary formats may come and go, but plain text endures. A `.txt` file from the 1980s is still as accessible today as it was back then.
- **Portability:** Plain text doesn’t lock you into a specific tool or ecosystem. Your data remains yours.
- **Processability:** Plain text can be manipulated in infinite ways. Whether through scripts, command-line utilities, or full-fledged applications, plain text’s flexibility is unmatched.

---

**Plain Text: Beyond Display**

The beauty of plain text lies in its raw nature. It’s only text, but its simplicity opens doors to infinite interpretations and transformations:

- **Dynamic Processing:** Metadata, tags, and structure can be added with simple conventions, like Markdown or frontmatter. Tools then transform these annotations into actionable insights.
- **Programmable Interactions:** You can parse, analyze, and process plain text with any programming language. Imagine a plain text note becoming a task list, a calendar entry, or a project tracker—all through automation.
- **Unlimited Potential:** The constraints of plain text are only defined by how it’s displayed. Text can be visualized as tables, diagrams, timelines, or any other form that suits your needs.

---

**The Noorg Approach: Watchers Today, LSP Tomorrow**

[Noorg](https://noorg.dev) currently uses a background application and watcher pattern to process notes dynamically. While this approach is functional, it’s not the final form. Let’s break down why:

### Watchers: The Current State

Noorg’s watcher monitors changes in your notes directory. When a file is saved, observers written in Rust, Python, or Lua react to those changes. This pattern provides real-time processing and flexibility but comes with challenges:

- **Redundancy:** File watchers reimplement functionality already covered by other systems, like file system events or editor-specific plugins.
- **Integration Complexity:** Although Noorgs is cross editort, the setup process can be cumbersome, requiring manual configuration and installation.
- **Cross-Platform Challenges:** File watchers behave differently across operating systems, complicating implementation.

### The Future: A Language Server Protocol (LSP) Implementation

The Language Server Protocol (LSP) offers a standardized way to communicate between editors and background processes. By transitioning to an LSP-based architecture, Noorg can achieve:

- **Editor-Agnostic Integration:** Nearly every modern editor supports LSP. This means Noorg would work seamlessly with VSCode, Neovim, Emacs, Sublime Text, and more without separate plugins.
- **Centralized Functionality:** Observers and metadata processing can be handled by the LSP server, reducing redundancy and simplifying updates.
- **Rich Features:** With LSP’s capabilities, Noorg could provide contextual suggestions, dynamic views, and inline annotations directly within the editor.
- **Ease of Shipping:** Building and shipping for all editors becomes as simple as distributing the LSP server. Editors handle the integration, reducing Noorg’s maintenance burden.

### Maintaining Observer Power

An LSP-based Noorg would retain the full power of current observers. Scripts written in Rust, Python, or Lua could still process notes dynamically. The difference? Observers would hook into a unified, editor-friendly framework. For example:

- Observers could add metadata in real-time as you type.
- Dynamic views, like Kanban boards or tag-based summaries, could be rendered directly in the editor.
- Advanced features, like inline content restructuring or API integrations, would become simpler to implement.

---

**Plain Text + LSP: The Ultimate Combination**

By embracing the simplicity of plain text and the power of LSP, Noorg can evolve into a truly universal tool. Here’s what this combination unlocks:

- **Offline First, Forever:** Plain text ensures your data remains accessible, while LSP ensures rich functionality without cloud dependencies.
- **Infinite Extensibility:** Use any programming language to build integrations, observers, and automations.
- **Universal Editor Support:** Write in any editor, from Vim to VSCode, and let Noorg handle the heavy lifting.
- **Future-Proof:** Standardized protocols and open formats ensure longevity and compatibility.

---

## Embrace the Plain Text Revolution

Plain text is more than a format—it’s a gateway to creativity and control. With tools like Noorg, the potential of plain text is unlocked, empowering you to focus on what matters: your ideas.

As Noorg transitions to an LSP-based architecture, its flexibility and power will only grow, making it an indispensable tool for anyone who values simplicity, adaptability, and innovation. Join us in embracing plain text and building a future where note-taking is as limitless as your imagination.

---

_Explore Noorg on [GitHub](https://github.com/realjockel/noorg) and become part of the plain text revolution. Let’s redefine what note-taking can be._

