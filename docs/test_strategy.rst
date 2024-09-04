=============
TEST STRATEGY
=============

INTRODUCTION
============

The test strategy is a plan that outlines the test approach, goals, scope, processes, resources and timelines.

Intended Audience
-----------------

- Chief Technical Officer
- Product Owner
- Product Manager
- Software Architect
- Developers
- Testers

Document Review and Approval
----------------------------

The present Test Strategy document shall be reviewed and approved by:

- Chief Technical Officer
- Product Owner

Project Background
------------------

``TODO`` Short description of the project

TEST OBJECTIVES
===============

Software testing aims at improving software quality.
The main broad objectives of software testing are:

- Bug detection.
- Verification of software correctness (functionalities).
- Verification of technical requirements.
- Assess software usability.

TEST APPROACH
=============

Processes
---------

Description of the main QA processes that take place within the Agile/Scrum-Master framework.

**User-Story specification phase**

- Definition of user-story acceptance tests.

**User-Story development phase**

- Specification of user-story passing tests.
- Specification of user-story non-passing tests.
- Specification of test scenarios involving the user-story and other functionalities.

**User-Story validation phase**

- Execution of exploratory tests.
- Execution of user-story passing & non-passing tests.
- Bug reporting (if any).
- Verification of fixed bugs (if any).

**User-Story post-validation phase**

- Development of automated tests.
- Execution of test scenarios.
- Execution of non-regression tests.
- Bug reporting (if any).
- Verification of fixed bugs (if any).

**Software release phase**

- Definition of test scope (Ideally full non-regression).
- Creation of test campaign.
- Execution of test campaign.
- Bug reporting (if any).
- Verification of fixed bugs (if any).
- Go/No-Go decision.
- Reporting of test campaign results.

Roles and Responsibilities
--------------------------

``TODO``

Types of test
-------------

`Types of Test </en/latest/types_test.html>`_

:doc:`types_test`

Data Set Strategy
-----------------

It can any one of the followings:

- The software is installed with an empty database and a data injector creates the data set.
- An anonymized copy of the production database is used as baseline of the test data set.
- An anonymized copy of the production database is used followed by the creation of additional data if the production copy lacks prerequisite data for some test cases.

In case that an anonymized copy of the production database is used, it is necessary to define the frequency or the criteria to update such database copy.

TEST DELIVERABLES
=================

Test deliverables refer to a list of documents, tools, and other tangible artifacts that must be created, provided, and maintained to support testing activities in a project.
A different set of deliverables is required before, during and after testing.

**Deliverables before test execution**

- Conception and specification of test cases for newly developed user-stories/functionalities.
- Conception of persistent standard data and pseudo-random test data for test environments.
- Creation of test campaign.

**Deliverables during test execution**

- Creation/Update of automation test scripts.
- Update of data injector utility (if any).
- Execution of manual and automated tests.
- Update tests execution status in test campaign.
- Creation/Update of bug tickets.

**Deliverables after test execution**

- Test execution report (for both manual and automated tests).
- List of created bug tickets.

EXIT CRITERIA
=============

Exit criteria is the set of conditions for permitting the test campaign to be officially completed.

The outcome of the test campaign can be either positive or negative, decided in a Go/No-Go meeting between the stakeholders.

If the outcome is considered to be positive, the release candidate under test can be deployed in production. Otherwise, more development would be required to make the software more stable and a new test campaign should restart.

The Go/No-Go meeting will be held after the test campaign has been finished.

A test campaign is considered to be finished when the following tasks have been completed:

- Creation of the test campaign in the test management software.
- Execution of the entire test campaign.
- Documentation of all bugs detected during the test campaign in the bug tracker.
- Fix and verification of all critical and blocking bugs detected during the test campaign execution
- Go/No-Go meeting in which a decision needs to be made on whether the current open bugs are acceptable for the software to be delivered or deployed in production.

The final decision taken in the Go/No-Go meeting is the responsibility of the Product Officer and Product Manager.

TEST TOOLS
==========

``TODO``

TEST AUTOMATION INFRASTRUCTURE
==============================

``TODO``

TEST ENVIRONMENTS
=================

``TODO``
