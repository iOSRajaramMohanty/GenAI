# 📚 Prompt Engineering Interview Guide (Complete - 40+ Q&A with Examples)

---

## 🧠 Overview
Prompt engineering is designing inputs to guide LLMs for accurate outputs.

👉 Real-world idea: Like giving clear instructions to a junior engineer.

---

# 🔹 Basic Questions

### 1. What is a prompt?
Input given to an LLM.

**Example:**  
"Explain APIs in simple terms"

---

### 2. What is prompt engineering?
Designing prompts for better outputs.

**Example:**  
Bad: "Explain error"  
Good: "Explain this error for a beginner in simple words"

---

### 3. Why is it important?
- Controls output  
- Reduces hallucination  
- Improves accuracy  

---

### 4. Types of prompting
- Zero-shot  
- Few-shot  
- Instruction  

---

### 5. What is zero-shot?
No examples.

**Example:**  
"Translate English to French"

---

### 6. What is few-shot?
Provide examples.

**Example:**  
Dog → Animal  
Car → Vehicle  
Apple → ?

---

### 7. What is context?
Extra data given.

**Example:**  
Passing product manual before asking question

---

### 8. What is system prompt?
Defines behavior.

**Example:**  
"You are a helpful assistant"

---

### 9. What is user prompt?
Actual question.

---

### 10. What is hallucination?
Incorrect generated info.

---

# 🔹 Intermediate

### 11. What makes a good prompt?
- Clear  
- Specific  
- Structured  

---

### 12. Prompt structure
Instruction + Context + Question + Output

---

### 13. Role-based prompting
"You are a doctor"

---

### 14. Chain-of-thought
"Explain step by step"

---

### 15. Output formatting
"Return JSON"

---

### 16. Temperature?
Controls randomness.

---

### 17. Max tokens?
Response length limit.

---

### 18. Stop sequence?
Where output stops.

---

### 19. Prompt injection?
Malicious prompt manipulation.

---

### 20. Why delimiters?
Separate sections clearly.

---

# 🔹 Advanced

### 21. Reduce hallucination?
"Answer only from context"

---

### 22. Prompt chaining?
Output → next prompt

**Example:**  
Summarize → Explain → Email

---

### 23. Dynamic prompts?
Change based on user

---

### 24. Template prompts?
Reusable prompts

---

### 25. Few-shot vs fine-tuning?
Examples vs training model

---

### 26. Guardrails?
Rules for output

---

### 27. Long context handling?
Chunk + retrieve

---

### 28. Prompt optimization?
Improve prompts iteratively

---

### 29. Structured prompting?
Force JSON/table

---

### 30. Evaluation?
Test accuracy

---

# 🔹 Scenario-Based

### 31. Wrong answers?
Improve context

---

### 32. Not structured?
Add format instruction

---

### 33. Hallucination?
Add constraint

---

### 34. Too long?
"Keep answer short"

---

### 35. Ignoring instructions?
Add examples

---

# 🔹 Real-World Examples

### 36. Customer Support Bot
Prompt:
"You are support agent. Answer only from FAQ."

---

### 37. Code Assistant
"You are senior developer. Fix this bug"

---

### 38. Sales Assistant
"Summarize sales data in 3 insights"

---

### 39. Healthcare Assistant
"Explain symptoms in simple terms"

---

### 40. RAG System Prompt
"Answer only from provided context. If not found say 'I don't know'"

---

# 🔹 Coding Examples

### 41. Basic
prompt = "Explain RAG"

---

### 42. Context-based
prompt = f"Context: {context}\nQuestion: {query}"

---

### 43. JSON output
prompt = "Return JSON"

---

### 44. Constraint
prompt = "Answer only from context"

---

# 🏁 Summary
Better prompts = Better AI outputs
