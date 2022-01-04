# Test Automation Examples

## Types of software testing
There are many different types of software tests, each with specific objectives and strategies:<br/>
  <strong>- Acceptance testing:</strong> Verifying whether the whole system works as intended.<br/>
  <strong>- Integration testing:</strong> Ensuring that software components or functions operate together.<br/>
  <strong>- Unit testing:</strong> Validating that each software unit performs as expected. A unit is the smallest testable component of an application.<br>
  <strong>- Functional testing:</strong> Checking functions by emulating business scenarios, based on functional requirements. Black-box testing is a common way to verify functions.<br>
  <strong>- Performance testing:</strong> Testing how the software performs under different workloads. Load testing, for example, is used to evaluate performance under real-life load conditions.<br>
  <strong>- Regression testing:</strong> Checking whether new features break or degrade functionality. Sanity testing can be used to verify menus, functions and commands at the surface level, when there is no time for a full regression test.<br>
  <strong>- Stress testing:</strong> Testing how much strain the system can take before it fails. Considered to be a type of non-functional testing.<br>
  <strong>- Usability testing:</strong> Validating how well a customer can use a system or web application to complete a task.<br>
  
  In each case, validating base requirements is a critical assessment. Just as important, exploratory testing helps a tester or testing team uncover hard-to-predict scenarios and situations that can lead to software errors.

Even a simple application can be subject to a large number and variety of tests. A test management plan helps to prioritize which types of testing provide the most value – given available time and resources. Testing effectiveness is optimized by running the fewest number of tests to find the largest number of defects.

## What is Test Case? How to Write an Ideal Test Case?
Before explaining what the test case is, let's briefly talk about what software testing is and for what purpose it is done.

### What is Software Testing?
Software testing is the process of evaluating and verifying that a software product or application does what it is supposed to do. The benefits of testing include preventing bugs, reducing development costs and improving performance.

### Why is Software Testing Done?
The main purpose of the test is to detect an error that may occur later, to reduce costs by reducing costs, and to take faster action regarding the error.

In addition, it is to ensure that the product of the desired quality is offered to the customer, thus increasing customer satisfaction.

### What is Test Case?
Test cases are the documents that specify the inputs, events or actions prepared according to the requirements and the results expected to occur as a result of these. Test cases also enable to reveal the problems and deficiencies in the requirements and design that form the basis of the software.

Software testing should be done systematically within a plan. Software tests can be done by different people at different times. In order to provide a common standard in this, one or more test cases should be written for each function of the software and / or each request of the customer.

### About Test Case
• A basic test case body consists of expected and actual outputs versus inputs, although there may be differences according to needs.

• Error notifications are made by specifying the test case number and step. In this way, it is possible not to repeat the situation where the same error occurs within the team.

• Additions and changes are made in test cases over time. For this reason, it is necessary to follow up with a version number as in software.

• The scenario should have a purpose and a reference. You can create a traceability matrix over references. In this way, you can keep track of whether there are any open topics and which scenarios should be run on which topics.

• A common addressing style should be determined. Like “do it, do it” or “do it, it should be seen”.

### Required Fields in Test Case
<strong>Group (Suite):</strong> Related test cases should be in the same group. If a test case cannot be run without running the other test case, these test cases should be in the same group. <br/>
<strong>Test Case No:</strong> ID of the test case. <br/>
<strong>Use Case No: </strong> Which use case the test case is associated with.<br/>
<strong>Test Purpose or Title: </strong> A title about why the test case was written.<br/>
<strong>Prerequisites: </strong> Infrastructure, prerequisites required to perform the test. <br/>
<strong>Priority: </strong> The importance of the test case for the system. There is no specific standard of priority, but it is usually written as top priority: 1 – lowest priority: 4.  <br/>
<strong>Test Step No: </strong>Test step number.  <br/>
<strong>Inputs: </strong> What to do in the test step, what action to take.  <br/>
<strong>Test Data: </strong> The data to be used when performing the test.<br/>
<strong>Expected Outputs: </strong> Expected outputs as a result of inputs (operation performed).<br/>
<strong>Actual Outputs: </strong> Outputs encountered while testing.<br/>
<strong>Situation: </strong> There are generally three situations; Pass, Fail, Block (Unsuitable for Test).<br/>
<strong>Notes: </strong> Notes or screenshots of the test.<br/>
<strong>Error No (Bug ID): </strong> ID of the found bug.<br/>
<strong>Error: </strong>Description of the error found while running the test case. In which step of the test case an error is found, it should be written on that line.<br/>

You can see the test case example below.

### Determination of Test Cases
The multitude of models and the variety of input sets result in an infinite number of test cases. It is not possible to consider all of them individually due to time and money constraints. Therefore, testers have to develop strategies to create the most test coverage with the least scenarios. All lines of code must be run at least once and a test set covering all inputs must be used to complete the test process.

### Operation and Evaluation of Test Cases
After creating appropriate test sets, testers translate them into executable forms, resulting in scenarios that simulate the actions of a typical user.

The process of running tests can be facilitated by a variety of tools. In addition, it can be done automatically. However, evaluating the results of the tests is not as easy as the application of the tests. 

The evaluation process is a comparison process and is the mutual evaluation of the software test results and the outputs specified in the specification.

### You can see the test case example below.

| Group | Test Case No | Test Case Title                           | Priority | Test Step No | Inputs                                                                                                | Expected outputs                                                               | Test Data                              | Actual Outputs                                                                 | Status       |
|-------|--------------|-------------------------------------------|----------|--------------|-------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------|----------------------------------------|--------------------------------------------------------------------------------|--------------|
| 1     | 1            | Login to the system with a valid Username | 1        | 1            | A user name and password defined on the login screen are entered and the login button is pressed.     | Access to the main screen of the application is provided without any problems. | Username : testUser, Password : 123456 | Access to the main screen of the application is provided without any problems. | Successful   |
| 1     | 2            | Login with invalid username               | 1        | 1            | An invalid username and / or password is entered on the login screen and the login button is pressed. | The message "Username and/or password is incorrect" should be displayed.       | Username : testUser, Password : 111111 | Login to the main screen of the application.                                   | Unsuccessful |
