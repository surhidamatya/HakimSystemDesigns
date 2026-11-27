# Chapter 3: A Framework for System Design Interviews

## Introduction
System design interviews simulate real-life problem solving. They test technical skills, but also collaboration, communication, and how you handle ambiguous requirements.

The chapter gives a **4-step framework** for approaching them.

---

## Step 1: Understand the Problem and Establish Design Scope

### Objectives
- Clarify requirements and assumptions.
- Don't jump into solutions too early.
- Show how you think by asking good questions.

### Approach
- **Ask Clarifying Questions:**
  - What are the most important features?
  - What scale does the system need to handle?
  - Are we building for web, mobile, or both?
  - Are there existing technologies or constraints?

- **Document Assumptions:** Write them on a whiteboard or paper so you can refer back.

### Example
**Problem:** Design a news feed system.  
**Questions:**
- Is it a mobile app, web app, or both?
- How many friends can a user have?
- Should the feed include images and videos?
- Is the feed sorted in reverse chronological order?

---

## Step 2: Propose High-Level Design and Get Buy-In

### Objectives
- Come up with a high-level architecture.
- Work with the interviewer to refine it.

### Approach
- **Draft a Blueprint:**
  - Draw boxes for the main components (e.g., clients, APIs, databases, caches, CDNs).
  - Treat the interviewer as a teammate.

- **Do Back-of-the-Envelope Calculations:**
  - Check that the design can handle the scale.

- **Walk Through Use Cases:** Find edge cases and test your assumptions.

### Example
For a news feed system, split the design into:
1. **Feed Publishing Flow:** Writing posts into databases and populating friends' feeds.
2. **Feed Retrieval Flow:** Aggregating friends' posts and displaying them in reverse chronological order.

---

## Step 3: Design Deep Dive

### Objectives
- Go deep on the important components.
- Show depth of understanding and that you can adapt.

### Approach
- **Prioritize Components:** Focus on the areas most relevant to the problem.
- **Discuss Bottlenecks:** Find likely performance issues and propose fixes.
- **Balance Detail:** Don't over-engineer or go down unnecessary rabbit holes.

### Example Topics
- **URL Shortener:** Hash function design.
- **Chat System:** Reducing latency, and handling online/offline status.
- **News Feed System:** Feed publishing and retrieval.

---

## Step 4: Wrap-Up

### Objectives
- Point out areas for improvement.
- Recap the design and discuss follow-ups.

### Approach
- **Identify Bottlenecks:** Discuss limitations and how to scale past them.
- **Summarize Design:** Recap the main design decisions and trade-offs.
- **Propose Enhancements:**
  - How to scale from 1 million to 10 million users.
  - Error handling for server failures or network issues.

---

## Best Practices

### Dos
- **Ask Questions:** Clear up ambiguity before solving.
- **Communicate:** Share your thought process with the interviewer.
- **Iterate with the Interviewer:** Treat them as a collaborator.
- **Show Flexibility:** Suggest alternatives and refine the design.
- **Focus on Critical Components:** Spend time on the parts that matter most.

### Don'ts
- **Avoid Premature Solutions:** Don't design before you understand the requirements.
- **Don't Go Silent:** Keep talking throughout.
- **Avoid Over-Engineering:** Aim for practical, scalable solutions.

---

## Time Management

### Suggested Time Allocation (for 45-Minute Interviews):
1. **Understand Problem and Scope:** 3–10 minutes
2. **High-Level Design and Buy-In:** 10–15 minutes
3. **Deep Dive:** 10–25 minutes
4. **Wrap-Up:** 3–5 minutes
