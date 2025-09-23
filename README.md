# Recursion
# Experiment-15: Recursion in C++

##  Aim  
To study and implement recursion in C++ through four different programs:  
1. Factorial of a number  
2. Reverse digits of a number  
3. Reverse a string  
4. Sum of natural numbers  

---

##  Objectives
- Understand the principle of recursion and its working mechanism.  
- Learn how problems can be broken down into smaller subproblems.  
- Differentiate recursion from iteration.  

---

##  Theory

### What is Recursion?
Recursion is a programming technique in which a function solves a problem by **calling itself**.  
- Complex problems are broken into smaller subproblems of the same type.  
- This continues until reaching a **base case**, where the problem is solved directly.  

### Essential Parts of Recursion
- **Base Case (Termination Condition):** Prevents infinite calling and stops recursion.  
- **Recursive Case:** Defines how the problem is reduced into a smaller subproblem.  

### Working of Recursion
- Each recursive call is stored on the **function call stack**.  
- Once the base case is reached, the stored calls resolve in reverse order (stack unwinding).  

### Types of Recursion
- **Direct Recursion** → Function calls itself directly.  
- **Indirect Recursion** → Function A calls B, and B calls A.  
- **Tail Recursion** → Recursive call is the last operation.  
- **Head Recursion** → Recursive call is made before other operations.  

### Advantages
- Elegant and clean solutions to complex problems.  
- Naturally fits problems like factorial, Fibonacci, reversal, and tree traversal.  
- Makes code closer to mathematical definitions.  

### Disadvantages
- Uses more memory due to the call stack.  
- May be slower than iteration.  
- Risk of stack overflow if base case is missing.  

---

##  Comparison Table

| Program            | Base Case Condition   | Recursive Formula                   | Example Input | Example Output | Concept Focus            |
|--------------------|-----------------------|--------------------------------------|---------------|----------------|--------------------------|
| Factorial          | n ≤ 1 → 1            | n × factorial(n-1)                   | 5             | 120            | Multiplication recursion |
| Reverse Digits     | n = 0 → stop         | print(n % 10), reverse(n / 10)       | 123           | 321            | Number reversal          |
| Reverse String     | End of string → stop | reverse(str+1), print(str)           | HELLO         | OLLEH          | String reversal          |
| Sum of Numbers     | n ≤ 1 → 1            | n + sum(n-1)                         | 5             | 15             | Addition recursion       |

---

##  Algorithms

### Factorial of a Number
1. Start.  
2. Input number `n`.  
3. If `n <= 1` → return 1 (base case).  
4. Else → return `n * factorial(n-1)` (recursive case).  
5. Display factorial.  

---

### Reverse Digits of a Number
1. Start.  
2. Input number `n`.  
3. If `n == 0` → return (base case).  
4. Else → print `n % 10`, call `reverseNumber(n / 10)`.  
5. Stop.  

---

### Reverse a String
1. Start.  
2. Input string `str`.  
3. If end of string → return (base case).  
4. Else → call `reverseString(str+1)`, then print current character.  
5. Stop.  

---

### Sum of Natural Numbers
1. Start.  
2. Input number `n`.  
3. If `n <= 1` → return 1 (base case).  
4. Else → return `n + sumNumbers(n-1)` (recursive case).  
5. Display sum.  

---

##  Concepts Used
- **Recursion** → Core principle in all programs.  
- **Base & Recursive Cases** → Prevent infinite calls and define problem reduction.  
- **Stack Memory** → Stores recursive calls until base case is reached.  
- **Mathematical Induction** → Base step + recursive step approach.  
- **Pointers & Strings** → Used in string reversal program.  
- **Arithmetic Operations** → Used in digit reversal and summation.  

---

##  Conclusion
- Recursion is a powerful concept in programming that allows problems to be solved by breaking them into smaller subproblems.  
- It simplifies logic and provides clean solutions but consumes more memory due to the stack.  
- If the base case is missing, recursion can cause stack overflow.  
- Both **recursion and iteration** have their advantages; choice depends on efficiency requirements and problem nature.  

---
