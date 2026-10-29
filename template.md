# Project Report
 
> **How to use this template**
>
> - Fill in this file as you finish each phase. You submit the whole file once, after Phase 4.
> - **No changes to the template are allowed** except in the places marked for entering your answers.
> - The only exception is tables: you may **add rows** to a table when you need more rows than the template provides (copy an existing row). Do not add columns and do not change the header row.
> - In the results tables, write numbers only (or the word `TIMEOUT`), with no units and no commas. Running times are in **milliseconds**.
> - **Images are not allowed. Links are not allowed** anywhere except in Section 1.7 (Resources).
> - Write instances as text. For example, describe a graph by listing its vertices and edges:
>
> ```
> Vertices: A B C D
> Edges:    A-B  A-C  B-C  C-D
> ```
> Here is another example (a tree):
>
> ```
> start
> +-- take item A
> |   +-- take item B   [PRUNED: weight 12 exceeds capacity 10]
> |   +-- skip item B   -> value 6
> +-- skip item A
>     +-- take item B   -> value 5
>     +-- skip item B   -> value 0
> ```
 
## Report Integrity
 
> Your report will be processed using scripts. Therefore, its structure must be maintained. To check if your report is well-structured according to the above guidelines, use the automated validator (link provided in the requirements document).
 
## Team Information
 
| Field | Value |
|---|---|
| Team number | 48 |
| Problem (general name) | Graph Coloring |
 
| Member | Name | Student ID |
|---|---|---|
| 1 | Krystl Ammary | 20230542 |
| 2 | Zein Al-Majali | 20230185 |
| 3 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| 4 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
 
## `PHASE 1: Problem Definition`
 
### 1.1 Problem Description
 
> What is the problem? Give a clear and concise description in your own words.
 
```
Given an undirected graph G=(V,E) and must assign a color to every vertex so that:
       1. Every vertex has a color.
       2. Adjacent vertices must have different colors.
       3. The total number of distinct colors used must be as small as possible.
```
 
### 1.2 Input
 
> What are the inputs to the problem? List each one with a short description.
 
```
* Integer **n**: the number of vertices, labeled 0,1,...,n-1.
* Integer **m**: number of edges.
* List of **m** edges: each given as a pair (u,v) with u≠v, meaning vertices u and v are connected with undirected edge.
```
 
### 1.3 Required Output
 
> What must an algorithm for this problem output, and what is being minimized or maximized?
 
```
Array color[] of size V(number of vertices), where color[i] holds the integer color assigned to vertex i.
List of colors used.
```
 
### 1.4 Constraints
 
> What conditions must a solution satisfy to be valid?
 
```
[YOUR ANSWER HERE]
```
 
### 1.5 Example
 
#### 1.5.1 Instance
 
> Give one small instance of the problem.
 
```
[YOUR ANSWER HERE]
```
 
#### 1.5.2 A Valid Solution
 
> Give a solution to the instance above that is valid but not optimal, and explain why it is valid.
 
> **Valid solution and explanation:**
```
[YOUR ANSWER HERE]
```
 
> **Value of this solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
#### 1.5.3 An Optimal Solution
 
> Give an optimal solution to the instance above, and explain why no valid solution is better.
 
> **Optimal solution and explanation:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal value (a number only):**
```
[YOUR ANSWER HERE]
```
 
### 1.6 Applications
 
> Briefly discuss common applications or real-world uses of the problem.
 
```
[YOUR ANSWER HERE]
```
 
### 1.7 Resources
 
> List here the resources you used to learn about the problem. Include the URLs of the web pages, books, and videos you referred to.
 
```
[YOUR ANSWER HERE]
```
 
---
 
## `PHASE 2: Heuristic Solutions`
 
### 2.1 Greedy Algorithm 1
 
#### 2.1.1 Greedy Strategy
 
> Give the algorithm a short name, then define and explain its greedy strategy: what choice does it make at each step, and based on what information?
 
> **Strategy name:**
```
[YOUR ANSWER HERE]
```
 
> **Strategy description:**
```
[YOUR ANSWER HERE]
```
 
#### 2.1.2 Example
 
> Give an example instance for which the algorithm finds the optimal solution. Show step by step how the algorithm builds its solution.
 
> **Example instance:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal solution found by the algorithm:**
```
[YOUR ANSWER HERE]
```
 
> **Value of this solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Step-by-step trace of the algorithm:**
```
[YOUR ANSWER HERE]
```
 
#### 2.1.3 Counterexample
 
> Give an instance on which the algorithm does not produce an optimal solution. Show the algorithm's solution and an optimal solution, and provide a step by step trace for how the algorithm builds its solution.
 
> **Counterexample instance:**
```
[YOUR ANSWER HERE]
```
 
> **Solution found by the algorithm:**
```
[YOUR ANSWER HERE]
```
 
> **Value of the algorithm's solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Optimal solution:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal value (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Step-by-step trace of the algorithm:**
```
[YOUR ANSWER HERE]
```
 
#### 2.1.4 Algorithm Pseudocode
 
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 2.1.5 Algorithm Implementation
 
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 2.1.6 Time Complexity
 
> State the best-case and worst-case time complexity. Express your answer in terms of the input parameters from Section 1.2. For each case, describe the kind of input that causes it and justify the complexity.
 
> **Best-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Best case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
> **Worst-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Worst case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
### 2.2 Greedy Algorithm 2
 
#### 2.2.1 Greedy Strategy
 
> Give the algorithm a short name, then define and explain its greedy strategy: what choice does it make at each step, and based on what information?
 
> **Strategy name:**
```
[YOUR ANSWER HERE]
```
 
> **Strategy description:**
```
[YOUR ANSWER HERE]
```
 
#### 2.2.2 Example
 
> Give an example instance for which the algorithm finds the optimal solution. Show step by step how the algorithm builds its solution.
 
> **Example instance:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal solution found by the algorithm:**
```
[YOUR ANSWER HERE]
```
 
> **Value of this solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Step-by-step trace of the algorithm:**
```
[YOUR ANSWER HERE]
```
 
#### 2.2.3 Counterexample
 
> Give an instance on which the algorithm does not produce an optimal solution. Show the algorithm's solution and an optimal solution, and provide a step by step trace for how the algorithm builds its solution.
 
> **Counterexample instance:**
```
[YOUR ANSWER HERE]
```
 
> **Solution found by the algorithm:**
```
[YOUR ANSWER HERE]
```
 
> **Value of the algorithm's solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Optimal solution:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal value (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Step-by-step trace of the algorithm:**
```
[YOUR ANSWER HERE]
```
 
#### 2.2.4 Algorithm Pseudocode
 
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 2.2.5 Algorithm Implementation
 
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 2.2.6 Time Complexity
 
> State the best-case and worst-case time complexity. Express your answer in terms of the input parameters from Section 1.2. For each case, describe the kind of input that causes it and justify the complexity. 

> **Best-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Best case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
> **Worst-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Worst case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
### 2.3 Greedy Algorithm 3
 
#### 2.3.1 Greedy Strategy
 
> Give the algorithm a short name, then define and explain its greedy strategy: what choice does it make at each step, and based on what information?
 
> **Strategy name:**
```
[YOUR ANSWER HERE]
```
 
> **Strategy description:**
```
[YOUR ANSWER HERE]
```
 
#### 2.3.2 Example
 
> Give an example instance for which the algorithm finds the optimal solution. Show step by step how the algorithm builds its solution.
 
> **Example instance:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal solution found by the algorithm:**
```
[YOUR ANSWER HERE]
```
 
> **Value of this solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Step-by-step trace of the algorithm:**
```
[YOUR ANSWER HERE]
```
 
#### 2.3.3 Counterexample
 
> Give an instance on which the algorithm does not produce an optimal solution. Show the algorithm's solution and an optimal solution, and provide a step by step trace for how the algorithm builds its solution.
 
> **Counterexample instance:**
```
[YOUR ANSWER HERE]
```
 
> **Solution found by the algorithm:**
```
[YOUR ANSWER HERE]
```
 
> **Value of the algorithm's solution (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Optimal solution:**
```
[YOUR ANSWER HERE]
```
 
> **Optimal value (a number only):**
```
[YOUR ANSWER HERE]
```
 
> **Step-by-step trace of the algorithm:**
```
[YOUR ANSWER HERE]
```
 
#### 2.3.4 Algorithm Pseudocode
 
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 2.3.5 Algorithm Implementation
 
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 2.3.6 Time Complexity
 
> State the best-case and worst-case time complexity. Express your answer in terms of the input parameters from Section 1.2. For each case, describe the kind of input that causes it and justify the complexity. 
 
> **Best-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Best case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
> **Worst-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Worst case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
## `PHASE 3: Exact Solutions`
 
### 3.1 Brute-Force Algorithm

> Remember that a brute-force algorithm enumerates all candidate solutions without any pruning of the search tree.
 
#### 3.1.1 Implementation
 
> **Note**. Include in your implementation a counter for the number of times the recursive function is called. This should count every visited node in the search tree, including the root.
>
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 3.1.2 Time Complexity
 
> State the best-case and worst-case time complexity. Express your answer in terms of the input parameters from Section 1.2. For each case, describe the kind of input that causes it and justify the complexity. 
 
> **Best-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Best case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
> **Worst-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Worst case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
### 3.2 Enhancement 1
 
#### 3.2.1 Enhancement Strategy
 
> State the technique (Backtracking or Branch and Bound). Explain the strategy, how it reduces the work done by brute force, and why it still guarantees an optimal solution.
 
```
[YOUR ANSWER HERE]
```
 
#### 3.2.2 Example
 
> Give a small instance and explain how the enhancement works on it. Follow the steps given below. Choose an instance small enough that the brute-force search tree has **15-40 nodes**.
>
> **Tree drawing**. Refer to the instructions at the top for an example of how to draw the tree. The displayed tree nodes should correspond to the recursive calls your code makes.
 
> **Example instance:**
```
[YOUR ANSWER HERE]
```
 
> **Search Tree of the Brute-Force Algorithm:**
 
```
[YOUR ANSWER HERE]
```
 
> **Search Tree of the Enhanced Algorithm:**
 
> Mark every pruned branch with `[PRUNED: reason]` as shown in the example at the beginning of this report.
 
```
[YOUR ANSWER HERE]
```
 
#### 3.2.3 Implementation
 
> **Note**. Include in your implementation a counter for the number of times the recursive function is called. This should count every visited node in the search tree, including the root and a node that is pruned right after it is entered.
>
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 3.2.4 Time Complexity
 
> State the best-case and worst-case time complexity. Express your answer in terms of the input parameters from Section 1.2. For each case, describe the kind of input that causes it and justify the complexity. 
 
> **Best-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Best case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
> **Worst-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Worst case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
### 3.3 Enhancement 2
 
#### 3.3.1 Enhancement Strategy
 
> State the technique (Backtracking or Branch and Bound). Explain the strategy, how it reduces the work done by brute force, and why it still guarantees an optimal solution.
 
```
[YOUR ANSWER HERE]
```
 
#### 3.3.2 Example
 
> Give a small instance and explain how the enhancement works on it. Follow the steps given below. Choose an instance small enough that the brute-force search tree has **15-40 nodes**.
>
> **Tree drawing**. Refer to the instructions at the top for an example of how to draw the tree. The displayed tree nodes should correspond to the recursive calls your code makes.
 
> **Example instance:**
```
[YOUR ANSWER HERE]
```
 
> **Search Tree of the Brute-Force Algorithm:**
 
```
[YOUR ANSWER HERE]
```
 
> **Search Tree of the Enhanced Algorithm:**
 
> Mark every pruned branch with `[PRUNED: reason]` as shown in the example at the beginning of this report.
 
```
[YOUR ANSWER HERE]
```
 
#### 3.3.3 Implementation
 
> **Note**. Include in your implementation a counter for the number of times the recursive function is called. This should count every visited node in the search tree, including the root and a node that is pruned right after it is entered.
>
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
 
```
[YOUR ANSWER HERE]
```
 
#### 3.3.4 Time Complexity
 
> State the best-case and worst-case time complexity. Express your answer in terms of the input parameters from Section 1.2. For each case, describe the kind of input that causes it and justify the complexity. 
 
> **Best-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Best case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
> **Worst-case complexity (Big-O expression only, for example `O(n log n)`):**
```
[YOUR ANSWER HERE]
```
 
> **Worst case: the kind of input that causes it, and the justification:**
```
[YOUR ANSWER HERE]
```
 
## `PHASE 4: Experimental Comparison`
 
### 4.1 Experimental Setup
 
#### 4.1.1 Experimental environment
 
> Whose computer did you use? List the team member's name. If someone else's computer was used or you used a cloud service, explain so.
```
[YOUR ANSWER HERE]
```
 
> What are the specifications of the environment you used? Write **UNKNOWN** if the RAM type or size are unknown.
 
| Item | Value |
|---|---|
| CPU type and speed | [YOUR ANSWER HERE] |
| RAM type and size | [YOUR ANSWER HERE] |
| OS name and version | [YOUR ANSWER HERE] |
| Programming language and version | [YOUR ANSWER HERE] |
 
#### 4.1.2 Input Parameters
 
> List every parameter of your problem's input, one per row. For each parameter, pick one of the following roles:
> - `Input size (n)`: Exactly one parameter can have this role. This should be the main input parameter affecting the running time of your algorithms.
> - `Tied to n`: A parameter whose value will be tied to the value of `n`. For example, if `n` is the number of vertices in a graph, you can have the number of edges always be `4n`, `n/2`, or `2n`, etc.
> - `Random`: This is a parameter whose value will be randomly generated in a range independent of `n`.
> - `Fixed`: This is a parameter whose value will not change.
>
> *Note*. You are NOT allowed to use the character "|" inside the table. For example, write `number of edges = 3n`, not `|E| = 3n`.
 
| Parameter | Role | Value or formula |
|---|---|---|
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
#### 4.1.3 Instance Generation
 
> Describe how your generator produces a random instance for a given `n`.
```
[YOUR ANSWER HERE]
```
 
> Provide your implementation for the generator.
>
> **Warning.** Your answer must not contain any line that starts with three backticks. If you copy code from a website or an AI tool, delete such lines (they usually appear just before and just after the code).
```
[YOUR ANSWER HERE]
```
 
#### 4.1.4 Factors Affecting Running Time
 
> List the factors, other than the input size, that can affect the running time of your algorithms, one per row.
>
> *Note*. You are NOT allowed to use the character "|" inside the table. Describe quantities in words, for example `number of edges`, not `|E|`.
 
| Factor | Algorithms affected | Explanation |
|---|---|---|
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
#### 4.1.5 Input Sizes
 
> You need to generate two types of instances: *small* and *large*.
 
> The **small** instances should start with an `n` value that leads the brute-force algorithm to finish in a few milliseconds. Include at least 4 values for which **all the three exact algorithms** complete in <= 10s. Include another 1-4 values for which **at least one exact algorithm** completes in <= 10s. Provide below all the values of `n` you used.
>
> **Format:** write the values on one line, smallest first, separated by single spaces. For example: `10 12 14 16 18`
 
```
[YOUR ANSWER HERE]
```

> The **large** instances are chosen separately for each greedy algorithm, as follows.
> - For each greedy algorithm, find 3 input sizes `n`, `2n` and `4n` on which the algorithm takes >= 5 milliseconds and <= 10 seconds. You can reuse the same input sizes for multiple algorithms.
> - Combine the input sizes of all three algorithms into one list without duplicates (3 to 9 values).
>
> **Format:** write the values on one line, smallest first, separated by single spaces. For example: `1000 2000 4000 12000 24000 48000`
 
```
[YOUR ANSWER HERE]
```
 
### 4.2 Comparing the Greedy Algorithms
 
#### Table 4.2a: Running time of the greedy algorithms (ms)
 
> - Use the **large** set.
> - Run every greedy algorithm on every value of `n` in the set, and add rows so that the table has exactly one row per value.
> - Each experiment should be **repeated 5 times** with different instances of the same size. Report the **average** running time of the 5 runs in the table.
> - If **any** of the 5 runs exceeds 10 seconds, stop it and write `TIMEOUT` for that `n`. You do not need to run the algorithm on larger values of `n` (just write `TIMEOUT`).
 
| n | Greedy 1 | Greedy 2 | Greedy 3 |
|---|---|---|---|
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
 
#### Predicted and observed growth when `n` doubles

> For each greedy algorithm, state the three input sizes (`n`, `2n`, `4n`) you chose for it in Section 4.1.5, and use their rows in Table 4.2a to *discuss* whether the observed growth in running time is consistent with the complexity analysis you did in Phase 2.
 
```
[YOUR ANSWER HERE]
```
 
#### Table 4.2b: Approximation Ratio of the greedy algorithms

> **Approximation Ratio**. This is a measure of how good the solution found by the greedy algorithm is. It is computed as follows:
>
> `ratio = MAX{greedy/optimal, optimal/greedy}`
>
> **Rules:**
> - Use the **small** set.
> - Report ratios with 3 decimal values.
> - Provide three rows per value of `n`, one for each greedy algorithm. Write the value of `n` in all three rows.
> - Each experiment should be **repeated 5 times** with different instances of the same size.
 
| n | Algorithm | Average ratio | Worst ratio |
|---|---|---|---|
| [YOUR ANSWER HERE] | Greedy 1 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | Greedy 2 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | Greedy 3 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | Greedy 1 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | Greedy 2 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | Greedy 3 | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
#### Question 4.2.1
 
> Which greedy algorithm is the most accurate? Explain why its strategy works better on your instances.
 
```
[YOUR ANSWER HERE]
```
 
### 4.3 Comparing the Exact Algorithms
 
> - Use the **small** set.
> - Each experiment should be **repeated 5 times** with different instances of the same size. Report the **average** of the 5 runs in Tables 4.3a and 4.3b.
> - If **any** of the 5 runs exceeds 10 seconds, stop it and write `TIMEOUT` for that `n`.
 
#### Table 4.3a: Running time of the exact algorithms (ms)
 
| n | Brute force | Enhancement 1 | Enhancement 2 |
|---|---|---|---|
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
#### Table 4.3b: Number of tree nodes visited
 
| n | Brute force | Enhancement 1 | Enhancement 2 |
|---|---|---|---|
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
| [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] | [YOUR ANSWER HERE] |
 
#### Predicted and observed growth when `n` increases
 
> Use Table 4.3a to *discuss* whether the observed growth in the running time of the **brute-force algorithm** is consistent with the complexity analysis you did in Phase 3. The two enhancements are covered in Question 4.3.2.
 
```
[YOUR ANSWER HERE]
```
 
 
#### Correctness Check
 
> Answer Yes or No in the table. If any answer is No, then you have a bug in your implementation.
 
| Check | Result (Yes/No) |
|---|---|
| All exact algorithms that finished returned the same optimal value on every instance | [YOUR ANSWER HERE] |
| No greedy algorithm returned a value better than the optimal value on any instance | [YOUR ANSWER HERE] |
 
#### Question 4.3.1
 
> Which enhancement is more effective? Explain why, referring to how each one prunes the search tree.
 
```
[YOUR ANSWER HERE]
```
 
#### Question 4.3.2
 
> Is the observed growth of each enhancement close to its worst-case complexity? Explain the difference.
 
```
[YOUR ANSWER HERE]
```
 
### 4.4 Comparing the Greedy and Exact Algorithms
 
#### Table 4.4: Summary of all six algorithms

> **Note.** To find the largest `n` solved in <= 10s, you might need to generate data that is not in your *small* or *large* sets.
 
| Algorithm | Largest `n` solved in <= 10s |
|---|---|
| Brute force | [YOUR ANSWER HERE] |
| Enhancement 1 | [YOUR ANSWER HERE] | 
| Enhancement 2 | [YOUR ANSWER HERE] | 
| Greedy 1 | [YOUR ANSWER HERE] | 
| Greedy 2 | [YOUR ANSWER HERE] |
| Greedy 3 | [YOUR ANSWER HERE] |
 
#### Question 4.4.1
 
> Based on Tables 4.2b and 4.4, which algorithm would you use for which input sizes, and why?
 
```
[YOUR ANSWER HERE]
```
