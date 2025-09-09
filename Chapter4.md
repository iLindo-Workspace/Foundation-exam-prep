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
- *Often used in Unit testing and Static Analysis*
- *Tests logic, paths, loops, and conditions*
- *Focuses on the code structures and processing of the system (internals)*


(1.) **Experience-based Testing**
- *Based on experience of Tester, Dev, User*
- *Uses combination of Black/White-Box techniques*
- *Conditions/Test Cases based on Experience*
- *Will find defects that Black/White-Box may miss*




---
<h1 align="center">Black-Box Test Techniques</h1>



### Learning Objective 4.2.1 (k3) Use Equivalence Partitioning to derive Test cases

**Equevalence Partitioning** - *Divides input data into valid/invalid partitions to reduce Test Cases*

**Partitions can be**:
- *Discrete* - (Mon, Tue, Wed ...)
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
    - *Lookout for tight coupled conditions, and if they exist also ensure the T/F is exercised for them*
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

(1.) **Software implementations tested earlier**
- *It focuses on the internals logic of the code allowing dev/testers to examine code as soon as it is written*

(2.) **Defects detected early**
- *By examining control flows, logic, and conditions inside the code as soon as it is available*

(3.) **Prone to requirements omissions**
- *It focuses on the code and not requirements. If some requirements are missed or not implements it might not detect them*
- This is why it compliments Black-Box Testing (specification based), which focuses on requirements*

(4.) **Used as part of Static Testing**
- *Is performed without executing program*
    - *Code Reviews*
    - *Walkthroughs*
    - *Control flow analysis*
- *Static testing identifies defects before runtime*

(5.) **Part of code reviews**
- *Devs or Testers read the code line-by-line to check:*
    - *Correct logic*
    - *Proper handling of conditions*
    - *Potential exception errors*

(6.) **Review Logic (Control flow graph)**
- *Control flow graphs helps to visualize:*
    - *Loops*
    - *Decisions (if,switch)*
    - *Branching Paths*
- *To ensure that all paths are logically corrected and testable*

(7.) **Measure Coverage**
- *Uses metrics like:*
    - *Statement Coverage (every line executed)*
    - *Branch Coverage (every branch tested)*
    - *Path Coverage (every possible path is executed)*
- Helps to identify untested parts of the code*

(8.) **Additional tests to meet higher coverage**
- *To improve defect detection and overall software quality*

(9.) **Increased confidence in code**
- *Thorough testing of internal logic ensures that the code works as intended*
- *Devs and stakeholders gain confidence that the implementation is reliable.*



---

<h1 align="center">Experience-based Test Techniques</h1>

### Learning Objective 4.4.1 (k2) Explain Error Guessing

**Error Guessing**: *It is a Experience-Based Test Technique where by testers uses intuition, experience, and knowledge of common mistakes to design test cases that are likely to uncover defects*

---

### Learning Objective 4.4.2 (k2) Explain Exploratory testing

**Exploratory Testing**: *Also an Experience-Based Test approach where testers learn, design, and execute tests simultaneously, often used to find defects that scripted test cases may miss and used in Agile.*

---

### Learning Objective 4.4.3 (k2) Explain Checklist-based testing

**Checklist-Based Testing**: *Also Experience-Based Test approach that uses list of important items to verify, ensuring that testers systematically cover critical areas without writing full test cases. Static design Test approach*


---


<h1 align="center">Collaboration-based Test Approaches</h1>

### Learning Objective 4.5.1 (k2) Explain how to write User Stories in collaboration with developers and business representatives

*It's about writing User Stories together(Testers,Devs,BA's) with a goal of ensuring that it captures **Business value**, it is **Clear** to the Devs, and is **Testable**.*

---

### Learning Objective 4.5.2 (k2) Classify difference between option for writing Acceptance Criteria

**Acceptance Criteria**: *Are things that must happen in order to consider the user story to be "Done".*

*This can include **Test cases** (both negative and positive), **Scenarios**, and **examples** that must be tested*

- **Ways to Write Acceptance Criteria**:

    (1.) **Scenario-Oriented Approach (BDD)**
    - *Focuses on **Behavior** in specific scenarios*
    - *Uses **Given/When/Then** format*
    - *Is best for automation* 

    (2.) **Rule-Oriented Approach (Business Rules/Bullet list)**:
    - *Written as a list of conditions or rules*
    - *Focuses on input-output mappings and constraints*
    - *Easier for stakeholders to read quickly*
    - *Describes rules/conditions & fits business validation*


---

### Learning Objective 4.5.3 (k2) Use Acceptance Test-Driven Development to derive Test cases

- **Steps in ATDD**:

        (1.) Write User Stories (Collectively)
        (2.) Define Acceptance Criteria
        (3.) Turn Acceptance criteria into test cases (before code is written)
        (4.) Run test -> fail initially -> Devs writes code -> Test pass

- **Full Example**:
    - **User Story**:
            "As a [Customer], I want to [Withdraw cash] from the ATM, so that I can [Access my money].

    - **Acceptance Criteria (Scenario-Oriented, BDD style)**

            (1.) 

                - Given the account has sufficient funds,
                - When the customer withdraws an amount,
                - Then The ATM dispenses the money and updates the balance
            (2.) 

                - Given the account has insufficient funds,
                - When the customer tries to withdraws,
                - Then The ATM shows an error and cash is not dispensed


    - **Derived Test Cases (ATDD)**

        | **TestCase ID** | **Precondition**      | **Action**    | **Expected Results**                      |
        |-----------------|-----------------------|---------------|-------------------------------------------|
        | TC01            | Balance = R500        | Withdraw R100 | R100 dispensed, Balance updated to R400   |
        | TC02            | Balance = R50         | Withdraw R100 | Error message shown: "Insufficient Funds" |
        