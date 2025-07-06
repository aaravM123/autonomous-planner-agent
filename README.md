
# Autonomous Task Planner Agent

This assistant uses OpenAI GPT-4o and LangGraph to:
- Accept a user-defined goal (e.g. "Learn LangGraph")
- Estimate how many days the goal should take based on complexity
- Break it down into subtasks using an LLM planner
- Automatically execute and review each subtask in a daily loop
- Persist memory between runs (like a real autonomous agent)

### Example Use Cases:
- Learn a new concept like "LangChain memory" over 5 days
- Break down coding goals like "Build a Python calculator"
- Create daily learning plans personalized by difficulty
- Resume progress automatically across Colab sessions

### Features:
- GPT-4o-powered task estimation and subtask generation
- Role-based loop (Planner → Executor → Reviewer)
- Memory file to persist daily progress (`agent_memory.json`)
- LangGraph conditional branching and recursion handling

### Files:
- `autonomous_planner.ipynb`: Colab notebook with full agent logic
- `requirements.txt`: Python dependencies
- `README.md`: This file

### Run Instructions:
```bash
pip install -r requirements.txt
# Then open and run the notebook in Google Colab
