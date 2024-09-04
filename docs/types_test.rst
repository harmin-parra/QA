=============
TYPES OF TEST
=============

Installation test
=================

**What:**

Test the installation on the target OS/hardware architecture.

Test the initial configuration of the system (if applicable).

**Who:** Tester.

Update test
===========

**What:** Test the system update from N-1 version to N version.

**Who:** Tester.

Unit test
=========

**What:**

Low level test to verify small pieces of code.
The typical usage of unit test is to verify the methods of a class.

Some unit testing frameworks:

+----------------------+----------------------+---------------------+
| Programming language | Unit test frameworks | Assertion libraries |
+======================+======================+=====================+
| Java                 | * JUnit              |                     |
|                      | * TestNG             |                     |
+----------------------+----------------------+---------------------+
| Python               | * Unittest           |                     |
|                      | * Pytest             |                     |
+----------------------+----------------------+---------------------+
| .Net                 | * NUnit              |                     |
|                      | * xUnit.net          |                     |
+----------------------+----------------------+---------------------+
| Node.js              | * Jest               | * Chai              |
|                      | * Mocha              | * Assert.js         |
|                      | * Jasmine            |                     |
|                      | * Karma              |                     |
+----------------------+----------------------+---------------------+

**Who:** Developers.

Component/Contract test
=======================

**What:**

Verify a component works properly in isolation or with mocked integration to other components.

Components generate integrate to each other through Soap/Rest APIs or asynchronous messaging (ActiveMQ, Kafka).

Contract testing consist in mocking such endpoints to verify both consumers and providers.

**Who:** Developers.

Integration test
================

**What:**

Verify that any pair of components work together properly when communicating with each other.

If the given pair needs in turn to communicate with other components, such communications will be mocked (see contract testing).

**Who:** Developers.

API test
========

**What:**

Can be seen as a subset of integration test.

An API is verified with all components or a subset of components fully integrated.

It allows testing the business rules while bypassing integration with one or more components (example: testing business rules without using the GUI).

**Who:**

Developers in the case of deep intra-module/intra-component APIs. (same as contract testing)
Testers in case of external APIs.

System test
===========

**What:**

Verify that entire system, with the complete and fully integrated components, works properly.
Also know as end-to-end test.

**Who:** Tester.

Functional test
===============

**What:**

Positive tests
--------------

- Verify that a functionality works as expected/specified.

- Verify the nominal case and alternative valid cases.

Negative / Error handling tests
-------------------------------

Verify the system handles error cases and displays proper error messages.

Boundary-value test
-------------------

Verify both valid and invalid boundary values for a given functionality.

**Who:**

Developers at a microcosmic level (unit, contract testing).
Tester at a macrocosmic level (e2e testing, external API testing).

Security test
=============

**What:**

Authentication
--------------

Verify that only known and activated users can get access to the system.

Authorization (Access Control)
------------------------------

Verify that users can only access ressources according to their roles/profiles.

Pentest
-------

In-depth security and intrusion tests.

The choice of the web development framework is paramount. Several of them (e.g., Laravel, Next.js, Spring Boot, Django, Ruby on Rails, .Net, etc) provide out-of-the-box security features to protect web applications against vulnerabilities like SQL injection, cross-site scripting, cross-site request forgery, and broken authentication, among others.

⚠️ Special attention needs to be paid on software external components:

Pick well-known external components.

Update external components regularly to avoid outdated and vulnerable versions of such components.

⚠️ The so-called “technical debt” needs to be avoided.

**Who:**

Developer at a microcosmic level (unit, contract testing).
Tester at a macrocosmic level (e2e testing, API testing).

Acceptance test
===============

**What:**

Verify software correctness (functional requirements are implemented according to the
specifications).

Verify technical requirements (Performance, load, stress).

**Who:** Tester and Product Owner

Usability test
==============

**What:** Verify whether the application is user-friendly.

**Who:** Tester and Product Owner

Localization test
=================

**What:** Verify software behavior for specific locations, regions and countries (time zone, language, currency, etc).

**Who:**

Developer at a microcosmic level (unit, contract testing).
Tester at a macrocosmic level (e2e testing, API testing).

Compatibility test
==================

**What:** Verify the software works properly across different operating systems, browser and devices.

**Who:** Tester.

