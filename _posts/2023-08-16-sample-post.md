---
layout: post
title: "The Keys to Effective Software Testing: Test Cases, Test Plans, and Test Runs"
date: 2023-08-16
---

# Test Cases, Test Plans, and Test Runs

Efficient testing of the software under test is a vital part of making sure that any company delivers a high-quality product. Software quality should always be a collaborative effort at every stage of the life cycle within a business, but the QA function also needs to be organised, efficient, and certain that the basics are understood and being executed effectively. 

In this post, I'll take a look at three key concepts in modern software testing - test cases, test plans, and test runs. We'll take a quick look at whay they are, and, crucially, why they are important. 

## Test Cases

A test case is a set of steps and conditions that will help determine if a particular feature or function of an application is working as expected.

In simple terms, a test case is a recipe that clearly defines the ingredients (inputs) and steps (actions) needed to produce the dish.

If you're looking for an industry definition, then you might often see a test case described as:

> a set of conditions through which a tester will ascertain whether an application, software, or feature, is working as intended/expected.

A test case should outline (**Note**: not all of these are "*requirements*" of a well-written test case):

- A clearly defined title
- A description (a more verbose description of what the test case covers)
- Any preconditions (requirements or necessary setup that needs to happen before the test case can be run)
- Relevant test data (any data that the test will need to perform the step)
- Expected results (what should happen when each step is followed?)
- Type of test (Functional, Smoke, Regression, Performance, etc)

It's not unusual to see additional information included in an in-depth test case. As an example, some test case management software might allow a creator to specifiy if the test case is automated or outline if it's a blocker to a release path.

The steps from a highly simplified test case could look like this:

| Step | Data | Expected Result |
| -----|------|-----------------|
| 1. Navigate to the login page |  | The login page should be displayed. Email address and password fields should be visible. A Login button should be visible. |
| 2. Enter an email address associated with an active account | petergriffin@example.com | |
| 3. Enter a password that is not associated with the entered email address | P@ssw0rd | | 
| 4. Click Login | | An inline error message should be displayed. No navigation should occur. The user should not gain access to the platofrm. | 

#### Why Test Cases Matter

Test cases bring a sense of calm and clarity to the world of testing. Ad-hoc and exploratory testing are, by their very nature, sporadic and largely non-uniform. Well-written test cases bring calm to the chaos and are important because they:

- Provide a clear procedure to follow to verify functionality.
- Can be repeated consistently across testing cycles.
- Can be understood and verfified by non-testing members of a team.
- Help identify new defects and regressions as the software changes.
- Give visibility into what has and hasn't been tested.
- Provide clear expectations of what needs to be test and what needs to be achieved.
- Give confidence that all aspects of the software/feature have been understood and considered. 

## Test Plans

A test plan outlines the scope, objectives, timeline, resources, and activities for a specific testing project. It serves as a guide for QA teams to execute testing in an organized way.

To go back to our cooking analogy, a test plan, again, is like a recipe for how to test a software application. It outlines all the different "ingredients" needed to do thorough testing.

Key elements of a test plan include:

Scope - This defines what features, components, and integrations will be tested. For example, a test plan scope could include:

- New user registration flows
- Payment processing module
- Integration with third-party billing system

Objectives - The goals and measures of success for testing. Examples:

- Uncover subsystem defects before public launch
- Validate new features meet specified requirements
- Achieve 90% test case coverage for core workflows

Timeline - The schedule for testing tasks and milestones. For instance:

- September - Complete regression testing
- October - Execute integration testing
- November - Start UAT across all subsystems
- December - Final validation 1 week before launch

Resources - Testing tools, environments, and team members. Such as:

- QA testing team (John, Sarah, Kevin)
- Staging environment and test data
- Testing tools like Selenium, JMeter

Activities - The types of testing and test design techniques to use. Examples:

- Functionality - Write exploratory, boundary, usability test cases
- Performance - Load and stress testing with 600+ concurrent users
- Security - OWASP top 10 vulnerability scans

#### Why Test Plans Matter

Test plans are great for organising and optimising software testing efforts. A well-constructed test plan outlines the goals, scope, timeline, resources, and activities needed to thoroughly validate that software meets requirements and provides a magical user experience. Without a test plan, testing can become fragmented and incomplete.

A good test plan helps testers do their job the right way. It's like having a map (who remembers maps?) so they don't get lost along the way. The test plan starts by saying what needs to be tested. This focuses efforts on the most important parts of the software. Like only baking the cake and not all the side dishes.

The plan also sets timelines for testing tasks. This keeps things moving forward at a good pace. Testers don't waste time choosing what to do next. The plan lists any tools, data, and people needed for testing. Making sure testers have what they need to find issues. No digging around for ingredients! 

Finally, the plan names different types of testing to do. Checking different aspects like security, performance, and usability. Not just the same thing over and over. With their route mapped out, testers can test efficiently and cover everything that needs to be covered to provide quality assurances. When testers follow the plan, the whole team can be confident in releasing quality software that works well.

## Test Runs

A test run is the fun part! It's the actual execution of a test case or set of test cases against the software under test. The same test cases can be executed repeatedly across multiple test runs.

During a test run, the steps outlined in each test case are followed, comparing the expected and actual results to find defects and anomalies. Details like test data, environment, and logs are recorded to help debug issues. 

#### Why Test Runs Matter

Performing test runs is critical for:

- Validating that new code/features work as intended.
- Catching bugs and identifying areas for improvement. Executing test cases can often uncover usability issues in an app.
- Providing confidence in the quality of the product or feature before release.
- Generating data to measure progress over successive runs.
