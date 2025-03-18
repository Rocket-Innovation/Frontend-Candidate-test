# Frontend-Candidate-test
Shared test for candidates who apply to Rocket-innovation

## Find the most Costly path
Find the most Costly path from the Graph as follows:

![Figure 1-1](files/max-path.png)

This example will have resulted in the red path.
Please note that the path cannot be reversed. The path should either go up or down.
The answer will be the maximum total value of each node along the path. Which, in this example, is 237.

# Test case

- input = `[[59], [73, 41], [52, 40, 53], [26, 53, 6, 34]]` output = `237`
- input = <https://github.com/Rocket-Innovation/Shared-Candidate-test/blob/main/files/hard.json> output = `7273`


---

## **Interactive Node-Based Calculator**  
Create an interactive **node-based calculator** using **React** that allows users to dynamically connect nodes and perform calculations.  

<img src="https://github.com/user-attachments/assets/09274ac2-ff1a-4fff-898a-b477b4af2297" width="500" />

### **Requirements**  

1. **State Management**  
   - Use **Zustand** for managing application state efficiently.  

2. **Draggable & Connectable Nodes**  
   - Implement a **fluid UI** with **smooth drag-and-drop functionality**.  
   - Nodes should be **movable** within the workspace.  
   - Users must be able to **drag connections** from one node’s **output** to another node’s **input** to form a calculation chain.  

3. **Node Structure**  
   - Every node must have **at least one input and one output**.  
   - Users should be able to **connect multiple nodes** in a sequence to continue calculations.  

4. **Calculation Nodes**  
   - Implement **four types of calculation nodes**:  
     - **Addition (+)**  
     - **Subtraction (-)**  
     - **Multiplication (*)**  
     - **Division (/)**  
   - Instead of manually entering numbers, each node must **fetch values from an API**:  
     - Use **[Random Number API](https://www.randomnumberapi.com/)** to get values.  
     - Example API call: `https://www.randomnumberapi.com/api/v1.0/random?min=1&max=100&count=2`.  
   - Each node should **display the numbers fetched** and show the computed result.  

5. **Result Node**  
   - A special **Result Node** that collects and **displays the combined result** of all calculation nodes in the sequence.  
   - The result updates dynamically as nodes are connected or modified.  

6. **Styling & UI**  
   - Use **only CSS or styled-components** for styling.  
   - The UI should be **fluid, responsive, and visually clear**.  
   - Ensure **smooth transitions and animations** for node movements.  

7. **Performance Optimization**  
   - Ensure **efficient state updates** to prevent unnecessary re-renders.  
   - Cache API responses to reduce redundant network calls.

---

## **Test Cases**  

| Input | Expected Output |
|---|---|
| 4 Calculation Nodes (`+`, `-`, `*`, `/`) connected dynamically with numbers fetched from API | Correct computed results |
| Result Node combining all calculation nodes | Dynamic total result |

For additional test cases, fetch inputs dynamically from the API.  
