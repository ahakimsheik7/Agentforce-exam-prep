# Topic Design

## 📘 Domain: AI Agents (35%)

Topic design is a core component of building reliable Agentforce agents.  
Topics determine what types of user requests an agent can recognize and handle.

Well-designed topics improve routing accuracy, reduce misclassification, and ensure the agent performs the correct tasks.

---

# 🎯 Objective

After studying this section, you should understand how to:

- Design effective topics for an Agentforce agent
- Define clear topic scope and responsibilities
- Write strong classification descriptions
- Avoid topic overlap
- Improve routing accuracy through better topic design

---

# 🧠 What is a Topic?

A **Topic** defines a specific capability of an agent.

Topics help the agent determine:

- Whether a request matches the topic
- What instructions should be applied
- Which actions should be executed

Topics act as the **intent classification layer** of the agent.

---

# 📌 Core Components of a Topic

Each topic contains several important configuration elements.

---

## 1️⃣ Classification Description

The classification description explains **what type of request the topic handles**.

This helps the agent decide when the topic should be used.

### Example

Weak description:

Handles case questions.

Strong description:

Summarizes customer support cases and highlights key issues and next steps.

Clear descriptions improve topic selection accuracy.

---

## 2️⃣ Scope

Scope defines **what the topic is allowed to do and what it should avoid doing**.

A good scope prevents the agent from performing unintended tasks.

### Example

Example scope:

The agent may summarize support cases but must not modify case records.

Clear scope boundaries reduce incorrect behavior.

---

## 3️⃣ Instructions

Instructions guide how the agent should respond when the topic is selected.

Instructions may define:

- Response style
- Output format
- Data usage rules
- Task boundaries

### Example instruction

Provide a short summary followed by recommended next steps.

Well-written instructions ensure consistent AI responses.

---

## 4️⃣ Associated Actions

Actions allow the topic to interact with Salesforce resources.

Examples include:

- Query Salesforce records
- Retrieve account information
- Trigger business workflows
- Access CRM data

Topics rely on actions to complete real tasks.

---

# ⚠️ Common Topic Design Mistakes

## Topic Overlap

Two topics attempt to handle similar user requests.

Example:

Topic A: Case Summary  
Topic B: Case Overview

This may cause the agent to select the wrong topic.

Solution:

Clearly separate topic responsibilities.

---

## Too Many Topics

Creating too many topics increases routing complexity.

Result:

Higher risk of misclassification.

Best practice:

Only create topics that support specific use cases.

---

## Vague Topic Instructions

Unclear instructions lead to inconsistent responses.

Always define:

- Expected output
- Data boundaries
- Task limitations

---

# 🧪 Testing Topic Design

After creating a topic, test it with different types of user input.

Example test inputs:

User input:

"Summarize my open cases."

User input:

"What are the key issues in my support tickets?"

User input:

"Give me an overview of my cases."

All of these should route to the **Case Summary Topic**.

If routing fails, improve the classification description.

---

# 🔧 Improving Topic Design

To improve topic performance:

- Write precise classification descriptions
- Avoid overlapping topics
- Define clear scope boundaries
- Keep topic responsibilities focused
- Test with multiple phrasing variations

These steps increase routing accuracy and reliability.

---

# 📊 Exam Focus

The Agentforce Specialist exam may test:

- When to create a new topic
- How to identify topic overlap
- How classification descriptions affect routing
- How instructions guide agent behavior

Understanding topic design is essential for configuring reliable agents.

---

# 🧠 Key Takeaways

- Topics define what the agent can handle.
- Clear classification descriptions improve routing.
- Scope limits prevent unintended tasks.
- Instructions guide agent responses.
- Actions allow topics to interact with Salesforce data.
- Good topic design reduces routing errors.

Well-designed topics are critical for building effective AI agents.

---

End of Section – Topic Design