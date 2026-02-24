# Enable Agentforce & Review Default Topics and Actions

## 📘 Domain: AI Agents (35%)

This section focuses on enabling Agentforce in a Developer Edition org and reviewing default Topics and Actions provided by Salesforce.

This is foundational configuration knowledge tested in the AI Agents domain.

---

# 🎯 Learning Objectives

After completing this section, you should understand how to:

- Enable Agentforce in a Salesforce org
- Create an employee agent
- Grant user access via permission sets
- Review default Topics and associated Actions
- Understand how default assets impact configuration decisions

---

# 🧠 Key Concepts

## 1️⃣ Agentforce for Employees

Agentforce for employees allows internal users to:

- Query records
- Search internal libraries
- View benefits information
- Perform task-based workflows
- Deploy agents into Slack

This differs from customer-facing agents and focuses on internal productivity.

---

# 🛠 Step 1 – Enable Agentforce

Before creating agents, required org features must be enabled.

### Enable Einstein

Setup → Einstein Setup  
Ensure **Turn on Einstein** is enabled.

Exam Note:
Agentforce depends on Einstein being activated.

---

### Enable Agentforce (Default)

Setup → Salesforce Go  
Search for: **Agentforce (Default)**  
Click:
- Get Started  
- Turn On  
- Confirm  

This activates default Agentforce capabilities and assets.

---

# 🗂 Step 2 – Review Default Agent Assets

Navigate to:

Setup → Agentforce Assets

There are two main tabs:

- Topics  
- Actions  

Understanding these assets is critical before building a custom agent.

---

# 📌 Topics

Topics define:

- Classification description
- Scope
- Instructions
- Associated actions

Example:
MigrationDefaultTopic

Within a Topic, you can review:

- Topic Configuration
- This Topic’s Actions

Exam Insight:
You should always review a Topic’s associated Actions before using it.

---

# ⚙️ Actions

Actions are executable tasks tied to Topics.

They allow the agent to:

- Query Salesforce records
- Perform updates
- Retrieve data
- Execute business logic

Not all Topics require all default Actions.

Best Practice:
Customize Topics instead of using them as-is when unnecessary actions exist.

---

# 🔐 Step 3 – Grant Access

Agents require permission sets to allow users to interact with them.

Important:
Agent configuration ≠ user access.

Configuration:
- Building the agent

Access:
- Permission set assignment

Exam Trap:
An agent can exist but not be usable without proper permission assignment.

---

# 🧪 Step 4 – Testing

After enabling Agentforce and reviewing Topics:

- Create a simple employee agent
- Assign permission set
- Test with multiple task scenarios
- Observe topic routing behavior

Testing ensures:
- Correct topic classification
- Proper action execution
- No unnecessary topic activation

---

# ⚠️ Important Updates

## New Agent Builder Experience (Dreamforce 2025)

Salesforce announced an updated Agent Builder experience.
The process may differ slightly from current UI steps.

Exam Relevance:
Understand concepts rather than memorizing UI clicks.

---

## Data Cloud → Data 360 Rebrand

As of October 2025, Data Cloud is rebranded to Data 360.

Functionality remains unchanged.

Exam Note:
Both terms may appear in documentation.

---

# 📊 Why This Matters for the Exam

From the AI Agents domain (35%), expect questions about:

- Required org setup before building agents
- Relationship between Topics and Actions
- Default assets and customization
- Permission sets and user access
- Agent availability in Slack

Understanding default Topics and Actions helps avoid:

- Overconfiguration
- Misclassification
- Unnecessary action execution

---

# 🧠 Key Takeaways

- Einstein must be enabled before Agentforce.
- Agentforce (Default) activates baseline Topics and Actions.
- Always review default Topics before using them.
- Topics contain associated Actions.
- Permission sets control access.
- Customization is preferred over blind usage of defaults.

---

End of Section