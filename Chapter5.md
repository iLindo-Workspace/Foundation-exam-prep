# Summary of Chapter 5
## Make sure you give at least one example for each K2 Level

---



<h1 align="center"> Test Planning</h1>



### Learning Objective 5.1.1 (K2) Exemplify the purpose and content of a test plan

| **Purpose**                  | **Contents**                |
|------------------------------|-----------------------------|
|Implements Policy/Strategy    | Objectives                  |
|Sets Test Objectives          | Scope                       |
|Means & Schedule              | Constrains/Assumptions      |
|Resources                     | Stakeholders                |
|Communicates Test Approach    | Communication               |
|Meets established criteria    | Risk/Risk Register          |
|Communicates level of document| Feature to Test/Not to test |
|Guid's Tester's thinking      | Budget/Schedule             |
---

### Learning Objective  5.1.2 (K1) Recognize how a tester adds value to iteration and release planning

**Testers contribute to both release planning and iteration planning, but their focus and activities differ depending on the level:**

- **Release Planning** - *Focuses on the overall project, High-level Strategy(long-term).* **Product level** 

- **Iteration Planning** - *Detailed, tactical(short-term)* **Team Level**


|           **Release Planning**        |            **Iteration Planning**             |
|---------------------------------------|-----------------------------------------------|
|Define/Re-define product backlog       | Iteration Backlog participation               |
|Test approach definitions              | Iteration planning and activities             |
|Refine user stories                    | Detailed Risk analysis                        |
|Provide basis for Test Approach        | Ensure testability of User stories            |
|Create Test plan for all iterations    | Refine Stories to Task                        |
|Define acceptance criteria             | Estimate Test effort (TAsk Level)             |
|Project/Product Risk analysis          | Identify Non-Functional Characteristics       |
|Estimate Test effort                   |                                               |


---

### Learning Objective  5.1.3 (K2) Compare and contrast entry criteria and exit criteria

(1.) **Entry Criteria** 
- *All the things that must take place before testing activities starts*
- *Conditions that must be met before testing activities begin*

(2.) **Exit Criteria**
- *What must happen for testing to stop*
- *Conditions that must be met in order to consider testing is "DONE"*


- **Entry**
    - *Availability of Req's/User stories/Models*
    - *Quality of test object*
    - *Availability of test items that have passed in previous Test Level*
    - *Test Environment*
    - *Test tools ready*
    - *Test Data*
    - *Budget/Time*
    - *Anything needed to test*

- **Exit**
    - *Planned Test Executed (thoroughness)*
    - *Risk Mitigation*
    - *Level of Coverage met*
    - *Completion Criteria*
    - *Open defects within agreed limit*
    - *"DONE"*
    - *Project Constraints (Budget/Time)*
---

### Learning Objective  5.1.4 (K3) Use estimation techniques to calculate the required test effort

**Test Effort** - *The amount of work required to meet test objectives*

**4 types of Estimation techniques**

(1.) **Ratio** - *Metrics based on historical data*

(2.) **Extrapolation** - *Metrics based on current iteration data*

(3.) **Wideband Delphi** - *Expert based, Consensus*

(4.) **Three-Point** - *Optimistic* **(a)**, *most likely* **(m)**, *pessimistic* **(b)**.
- *Formula* - **(a + 4 * m + b) / 6**

---

### Learning Objective  5.1.5 (K3) Apply test case prioritization

**Test Case Prioritization** - *Is about which test case to run first when time or resources are limited*

**Prioritizing** - *is the selection and ordering test cases to maximized value of testing*

**Levels of Prioritization**
- **Risk-Based** - *Focuses on areas of high-risk*
- **Coverage-Based** - *Prioritizes test cases that cover the most functionality or critical paths*
- **Requirements-Based** - *Prioritizes base on requirements importance*

---

### Learning Objective  5.1.6 (K1) Recall the concepts of the test pyramid


**The Test Pyramid is a visual metaphor that helps teams structure their automated testing strategy. It emphasizes having more low-level, fast, and reliable tests and fewer high-level, slow, and brittle tests.**


| **Layer**         | **Description**                                 | **Example**                    |
|-------------------|-------------------------------------------------|--------------------------------|
|Unit Tests         | Test individual components or functions         | Function tests, Class methods  |
|Integration Tests  | Test interactions between components or systems | API tests, Database connections|
|UI/E-to-E Tests    | Test entire system through the user interface   | Selenium test, user workflows  |




---

### Learning Objective  5.1.7 (K2) Summarize the testing quadrants and their relationships with test levels and test types

(1.) **Quadrant 1** *(Technology-Facing, Support the Team)*
- *Focuses on code quality, correctness*
- *Gives developers fast feedback, ensure the code works as intended*

(2.) **Quadrant 2** *(Business-Facing, Support the Team)*
- *Focuses on functionality, requirements validations*
- *Acceptance Test, Functional Test*
- *Confirms that the system does what the business needs*

(3.) **Quadrant 3** *(Business-Facing, Critique Product)*
- *Focuses on exploring system behavior from user's perspective*
- *System Testing, User Acceptance Testing, Usability Testing*
- *Evaluates product from end-user's view, find gaps/defects*

(4.) **Quadrant 4** *(Technology-Facing, Critique Product)*
- *Focuses on Non-Functional Qualities and Performance*
- *Performance, Security, Load/Stress Testing*
- *Exposes weakness in quality attributes*

---
<h1 align="center">Risk Management</h1>

### Learning Objective 5.2.1 (K1) Identify risk level by using risk likelihood and risk impact

**Risk** - *Is the likelihood of something to happen (possibility), and if it does what would be the impact (damage)*

**Risk Level** - *Is the factor of Likelihood * a factor of Impact*


**Risk Management has**:

(1.) **Risk Analysis** - *Involves identifying and assessing risks to the project/product*
- **Activities**
    - *Identifying potential failures (Technical, Business, Operation)*
    - *Assessing likelihood and impact of each risk*
    - **Outcomes** -> *Risk Register (Part of Test Plan)*

(2.) **Risk Control** - *Mitigates and Monitors Risks*
- **Activities**
    - **Mitigation** - *Actions to reduce likelihood or impact of risk(Extra testing, Automation, Reviews)*
    - **Monitoring** - *Regularly checking risk status and update plans*


**Risk-Based Testing**
*Risk influences how testing is performed:*

(1.) **Test Activities Used** - *Focuses effort on high-risk areas first*

(2.) **Prioritization** - *Executes test cases for high-risk features earlier*

(3.) **Coverage** - *Ensures critical features receives sufficient test coverage*

(4.) **Technique Used** - *Apply appropriate testing technique(exploratory testing, etc)*

(5.) **Management** - *Allocate resources, monitor progress, and report on risk mitigation*


---

### Learning Objective 5.2.2 (K2) Distinguish between project risks and product risks


(1.) **Project Risks**
- *Impact Testing Service Delivery, Test Schedule/Budget/Scope*
- *Prevents Testing from Tsking place*
- *Causes Testing to take longer than planned*
- *Includes*
    - *Organizational issues*
    - *People Issues*
    - *Supplier Issues*
    - *Technical Issues*

(2.) **Product Risks**
- *Product not of expected Quality(Functional, Performance)*
- *Software may not work as expected*
- *Software may not work in the intended environment*
- *Leads to:*
    - *User dissatisfaction*
    - *Loss of revenue, trust, and reputation*
    - *Maintenance cost*
    - *Legal penalties*
    - *Loss if life or harm*

---

### Learning Objective 5.2.3 (K2) Explain how product risk analysis may influence thoroughness and test scope


- *Coverage*
- *Scope*
- *Types and Levels of Testing*
- *Type of Design Technique*
- *Level of Testing*
- *Type of Testing*
- *Priorities*
- *Extent of Testing*
- *Non-Testing Activities to reduce risk*
---

### Learning Objective 5.2.4 (K2) Explain what measures can be taken in response to analyzed product risks 

**Product Risk Control** - *Is a response to identified product risks*
- *Consist of Risk Mitigation = Testing, Acceptance, Transfer, Contingency planning = actions to reduce risk*

- *and Risk Monitoring = Effectiveness of Actions, Improve Risk Management*

 - **Examples of Mitigation:**
    - *Testers with relevant experience / skills*
    - *Level of Test Independence*
    - *Appropriate Test Techniques and Coverage*
    - *Appropriate Test Types for Quality Characteristics*
    - *Dynamic Testing*
    - *Regression Testing*
---

<h1 align="center">Test Monitoring, Test Control, Test Completion</h1> 

### Learning Objective 5.3.1 (K1) Recall metrics used for testing



--- 

### Learning Objective 5.3.2 (K2) Summarize the purposes, content, and audiences for test reports

---


### Learning Objective 5.3.3 (K2) Exemplify how to communicate the status of testing 

---

<h1 align="center">Configuration Management</h1> 

### Learning Objective 5.4.1 (K2) Summarize how configuration management supports testing
---

<h1 align="center">Defect Management</h1> 

### Learning Objective 5.5.1 (K3) Prepare a defect report 