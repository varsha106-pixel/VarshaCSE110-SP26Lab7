1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.
I would choose the second option: manually running tests locally before pushing the code. The Recipe project was split into distinct steps (A1–A11 for Expose, B1–B13 for Explore), so running tests after completing each chunk confirms that each part works correctly before moving on. This also makes it much easier to pinpoint exactly which step introduced a bug, rather than discovering issues late and having to trace back through many changes. Additionally, running tests manually gives fast, immediate feedback without the overhead of setting up a CI pipeline, which would be overkill for a solo project like this.
2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)
   No you would not. End to end testing is used for testing the entire flow of an app. You would use a unit test for this to test the output of a function.






