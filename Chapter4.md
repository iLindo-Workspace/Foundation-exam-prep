# Summary of Chapter 4
## Make sure you give at least one example for each K2 Level

---






<h1 align="center"> Test Techniques Overview</h1>



### Learning Objective 4.1.1 (k2) Distinguish between Black-Box, White-Box, and Experience-based Testing Techniques

(1.) **Black-Box**
- *Specification based*
- *Requires code execution*
- *Checks if the system works as required*
- *Focuses on inputs and outputs, not the internals*
- *Includes both Functional and Non-Functional testing*
- *Focuses on the Behavior of the system (Externals)*


(2.) **White-Box**
- *Structural based*
- *Requires NO code execution*
- *Testing the structures of the code and confirms if it works as required*
- *Often used in Unit testing and Statis Analysis*
- *Tests logic, paths, loops, and conditions*
- *Focuses on the code structures and processing of the system (internals)*


(1.) **Experience-based Testing**
- *Based on experince of Tester, Dev, User*
- *Uses combination of Black/White-Box techniques*
- *Conditions/Test Cases based on Experiecnce*
- *Will find defects that Black/White-Box may miss*




---
<h1 align="center">Black-Box Test Techniques</h1>



### Learning Objective 4.2.1 (k3) Use Equivalence Partitioning to derive Test cases

**Equevalence Partitioning** - *Divides input data into valid/invalid partitions to reduce Test Cases*

**Partitions can be**:
- *Descrete* - (Mon, Tue, Wed ...)
- *Continuous* - (<0 to 100 >)
- *Unordered* - (Red, Blue, Orange ...)
- *Ordered* - (S, M, L, XL)

 <span style="color:green; font-weight:bold;">**N.B**</span>   *100% coverage is achieved by test cases that exercise all defined equivalence classes, both the valid and invalid partitions*

---
### Learning Objective 4.2.2 (k3) Use State Boundary Value Analysis to derive Test cases

**BVA** - *Focuses on edges of input ranges where bugs often occur*

- *Works with ranges (Minimum & Maximum Values)*
- *Used to test calculations*
- *When the risk high and you want to strengthen your tests, use 3BVA*

<span style="color:green; font-weight:bold;">**N.B**</span> *To achieve 100% Boundary Value Analysis (BVA) coverage, create test cases that include all boundary values of each input range, including the minimum, maximum, just above the minimum, just below the maximum, and values just outside the valid range.*


---
### Learning Objective 4.2.3 (k3) Use Decision Table to derive Test cases

**Decision Logic Table** - *Uses tables to model complex business rules and conditions*

- *Tests combination of business rules and their relationship to each other*
- *Identify business rules (Conditions)*
- *Identify actions (Results of combining rules)*
- *Answer = True/False*


**Rationalization** - *Used for eliminating extra test cases*
- **RULES**
    - *Your test cases should exercise both True and False for each condition*
    - *Lookout for tight coupled conditions, and if they exist also ansure the T/F is exercised for them*
    - *Once you have noticed repeating test cases, you can start eliminating*

<span style="color:green; font-weight:bold;">**N.B**</span>  *To achieve 100% coverage in Decision Table Testing, create test cases that cover every rule (i.e., every unique combination of conditions and their corresponding actions) in the decision table.*

---

### Learning Objective 4.2.4 (k3) Use State Transition Testing to derive Test cases

**State Transition Testing** - *Tests system behavior based on changes and events*

- *Test workflows, process flows, Navigation through the system*
- *State Transition Diagram = Positive Tests*
- *State Transition Table = Negative Test*
- *When risk is high and you want to strengthen your test use*:
    - *0 Switch:* Tests pair of States
    - *1 Switch:* Test pair of Events/Transitions

<span style="color:green; font-weight:bold;">**N.B**</span> *To achieve 100% coverage in State Transition Testing, design test cases that ensure every possible state and every valid transition between states is exercised at least once.*

---

<h1 align="center">White-Box Test Techniques</h1> 



### Learning Objective 4.3.1 (k2) Explain Statement Testing

*Focuses on the coverage of statements, how many executable statements are exercised out of total number of statements*

---

### Learning Objective 4.3.2 (k2) Explain Branch/Decision Testing

*Focuses on outcomes of Decisions (True/False) such as "if statements", and loops structures*

---

### Learning Objective 4.3.3 (k2) Explain the value of White-Box Testing

---

<h1 align="center">Experience-based Test Techniques</h1>

### Learning Objective 4.4.1 (k2) Explain Error Guessing

---

### Learning Objective 4.4.2 (k2) Explain Exploratory testing

---

### Learning Objective 4.4.3 (k2) Explain Checklist-based testing


---


<h1 align="center">Collaboration-based Test Approches</h1>

### Learning Objective 4.5.1 (k2) Explain how to write User Stories in collaboration with developers and business


---

### Learning Objective 4.5.2 (k2) Classify differemce between option for writting Acceptance Criteria


---

### Learning Objective 4.5.3 (k2) Use Acceptance Test-Driven Development to derive Test cases


