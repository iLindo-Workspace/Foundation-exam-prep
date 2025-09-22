# Summary of Chapter 2
## Make sure you give at least one example for each K2 Level

---
<h1 align="center">Testing in the Context of SDLC</h1>


### Learning Objective 2.1.1 (K2) Explain the impact of the chosen SDLC in Testing
(1. ) Scope & Timing
- **Sequential Models**: *Testing is only performed after development phases, so scope is defined early, but testing is squeezed at the end*
- **Agile/Iterative**: *Testing is continuous, with scope evolving sprint-by-sprint.* 

(2. ) Level of details of Testware
- **Waterfall**: *Formal and detailed testware because requirements are stable and fixed*
- **Agile**: *Lightweight test documents because it's lean and adaptive to ever changing requirements*

(3. ) Test Technique
- **Waterfall/V-Shape**: *Strong reliance on formal test design techniques (EP,BVA,Decision Tables, State Transition Testing) since Test basis is detailed requirements*
- **Agile**: *Mix of Exploratory Testing, ATDD, and Risk-based techniques because requirements change often.*

(4. ) Test Approach
- **Waterfall**: *Preventive, Structured Approach (detailed Planning)*
- **Agile**: *Reactive, Flexible Approach (Continuous Adaptation)*

(5. ) Extent of Test Automation
- **Waterfall**: *Less automation, more manual testing*
- **Agile**: *High automation (unit testing, regression, CI/CD, performance, security) to support continuous delivery*

(6. ) Roles & Responsibilities
- **Waterfall**: *Testers are usually independent from the developers, testing is a separate phase.*
- **Agile**: *Whole team Approach, Developers, Testers BA's collaborate on Testing*

---

### Learning Objective 2.1.2 (K1) Recall good testing practices that apply to all SDLC's

(1. ) *Every development activity has a corresponding test activity (V-Shape Model)*

(2. ) *Each test level must have a specific (and different) objective for that level*

(3. ) *Test Analysis and Test Design should start DURING the corresponding development activity*

(4. ) *Tester start Reviewing Draft versions of User stories/Technical Designs and not wait until final version are completed*


---
### Learning Objective 2.1.3 (K1) Recall examples of test-first approaches in development

(1. ) **Test-Driven Development Approach** - *Focuses on unit level (developer tests)*
- **Direct code through test cases**
- **Process** → RED - GREEN - REFACTOR :
    - Write Test first (but will fail since there's no code to test) <span style="color:red; font-weight:bold;">RED</span> 
    - Developer writes minimum code to make test pass <span style="color:green; font-weight:bold;">GREEN</span> 
    - Refactor the code (clean it up, improve design) while keeping test passing  <span style="color:orange; font-weight:bold;">REFACTOR</span> 

(2. ) **Acceptance Test-Driven Development Approach** - *Focuses on Customer/Business Acceptance criteria*
- **Test cases are created based on Acceptance Criteria**
- **Process**:
    - *3 Amigos (BA's, Devs, Testers) meet and define Acceptance Criteria before code*
    - *Coding is developed until acceptance criteria test is passed*

(3. ) **Behavior Driven Development Approach** - *Systems behavior from user perspective*
- **Process**:
    - *3 Amigos meet up and discuss features and desired behaviors*
    - *Define Scenarios using Given-When-Then to express examples of behavior*
    - *Scenarios are turned into automated acceptance test*
    - *Code is developed until scenarios are passed*
    - *Refactor and Maintain*


---
### Learning Objective 2.1.4 (K2) Summarize how DevOps might have an impact on Testing

(1. ) **Organizational Approach**
- *Is about bridging Development with Operations. Shared responsibility equally*

(2. ) **Autonomy & Collaboration**
- *Team work, Cross-functionality*

(3. ) **Fast Feedback**
- *Testing is build into pipelines to provide immediate feedback on code changes*

(4. ) **Integrated Tool**
- *Test tools are integrated with DevOps tool chains*

(5. ) **CI/CD**
- **Requires**:
    - *Shift-Left Testing (component testing, static analysis)*
    - *Automated Regression suites*
    - *Automated Pipeline*

(6. ) **Non-Functional quality characteristics**
- *Performance, Security, Reliability are validated continuously, not only at the end*


---
### Learning Objective 2.1.5 (K2) Explain Shift-Left Approach

**Shift-Left** - *means moving test activities earlier in the SDLC*

**Practices**

(1. ) **Review for Testability**
- *Analyze requirements, designs, user stories before coding to ensure they can be tested effectively*

(2. ) **Test cases before Coding**
- *Develop unit, integration, acceptance testing (test-first approaches) earlier so that development is guided by them

(3. ) **CI/CD  = Automated components test**
- *Continuous Integration runs automated test whenever there's a code commit to catch issues earlier*

(4. ) **Static Analysis before Dynamic Testing**
- *Checks requirements, code, design without execution*

(5. ) **Non-Functional Testing at Component Level**
- *Test performance, reliability, and security early and not after completion*


### Learning Objective 2.1.6 (K2) Explain how retrospectives can me used as a mechanism for process improvement

**Retrospectives** - *Are meetings are held at the end of Iteration/Sprint/Milestone/Project*

- Usually everyone who is part of the project is part of these meetings
- Test Summary reports are written (results of the project)
- Discussions:
    - *What worked (keep it going)*
    - *What didn't work (ideas to fix)*
    - *How to improve to ensure success in the future*



---

<h1 align="center">Test Levels & Test Types</h1>

### Learning Objective 2.2.1 (K2) Distinguish the different Test Levels

**Test Levels** - *Are groups of activities that focus on a specific level of Testing*

(1. ) **Component/Unit Testing** (*Performed by Devs*) - *Tests individual components to verify if each component works as specified*

(2. ) **Component Integration Testing** - (*Performed by Devs or Testers*) - *Test interfaces and interactions between components/modules to ensure that they interact correctly*

(3. ) **System Testing** - (*Often performed by independent testers*) - *Test the system as a whole to validate that the system meets the requirements*

(4. ) **System Integration Testing** (*Performed by Testers*) - *Tests the interactions between systems to verify if they work together* 

(5. ) **Acceptance Testing** (*Performed by Customers, End-users, Business Reps*) - *Test the full system in the real-world environment to confirm if the system is acceptable for delivery and meets business/user need*

---
### Learning Objective 2.2.2 (K2) Distinguish the different Test Types

(1. ) **Functional Testing** - *What the system does aka Specification Based Testing*
- *Functional Behavior*
- *Black-Box*

(2. ) **Non-Functional Testing** - *How the system does it*
- *Characteristics, attributes, properties of the system*
- *"How well" the system behaves*

(3. ) **Black-Box** - *Specification based*
- *Test cases derived from specifications*
- "Works as required"

(4. ) **White-Box** - *Structural testing*
- *Derives test cases from the systems implementation or internal structure*
- *Thoroughness - Coverage*:
    - *Statement/Decision Coverage*
    - *Component/Modules/Units coverage*
    - *Functions/Feature Coverage*
    - *Workflows covered*


---
### Learning Objective 2.2.3 (K2) Distinguish Confirmation testing from Regression Testing

- **Confirmation Testing**: *Testing to confirm that reported defects have been fixed*

- **Regression Testing** - *Testing to check if new changes (fixes, enhancements, updates) did not introduce defects into unchanged parts of the system*

---


<h1 align="center">Maintenance Testing</h1>

### Learning Objective 2.3.1 (K2) Summarize Maintenance Testing and its Triggers

**Maintenance testing** - *Is to do with changes to the production/live environment*

- **Triggers**:
    - Modification - *Any enhancements, corrective and emergency fixes (hardware, software, middleware, OS)*
    - Migration - *From one platform to another, it can be system or data*
    - Retirement - *Phasing out of a system*