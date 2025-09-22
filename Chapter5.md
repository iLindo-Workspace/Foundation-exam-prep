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
|Release of Product                     | Single Iteration (Sprint)                     |
|Define/Re-define product backlog       | Iteration Backlog participation               |
|Create Test plan for all iterations    | Iteration planning and activities             |
|Project/Product Risk analysis          | Detailed Risk analysis                        |
|Write Testable User Stories            | Ensure testability of User stories            |
|Refine user stories                    | Refine Stories to Task                        |
|Estimate Test effort                   | Estimate Test effort (Task Level)             |
|Test approach definitions              | Identify Non-Functional Characteristics       |
|Provide basis for Test Approach        |                                               |
|Define acceptance criteria             |                                               |

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

(1.) **UI/E-to-E Tests** - *1% - 5%*

(2.) **Integration Tests** - *5% - 15%*

(3.) **Unit Tests** - *80% - 90%*

                                            /\
                                           /  \
                                          /____\  -> 1
                                         /      \
                                        /________\  -> 2
                                       /          \
                                      /____________\ -> 3

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
- *Prevents Testing from Taking place*
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

(1.) **Project Progress Metrics** - (*Task Completion, Resource Usage, test effort*)

(2.) **Test Progress Metrics** - (*Test implementation Progress, Test Environment implementation progress, Number of Testcases run divided by number of Testcase not run, Number of Passed Testcases divide by Number of failed Test cases, Test execution time*)

(3.) **Product Quality Metrics** - (*Availability, response time, mean time to failure*)

(4.) **Defects Metrics** - (*Number and Priorities of Defects found divided by the Number of fixed defects, Defect density, Defect Detection Percentage*)

(5.) **Risk Metrics** - (*Residual Risk level*)

(6.) **Coverage Metrics** - (*Requirements coverage, Code coverage*)

(7.) **Cost Metrics** - (*Cost of testing, Organizational cost of quality*)

--- 

### Learning Objective 5.3.2 (K2) Summarize the purposes, content, and audiences for test reports

                                         Test Reports
                                        /            \
                                       /              \
    Test Monitoring & Control <- Test Progress      Test Summary -> Test Completion Activity

<span style="color:green; font-weight:bold;">N.B</span> Purpose of Test reports is to Communicate test information during (Progress) and after (Summary) Testing.

(1.) **Test Progress Reports** - (*Regular updates (daily/weekly/etc) that shows how testing is going while it's happening*)

- **Contents**
    - **Test Period** - (*Timeframe covered*)
    - **Actual Progress** - (*On track, ahead, or behind*)
    - **Impediments** - (*Blockers that the team faced and how they were handled*)
    - **Test Metrics** - (*Number of test executed, Passed/Failed, Defect density*)
    - **New/Changed Risks** 
    - **Testing planned for the next period** - (*What will be tested in the upcoming report cycle*)

(2.) **Test Summary Reports** - (*Created at the end of testing cycle project and give an overall evaluation of testing outcomes*)

- **Contents**
    - **Summary** - (*Overall of what wa tested, scope, results*)
    - **Evaluation of Testing + Quality against PLAN** 
    - **Deviations from Test Plan (Strategy)**
    - **Impediments (On workarounds)**
    - **Test Metrics** - (*Based/summarized progress reports*)
    - **Residual/Unmitigated Risks, Defects not fixed**
    - **Lesson learned for testing improvement** 

---


### Learning Objective 5.3.3 (K2) Exemplify how to communicate the status of testing 

(1.) **Verbal** - (*Team members, Stakeholders (daily stand-ups)*)

(2.) **Dashboards** - (*CI/CD dashboards, task boards, burn-down charts*)
 
(3.) **Electronic** - (*Email, Chat, Conference*)

(4.) **Online Documentation**

(5.) **Formal Reports** - (*Test Progress/Test Summary*)


---

<h1 align="center">Configuration Management</h1> 

### Learning Objective 5.4.1 (K2) Summarize how configuration management supports testing


**Configuration Management** - *Helps testing by ensuring consistency, traceability, and control of test artifacts, code, and environment throughout SDLC.*

(1.) **Referential Integrity & Traceability** - *CM links Requirements -> Design -> Code -> Test Cases -> Results*

(2.) **Version Control** - *Reduces confusion when multiple versions exists*

(3.) **Change Tracking & Impact Analysis** - *When code or requirements changes, CM is able to identify test cases that are impacted. Helps testers to re-run or update the necessary tests*

(4.) **Test Planning Integration** - *CM practices are initiated in test planning, ensuring the right basis is defined and managed from the start*

(5.) **CI/CD & DevOps** - *Ensuring repeatable stable environment for automated regression testing*

---

<h1 align="center">Defect Management</h1> 

### Learning Objective 5.5.1 (K3) Prepare a defect report 

**Defect report** - *Provides those responsible for resolving defects with* **sufficient information** *to resolve the issue. They also provide the means to* **track the quality** *of the work products. Offer* **insights** *for improvement of the development and test process*


- **Structure**
    - **Defect ID** - (*Uniquely Identifies the defect logged*)
    - **Title Summary** - (*Short description of the defect*)
    - **Date Reported** - (*When the defect was logged*)
    - **Reported By** - (*Author/Role(Tester,Dev)*)
    - **Issuing Organization** - (*Which team or company found the defect*)
    - **Test Object** - (*Item under test (module, feature)*)
    - **Test environment** - (*OS, Browser, Build number*)
    - **Context of Defect:**
        - **Test Case ID**
        - **Test Activity** (*function, regression, exploratory, etc*) 
        - **SDLC Phase** 
        - **Test Technique**
        - **Test Data**
    - **Steps to Reproduce** - (*Step-by-step actions*)
    - **Expected Results** - (*What should happen*)
    - **Actual Results** - (*What actually happens*)
    - **Severity** - (*Impact on the system (Critical, Major, Minor)*)
    - **Status** - (*New, Open, Fixed, Retest, Closed, Deferred*)
    - **References** - (*Related Requirements, Design Docs, or Test Cases*)
