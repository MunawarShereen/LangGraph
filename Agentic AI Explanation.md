# What is Agentic AI?

**Agentic AI** is a type of artificial intelligence that can take up a specific task or goal from a user and work towards completing it independently, with minimal human guidance. 

Unlike traditional AI that just answers a prompt and stops, an Agentic AI **plans**, **takes action**, **adapts to changes**, and **seeks help only when absolutely necessary**.

---

## Key Characteristics of Agentic AI

An Agentic AI system is defined by six core characteristics:

### 1. Autonomous
Autonomy refers to the AI system's ability to make decisions and take actions on its own. Instead of following strict, step-by-step human instructions, it is **proactive**. 

While this independence is powerful, unmonitored AI can sometimes exhibit biased behavior or make unwanted decisions. Therefore, autonomy is usually controlled using safeguards:
* **Permission Autonomy:** Giving the agent limited access to specific tools or actions.
* **Human-in-the-Loop (HITL):** Requiring the agent to ask for human permission before executing a critical action.
* **Override Control:** Allowing the user to stop, pause, or change the agent's behavior at any time.
* **Policies & Rules:** Setting strict boundaries (e.g., *"Never schedule an interview on a weekend"*).

### 2. Goal-Oriented
Autonomy needs a direction, and that direction is the **goal**. The user assigns a goal, and the agent figures out how to automate the steps to get there.
* Goals can be broad or have strict constraints.
* Goals are usually stored in the agent's "core memory" so it doesn't lose focus.
* Goals can be altered dynamically by the user as the task progresses.

### 3. Planning
Planning and execution happen in a continuous, iterative loop. The agent divides a massive goal into smaller, manageable sub-tasks. The planning process usually involves:
1.  Generating multiple candidate plans.
2.  Evaluating the pros and cons of each plan.
3.  Selecting and executing the best possible path.

### 4. Reasoning
Reasoning is the agent's ability to interpret information, draw logical conclusions, and make decisions. Reasoning is crucial during *both* the planning phase (deciding what to do) and the execution phase (figuring out how to do it).

### 5. Adaptability
Things don't always go according to plan. Adaptability is the agent's ability to modify its strategies or actions in response to unexpected conditions or failures.
* *Example:* If the agent tries to use a Calendar API to book a meeting and the API crashes, an adaptable agent won't just fail. Instead, it will adapt by sending an email to the user asking, *"When are you free?"*

### 6. Context Awareness
A good agent doesn't suffer from amnesia. Context awareness is the ability to understand, retain, and use relevant information from ongoing tasks, past interactions, user preferences, and environmental cues to make better decisions throughout a complex, multi-step process.

---

## Core Components of an Agentic AI System

To build an Agentic AI (like with LangGraph), you typically need five main building blocks:

1.  **Brain:** The core intelligence engine driving the agent (usually a powerful Large Language Model like GPT-4, Claude, or Gemini).
2.  **Orchestrator:** The internal manager that handles the step-by-step planning and execution loop.
3.  **Tools:** External services, functions, or APIs that the agent can use to interact with the real world (e.g., web search, calculators, email APIs, databases).
4.  **Memory:** Systems for state tracking, short-term memory (for the current conversation), and long-term memory (for recalling past interactions).
5.  **Supervisor:** An oversight module that handles human approval requests (HITL) and ensures the agent isn't violating any core policies.
