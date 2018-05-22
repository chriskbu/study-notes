### Week 1 - Fundamentals of testing

#### The seven principles of testing

* **P1. Testing shows presence of defects**
  * Testing can show that defects are present, but cannot prove there are no defects. 
  * Testing reduces probability of undiscovered defects remaining in the software; but even if no defects are found,
    this is not a proof of correctness.
* **P2. Exhaustive testing is impossible**
  * Tesing everything is not feasable. We use risks and priorities to focus test efforts.
* **P3. Early testing**
  * Testing should start as soon as possible in the development life-cycle and should be focused on defined objectives.
* **P4. Defect clustering**
  * A small number of modules contain most of the defects discovered during pre-release testing.
* **P5. Pesticide paradox**
  * If the same set of tests will be repeated over and over, it will no longer find new bugs.
* **P6. Testing is context dependent**
  * i.e. safety-critical SW is tested differently than an e-commercial website.
* **P7. Absense-of-errors fallacy**
  * Finding and fixing defects does not help if the SW system is unstable or does not meet the users expectations.

#### What is testing

The process consisting of all life cycle activities for both:

* Static
* Dynamic

Concerned with the planning, preparation and evaluation
of software products and related work products
to determing the satisfy the specified requirements
to demonstrate that they are fit for purpose
to detect defects.

#### Testing can be focused on

* Confirming that the software system meets the requirements
* Causing as many failures as possible
* Check that no defects have been introduced during changes
* Assess the quality of the software (with no intention of finding bugs)
* Finding defects to reduce the probability of undiscovered defects
* Gaining confidence in the level of quality
* Providing information for decision-making
* Preventing defects

#### Different states of testing

* Test planning
  * A team dedicated to planning.
  * Determine what is being tested.
  * Determine what tools and methods are being used.
* Test control
  * Check if plans are followed and reevaluate them.
* Test analysis
  * Analyse the project.
  * Determine cases and input.
* Test design
  * Automated tests, usertests?
* Test implementation
  * Generate testdata and implement tests.
* Test execution
  * Execute the tests with the test input.
* Checking results
  * Check results for all tests.
* Evaluating exit criteria
  * Check if exit criterias are fufilled.
* Test result reporting
  * Create reports.
* Test closure
  * Archive the reports and datas for later use.

##### Plan and control

* Plan means: what, how, when, by whom?
  * Scope, objectives and risk analysis
  * Test levels and types that will be applied
  * Documentation that will be produced
  * Assign resources for the different test activites
  * Schedule test implementation, execution, evaluation
* Control and adjust the planning to reflect new information, new challenges of the project

##### Analysis and design

* Review test basis:
  * Requirements
  * Product architecture
  * Product design
  * Interfaces
  * Risk analysis report
  * **Confirm text material is correct**
* Analysis: general test objectives are transformed into
  * Test conditions
  * Test cases
* Design:
  * Test cases
  * Test environments
  * Test data
  * Create tracebility

##### Implementation and execution

* Implement
  * Group tests into scripts
  * Prioritize the scripts
  * Prepare test oracles (expected output)
  * Write automated test scenarios
* Execute
  * Run the tests and compare with oracles
  * Report incidents
  * Repeat test activities for each corrected discrepancy
  * Log the outcome of the test execution

##### Evaluate exit criteria and report

* Evaluate:
  * Assess the test execution
  * Check if
    * more tests are needed
    * exit criteria should be changed
* Report
  * Write or extract a test summary report for stackeholders

##### Test closure activities

* What deliverables have been delivered? Is there anything missing?
* Check the closure of incident reports
* Achive the items delivered:
  * SW code
  * Set of tests & results
  * Documentation created/updated
    * *this is necessary for future reuse*
* Analyze lessons learned for future releases

#### The psychology of testing

##### Skills needed

* Curiosity
* Professional pessimism
* Attention to details
* Good communication skills
* Experience on error guessing

* Communicate failures in a constructive way
  * Fact-focused - give factual reports and review findings

#### Independence test levels

* Independence is often more effective at finding defects and failures.
  * However, the developer can very efficiently find bugs in their own code.
* Applying a certain level of independence of the testing depends on the objective of testing

##### Independence levels

Levels lowest->highest:

* Test designed by the same person that wrote the code
* Test designed by another person from the same team(dev. colleague), but same organization
* Tests designed by a person from a different team (QA colleague), but same organization
* Test designed by a person from a different organization/company (outsourcing the testing)

##### Tips and tricks

* Be clear and objective

Confirm that:

* You have understood the requirements
* The person that has to fix the bug has understood the problem
