# 01 – Agent Configuration

## 📘 Domain: AI Agents (35%)

Agent Configuration is a core component of the Salesforce Agentforce Specialist Certification exam.  
This section focuses on how agents are created, structured, and optimized for correct behavior and routing.

---

# 🎯 Objective

Understand how to properly configure an Agentforce agent in a Salesforce org, including:

- Agent creation
- Scope definition
- Topic configuration
- Routing logic awareness
- Testing practices
- Avoiding overconfiguration

---

# 🧠 What Is an Agent?

An Agent in Agentforce is a reasoning layer that:

1. Interprets user input
2. Matches it to a configured Topic
3. Applies Prompt instructions
4. Executes Actions (if defined)
5. Returns structured output

Agent configuration determines how accurately this process works.

---

# 🛠 Agent Creation Process

## Step 1 – Define the Use Case

Before creating an agent, clearly define:

- Who will use the agent?
- What specific tasks should it handle?
- What tasks should it NOT handle?
- Does it require CRM data access?
- Will it be deployed internally or externally?

Exam Tip:
Agents should be narrowly scoped and aligned to a specific business function.

---

## Step 2 – Create the Agent

Within Salesforce Setup:

- Navigate to Agentforce
- Create a new Agent
- Define the agent name clearly
- Add a precise description

Best Practice:
Avoid vague agent names like “General Assistant.”
Use task-specific naming such as:
“Internal Case Summary Agent”

Clear naming improves routing and maintainability.

---

## Step 3 – Configure Topics

Topics define what the agent is capable of handling.

Key considerations:

- Only add topics required for the use case
- Avoid overlapping topic descriptions
- Write clear and specific topic instructions
- Test routing across multiple input variations

Exam Risk:
Adding unnecessary topics increases misclassification.

Minimal configuration improves routing accuracy.

---

# ⚠️ Common Configuration Mistakes (Exam Relevant)

## 1. Overconfigured Agent

Adding all available standard topics without need.

Result:
- Routing confusion
- Incorrect responses
- Reduced performance

Correct Approach:
Only configure required topics.

---

## 2. Poor Topic Descriptions

Vague topic instructions can cause intent misrouting.

Example (Weak):
“Handles user questions.”

Example (Strong):
“Summarizes open service cases and extracts key next steps.”

---

## 3. Ignoring Scope Boundaries

Agents must have clear limitations.

Prompts should include:
- What the agent does
- What it does not do
- When to decline

---

# 🧪 Testing and Validation

Agent configuration must include structured testing.

Test for:

- Correct topic selection
- Edge case inputs
- Ambiguous user requests
- Out-of-scope questions

If routing fails:
- Refine topic descriptions
- Adjust prompt instructions
- Reduce topic overlap

Testing is heavily implied in exam scenarios.

---

# 🔐 Configuration vs Deployment

Agent configuration differs from deployment readiness.

Configuration includes:
- Agent creation
- Topic setup
- Prompt alignment

Deployment includes:
- Permission sets
- Connected channels
- Activation checklist review

Exam Reminder:
An agent can be configured correctly but not yet production-ready.

---

# 🧩 Architecture Flow

User Input  
→ Topic Match  
→ Prompt Instructions  
→ Optional Action Execution  
→ Structured Response  

Understanding this flow is critical for exam success.

---

# 📌 Key Takeaways

- Agents should be narrowly scoped.
- Only required topics should be added.
- Clear descriptions improve routing.
- Overconfiguration increases error risk.
- Testing is essential before deployment.

---

# 🎯 Exam Focus Summary

Within the AI Agents domain, expect questions on:

- Proper agent setup
- Topic alignment
- Routing logic
- Misconfiguration troubleshooting
- When to add or remove topics

Understanding configuration principles is foundational to the certification.

---

End of Section – Agent Configuration