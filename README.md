# RAG-Based Support Ticket System

## Test Overview

This test evaluates your ability to reason about real-world system design, apply AI concepts like Retrieval-Augmented Generation (RAG), and demonstrate your software engineering and problem-solving skills.

---

## Context

Modern customer support systems often struggle with retrieving relevant past tickets or documents due to overreliance on keyword-based search mechanisms. This causes inefficiencies and poor user experience when resolving issues that require contextual understanding or pattern recognition.

---

## Scenario

Agents and users face delays and frustration when keyword-based systems return large volumes of irrelevant or loosely related results. The inability to understand nuanced queries—such as specific conditions, environments, or error variants—leads to decreased efficiency in issue resolution.

### Example:

**Agent:** Alex, a support engineer

**Query:** "Login error on Safari browser for enterprise users"

**Problem:**

* Current system returns generic login issues and ignores browser/user group context.

---

## Your Task

You are required to **design and implement a prototype** of a **RAG (Retrieval-Augmented Generation) system** that:

* Understands the semantic context of support queries
* Retrieves relevant historical tickets from a sample dataset
* Uses the retrieved content to generate contextual suggestions or summaries

### Deliverables

1. **Code Implementation**

   * Use Python with any framework (Streamlit, Flask, etc.)
   * Must include:

     * Text encoder (e.g., `intfloat/multilingual-e5-large-instruct` or `sentence-transformers`)
     * Explanation of model choices (embedding model, vector store, LLM)
     * Retrieval strategy (e.g., top-k, filters)
     * Vector search (e.g., FAISS, Milvus, or in-memory cosine similarity)
     * A few sample tickets embedded and searchable
     * Simple query interface (command-line works or anything that's easy)
     * Output showing relevant tickets and a generated answer

3. **Bonus (Optional)**

   * Integrate basic feedback mechanism for ticket relevance
   * Use pre-trained LLM to generate the final response

---

## Sample Support Tickets

### Ticket 1

* **Title:** Login failure on Safari for SSO users
* **Browser:** Safari 16.3
* **OS:** macOS Ventura
* **Customer Type:** Enterprise
* **Issue:** Redirect loop during SSO login
* **Resolution:** Clear cookies, update Safari settings to allow cross-site tracking.

### Ticket 2

* **Title:** Generic login issues
* **Browser:** All
* **Customer Type:** Mixed
* **Issue:** Password reset email not received
* **Resolution:** Whitelist support domain in email settings.

### Ticket 3

* **Title:** Login error specific to Chrome extensions
* **Browser:** Chrome
* **Customer Type:** SMB
* **Issue:** Conflict with password manager extension
* **Resolution:** Disable conflicting extension.

---

## Evaluation Criteria

* Correctness and relevance of retrieved tickets
* Bonus points for creativity and feedback handling

---

## Submission Instructions

* Submit a GitHub/GitLab repository
* Include a README with setup and run instructions

---

## Deadline

You have 48 hours to design a solution. Send us a github / bitbucket etc link to your repo, please keep the repo as public.

---

## Good Luck!

Feel free to use open-source tools and pre-trained models. The goal is to show your ability to think critically, build usable systems, and communicate your design effectively.
