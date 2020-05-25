![Pic](https://github.com/RedRockControls/SimpleUnitTestLibrary/blob/master/img/Banner.JPG)

# SimpleUnitTestLibrary

A lightweight unit test library for testing TwinCAT3 source code with the following goals:
1. Impose minimum setup cost for a new test
2. Provide a Gui to show test results
3. Support re-testing after an online change 
4. Support concurrent and sequential test execution


To create a test:
* Inherit from a base class
* Create an instance
* Call TestFinished()

To run all the tests together, call:

```plaintext
tcl_SimpleUnitTestLibrary.TestFramework.TestRunner(RunTestsSequentially := FALSE);
```
To run all the tests one after another, call: 
```plaintext
tcl_SimpleUnitTestLibrary.TestFramework.TestRunner(RunTestsSequentially := TRUE);
```