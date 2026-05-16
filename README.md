1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.
I would choose the second option: manually running tests locally before pushing the code. The Recipe project was split into distinct steps (A1–A11 for Expose, B1–B13 for Explore), so running tests after completing each chunk confirms that each part works correctly before moving on. This also makes it much easier to pinpoint exactly which step introduced a bug, rather than discovering issues late and having to trace back through many changes. Additionally, running tests manually gives fast, immediate feedback without the overhead of setting up a CI pipeline, which would be overkill for a solo project like this.
2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)
   No you would not. End to end testing is used for testing the entire flow of an app. You would use a unit test for this to test the output of a function.

3) What is the difference between navigation and snapshot mode?
   The difference between navigation and snapshot mode is navigation mode analyzes a page right after it loads and gives performance metrics like load time and JavaScript execution but it can't analyze user interactions or dynamic content changes. Snapshot mode analyzes the page in its current state at a single moment in time, making it better for finding accessibility issues, but it can't measure JS performance or track changes to the DOM.
4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.
   1) We could add a lang attribute to the html element. Missing the lang attribute hurts accessibility for screen readers and users in different locales resulting in the accesibility score of 90.
   2) We could add a meta description. The page has no <meta name="description"> tag, which is what dropped the SEO score to 91.
   3)  We could implement a Content Security Policy. Lighthouse flagged several security items under Best Practices, including no CSP to guard against XSS attacks and no HSTS policy. Adding security headers would strengthen the site's trust and safety posture.




