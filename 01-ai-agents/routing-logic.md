# Routing Logic

## 📘 Domain: AI Agents (35%)

Routing logic determines how an Agentforce agent selects the correct Topic when a user submits a request.

Understanding routing behavior is critical for designing reliable agents and troubleshooting incorrect responses.

---

# 🎯 Objective

After studying this section, you should understand how:

- Agents interpret user input
- Topics are selected during classification
- Topic descriptions affect routing decisions
- Poor topic design causes misclassification
- Routing issues can be tested and corrected

---

# 🧠 How Routing Works

When a user interacts with an agent, the system follows a classification process.

Routing flow:

User Input  
→ Intent Interpretation  
→ Topic Matching  
→ Topic Instructions Applied  
→ Actions Executed  
→ Response Generated

The most important step in this flow is **Topic Matching**.

If the wrong topic is selected, the response may be incorrect.

---

# 📌 Topic Classification

Topic classification determines which topic best matches a user request.

The agent evaluates:

- Topic classification descriptions
- Topic scope definitions
- Prompt instructions
- Available actions

The topic that best matches the user intent is selected.

---

# 🧩 Example Routing Scenario

User input:

"Summarize the latest support cases."

Possible topics:

1. Case Summary Topic  
2. Case Update Topic  

Correct routing:

Case Summary Topic

Reason:

The user requested a summary, not a modification.

Well-written topic descriptions help the agent choose correctly.

---

# ⚠️ Common Routing Problems

## 1️⃣ Topic Overlap

Two topics attempt to handle similar requests.

Example:

Topic A: Handles case questions  
Topic B: Handles case summaries

Result:

The agent may choose either topic incorrectly.

Solution:

Define more precise classification descriptions.

---

## 2️⃣ Vague Topic Descriptions

Poor description example:

Handles user questions about cases.

Better description:

Summarizes open service cases and extracts key next steps.

Clear descriptions improve routing accuracy.

---

## 3️⃣ Too Many Topics

Excessive topics increase classification complexity.

More topics → greater chance of misrouting.

Best practice:

Use only necessary topics.

---

# 🧪 Testing Routing Behavior

Testing helps confirm whether routing works correctly.

Recommended test approach:

Test with different phrasing.

Example:

Input 1:  
"Summarize my support cases."

Input 2:  
"Give me an overview of my open cases."

Input 3:  
"What are the key issues in my support tickets?"

All should route to the same summary topic.

If they do not, the topic description may need adjustment.

---

# 🔧 Improving Routing Accuracy

To improve routing:

- Write clear classification descriptions
- Avoid overlapping topics
- Keep topic scope focused
- Test multiple user input variations
- Remove unnecessary topics

These steps reduce misclassification.

---

# 📊 Exam Focus

The Agentforce Specialist exam may test scenarios such as:

- An agent selecting the wrong topic
- Determining why routing failed
- Choosing the best way to improve topic classification
- Identifying topic overlap problems

Understanding routing logic is essential for answering these scenario-based questions.

---

# 🧠 Key Takeaways

- Routing determines which topic handles a user request.
- Topic classification descriptions guide routing decisions.
- Overlapping topics can cause misclassification.
- Clear scope definitions improve routing accuracy.
- Testing different input variations helps validate routing behavior.

Effective routing design leads to reliable and predictable agent responses.

---

End of Section – Routing Logic