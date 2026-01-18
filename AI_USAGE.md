# AI Attribution Policy

I used ChatGPT as a supporting tool for understanding concepts and resolving specific implementation doubts during development. The final code and outputs were verified by me.

- Tools Used : OpenAI ChatGPT

## Prompts Used:
- "How do we construct ρ = (L L†) / Tr(L L†) in PyTorch?"
- "How is quantum fidelity computed between two density matrices?"
- "Can you check if my training loop logic is correct and suggest fixes?"
- "How do I save and reload my best model weights during training?"
- "Can you check if the model.py file that i uploaded implements correctly?"
- "Can I check if my model has runned successfully and that I got output in Terminal?"
-"Can you help me debug why my validation fidelity is not improving?"
-"Give me a ready to copy text for the formula used for rho which had hermition matrix"

## Verification:
- Code Logic: After receiving explanations or sample snippets from ChatGPT,I manually checked the logic against standard definitions from quantum information theory. For example, I verified the Pauli basis construction in 'data.py' and the fidelity and trace distance formulas in 'utils.py' using formulas and online references(like using chatgpt for some information on quantum ).
- Model Constraints: I independently verified that constructing ρ as ρ = (L L†) / Tr(L L†) guarantees Hermiticity, positive semi-definiteness, and unit trace, and then confirmed that my implementation in 'model.py followed this exactly.
- Testing: I validated AI-assisted suggestions by running 'train.py' and monitoring training behavior, convergence, and evaluation metrics. Consistently high validation fidelity and reasonable trace distance values confirmed the correctness of the implementation.

