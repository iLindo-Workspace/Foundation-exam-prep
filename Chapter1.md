# Summary of Chapter 1
## Make sure you give at least one example for each K2 Level

---






<h1 align="center"> What is Testing and Why do we test?</h1>

*It is the evaluation of functionality of a product under test against specified requirements to determine if its working as intended, also to identify defects with the intent of mitigating them so that they won't have much impact on the product, yielding to high quality product.*

*We do testing to reduce the level of risk and improve quality of a product before it goes live*

### Learning Objective 1.1.1 (k2) Identify Typical test objectives


(1. ) **Evaluate work products(requirements, user stories, design, code)**
- *Checking requirements, designs, code, and documentation before/during testing. Through Reviews and Static Testing*

(2. ) **Trigger failures and finding defects**
- *Executing test to reveal where the software does not behave as intended. Test execution*

(3. ) **Ensure required coverage for Test Object**
- *Confirm that enough  testing has been performed, be it Functional(black-box), Structural(white-box), Risk-Based, and Non-functional. Test Design, Test Execution, Monitoring*

(4. ) **Reduce risks of low software quality**
- *Focus on high-risk areas to prevent business failures. Test Planning, Test Execution* 

(5. ) **Verify specified requirements are met**
- *Check if the product does what the requirements/specification say. Test Design, Test Execution*

(6. ) **Verify whether the test object complies with legal, contractual, and regulatory requirements**
- *Ensure legal, safety and standards are satisfied. System & Acceptance Testing*

(7. ) **Provide information to stakeholeders to allow them to make informed decisions**
- *Report progress, risks, and quality metrics to stakeholders. Test Progress Report* 

(8. ) **Build confidence in the quality of the test object**
- *Show through repeated successful test that the product is ready. Test Execution, Test Reporting*

(9. ) **Validate that the test object is complete and works as expected by the stakeholders**
- *Confirm system completness and user expecttions are met. System & Acceptance Testing*


---

### Learning Objective 1.1.2 (k2) Differentiate Testing from Debugging
- *Testing generates failures in the software caused by defects in the code.*
- *Debugging is the process of finding root cause of the defect, analyse it, and fix it.*


#### Process encapsulating both Testing and Debugging

| **Testing**                                | **Debugging**              |
|--------------------------------------------|-----------------------------|
| (1) Generates failures caused by defects   | (2) Isolates the defect     |
| (7) Runs Confirmation/Re-test              | (3) Regenerates failure     |
| (8) Runs Regression test                   | (4) Diagnoses defect        |
|                                            | (5) Fixes defect            |
|                                            | (6) Checks fix              |

---
<h1 align="center">Why is Testing necessary?</h1>



### Learning Objective 1.2.1 (K2) Exemplify Why Testing is Necessary

**Success Factors**  
Testing contributes to project and product success by:  
- **Reducing risks and cost** → By identifying high-risk areas early, defects are found and fixed before the product is released, preventing expensive late fixes.  
- **Improving collaboration** → Testers, business analysts, developers, project managers, and stakeholders work together toward the same goal of delivering quality.  
- **Supporting decisions** → Test reports provide insights on product readiness, enabling stakeholders to make informed release decisions.  
- **Improving quality** → Multiple test executions help mitigate risks and ensure reliability.  
- **Ensuring compliance** → Testing checks that the product follows regulations, standards, and contractual obligations.  
- **Delivering value** → Ensures the product meets business requirements and user needs.  

**Consequences of No or Insufficient Testing**  
- **Safety risks** → In critical domains (e.g., medical devices, aviation, automotive), software failures can cause injury or loss of life.  
- **Financial loss** → Defects in production can lead to costly downtime, recovery, and penalties.  
- **Reputation damage** → Poor quality releases reduce customer trust and damage the brand.  

---
### Learning Objective 1.2.2 (k1) Recall the ralation between Testing and Quality Assurance

**Quality Mangement** = *Quality Assurance + Quality Control (**This is where Testing is**)*

- **QA** - is Proactive, focuses on the processes use to develop the product with a goal of preventing defects(through training, standards, guidelines, documentations). Happens before and during development
- **QC** - is Reactive, product oriented, checks for the level of quality and if the product is working as expected (through testing reviews, inspections).

---
### Learning Objective 1.2.3 (k2) Distinguish between Root Cause, Failure, Defect, and Error

| **Term**       | **Who/What caused it**      | **Where it exist**            | **When it appears** | **Example**                 |
|----------------|-----------------------------|-------------------------------|---------------------|-----------------------------|
| Error          | Human Mistake               | Req, Design, Code             | During Development  | Wrong Logic                 |
| Defect         | Result of an Error          | In a Code or System           | During Testing      | Incorrect Calculation       |
| Failure        | Execution of Defect         | In a running System           | During runtime      | App Crashes                 |
| Root Cause     | Underlying issues           | In a process of Understanding | during Analysis     | Misinterpreted specification |


#### **How they relate**
- Root cause (lack of training)
- Leads to Error (wrong logic written by developer)
- Creates defect (fault in the code)
- Which results to a failure (Software not working as it expected)
---

<h1 align="center">Testing Principles</h1>

### Learning Objective 1.3.1 (k2) Explain the Sevent Testing Principles
(1. ) **Testing shows presence of defects, not their absence**
- Testing proves that bugs do exist, but it can never prove that **NO** bugs exist

(2. ) **Exhaustive Testing is impossible**
- You cannot test everything (all inputs, combinations, paths), insted focus your test on priorities, risks, and critical areas

(3. ) **Early testing saves time and money**
- The earlier the defect is found in the SDLC the Cheaper it is to fix

(4. ) **Defects cluster together**
- Refers to certain modules being more error-prone than others, so testers focus more effort there.

(5. ) **Pesticide Paradox/Test Wear Out**
- Running the same test case repeatedly will no longer find new defects. Solution is to regularly review and improve test cases, add variations, and change scenarios

(6. ) **Testing is Context-dependent**
- Testing depends on the type of system(games, aviation software) and risks involved

(7. ) **Absence-of-Defect Fallacy**
- Just because that the software is defect free doesn't mean it meets the business needs

---

<h1 align="center">Testing Activities, Testware and Test Roles</h1>

### Learning Objective 1.4.1 (k2) Summarize the different Test activities, and Tasks


(1. ) **Test Planning**
- *Identify Objectives and Risks*
- *Select Test Strategy & Approach*
- *Define Entry & Exit Criteria*
- *Estimate Effort & Resources*
- *Schedule Test Activities*

(2. ) **Test Monitoring & Control**
- *Measure test progress (planned vs actual)*
- *Report Test Status*
- *Adjust plans when necessary*

(3. ) **Test Analysis**
- *Review requirements, user stories, or design documents*
- *Identify what to test*
- *Define Test conditions and prioritize them*

(4. ) **Test Design**
- *Derive Test Cases from Test Conditions*
- *Identify Test Data*
- *Identify Test environment needs/Requirements/Tools*
- *Test steps*
- *Define expected results*

(5. ) **Test Implementation**
- *Develop Automated/Manual test scripts*
- *Organize Test Suites*
- *Verify Test environment setup*
- *Create Test Execution Schedule*

(6. ) **Test Execution**
- *Execute Test cases (Manual/Automate)*
- *Compare Actual vs Expect results*
- *Log defect for failures*
- *Re-test/Confirmation after fixes*
- *Run Regression Testing*

(7. ) **Test Completion**
- *Check Exit criteria is met*
- *Archive Testware & data for reuse*
- *Document Lesson learned*
- *Write final Test Summary Report*

---
### Learning Objective 1.4.2 (k2) Explain the Impact of Context on the Test Process

- **SDLC**
    - *Waterfall - Testing is done on the later stage, and has heavy documentation*
    - *Agile - Testing is continuous, and lighter documentation*
- **Project/Product Risk**
    - *High-risk systems like (Banking, Aviation, Medical) require regorous testing*
    - *Low-risk system like games, websites may need only just basic Functional Testing*
- **Time & Budget Constraits**
    - *When deadlines are tight, we use Risk-Based Testing, focus on critical features first*
    - *When Budget is high, broader coverage, more automation, performance testing*
- **Business & Regulatory Requirements**
    - *Some domains (finance, health, government) require compliance with legal or safety standards*
- **Technology & Tools Used**
    - *Testing differes for Web apps, Mobile apps, Embedded systems, Cloud Systems
- **Team skils & Experience**
    - *More experienced testers can design exploraory tests, automation, performance*
    - *Junior team may rely more on checklist and pre-written scripts*
- **Stakeholders**
    - *If customer cares more about perfomance - Load/Stress testing emphasized*
    - *If the care more about UX - Usability testing is emphasized*

*Test Process is Context-Dependent (Test principle No. 6). Factors like SDLC, Risks, Deadlines, Regulations, Technology, Team skills, and Business prioritise influence how testing is planned, designed, and executed*

---
### Learning Objective 1.4.3 (k2) Differentiate Testware that supports the Test Activities


**Testware**: *All the artifacts (documents, tools, scripts, data) created and used to support Testing*

(1. ) **Test Planning**
- *Test Plan*
- *Risk Analysis Report*
- *Schedule and Resource Plan*

(2. ) **Test Monitoring & Control**
- *Test Progress Reports (planned vs actual)*
- *Test Status Dashboards*

(3. ) **Test Analysis**
- *Test Conditions*
- *Traceability Metrics*

(4. ) **Test Design**
- *Test Cases*
- *Test Data Requirements*
- *Test Procedures (step-by-step execution instructions)*


(5. ) **Test Implementation**
- *Automated/Manual test scripts*
- *Test Suites*
- *Environment setup scripts*
- Test Execution Schedule*

(6. ) **Test Execution**
- *Test Logs(Results of each test run)*
- *Defects report*
- *Screenshots*

(7. ) **Test Completion**
- *Archive Test cases and scripts for reuse*
- *Lesson learned/Retrospective notes*
- *Test Summary Report*

---

### Learning Objective 1.4.4 (k2) Explain the value of maintaining Traceability


- **Traceability**: *Is the ability to link related work products across SDLC.*
    - *In testing it means linking Requirements → Test Conditions → Test Cases → Defects → Test Results*

(1. ) **Ensures Coverage**
- *Every Requirement is Tested*
- *You can verify that no requirement is missed*

(2. ) **Supports Impact Analysis**
- *When requirements, traceability helps identifying affected test cases and defects*

(3. ) **Improves Defect Management**
- *Defects can be traced back to the requirement or test case that revealed it*

(4. ) **Provides audit & Compliance Evidence**
- *Especially important for regulated industries, traceability prooves that all requirements where tested and defects are handled*

(5. ) **Facilitates Reporting and Decision Making**
- *Test Managers and Stakeholders can see test progress status*

(6. ) **Helps reuse and Maintenance**
- *Test cases linke to requirements can be reused in Regression testing or future releases, makes maintaning and updating test much easier*

---
### Learning Objective 1.4.5 (k2) Compare Diffferent Roles in Testing


| **Test Manager**         | **Tester**           |
|--------------------------|----------------------|
| Test Process             | Test Analysis        |
| Test Planning            | Test Design          |
| Team Leader              | Test Implementation  |
| Test Monitoring & Control| Test Execution       |
| Test Completion          | Technical Engineering|

---


<h1 align="center">Essential Skills and Good Practices in Testing</h1>

### Learning Objective 1.5.1 (k2) Give examples of Generic skills required in Testing
- **Analytical skills**
    - *Ability to understand complex systems, requirements, and workflows*
    - *Helps to identify what to test and where defects might hide*
- **Attention to Details**
    - *Carefully noticing small deviations and inconsistencies*
- **Critical Thinking**
    - *Questioning assumptions, considering alternatives, asserting risk logically*
- **Communication skills**
    - *Clearly document defects, writing test cases, and reporting findings*
- **Creativity** 
    - *Thinking of unexpected scenarios that might reveal hidden defects*
- **Curiosity/Investigative mindset**
    - *Desire to dive deeper to understand why something fails rather than doing nothing*
- **Risk Awareness**
    - *Understand which areas are most likely to fail and the impact of defects*
- **Team work and Collaboration**
    - Working effectively wih everyone involved is critical

---

### Learning Objective 1.5.2 (k1) Recall advantages of the Whole Team Approach
(1. ) *All responsible for quality*

(2. ) *Share expertise and knowledge with the team*

(3. ) *Co-Location = better Collaboration & Communication*

(4. ) *Tester helps Business Rep create Acceptance criteria*

(4. ) *Tester works with Developer to create Test Strategy*

(5. ) *Leverage skills/experience*

(6. ) *Sometimes high level of independancy*

---

### Learning Objective 1.5.3 (k2) Distinguish the Benefits and Drawbacks of Independancy Testing


**Independence Testing**: *Refers to testing from different perspective*


**Benefits**:

(1. ) **Avoids Authors Bias**
- *The person who wrote the code is less likely to spot their own mistakes*

(2. ) **Fresh Perspective**
- *Independent tester may notice different defects that developers*

(3. ) **Challenge Assumption**
- They can question requirements, designs, and implementations that developers might take for granted

(4. ) **Increased confidence in results**
- Independent confirmation that the product works as expected

**Drawbacks**:

(1. ) **Loss of Responsibility**
- *Developers may rely too much on testers and neglecting unit testing*

(2. ) **Poor Communication**
- *If the independent tester is too rigid, communication suffers, leads to poor/low quality*

(3. ) **Testing seen as a Bottleneck**
- *When Testing is separate, project may blame testers for slow delivery*

(4. ) **"Us vs Them" Mentality**
- *Separation can create tension instead of team work*

**Levels of Independence**
- Author test own work **(No independence)**
- Different person in the same team **(Low independence)**
- Independent Test Team **(High independence)**
- Business Reps or User Testers **(UAT, even higher independence)**