---
title:      "Jest"
ring:       assess
quadrant:   languages-and-frameworks
tags:       [quality]
---

[Jest](https://jestjs.io/) is an open-source JS-based testing framework maintained by Facebook. 
It is designed to be easy to use and provides a comprehensive set of tools for writing end-to-end, integration, and unit tests for JavaScript applications. 
It is a complete and ready to set up JavaScript testing solution.

In the CHT, Jest is used to test [cht-interoperability](https://github.com/medic/cht-interoperability).

### Advantages
* Easy to use: Jest is intuitive and easy to set up, making it ideal for beginners and experienced developers.
* Extensive test coverage: Jest provides a complete set of tools for writing unit, integration, and end-to-end tests.
* Integration with other frameworks: Jest integrates well with projects that use React, but can also be used with other JavaScript frameworks (​​Babel, TypeScript, Node, React, Angular, Vue and more).
* Fast and efficient: Jest uses parallel test execution and other techniques to speed up test execution time.
* Provides testing support for asynchronous code.
* It is maintained and well-documented, making it easy to learn.
* Code Coverage: Jest provides built-in code coverage reports to help developers identify areas not covered by tests.

### Drawbacks
* Compared to Jasmine and other frameworks, not many libraries and toolings are supported by Jest.
* People not comfortable with the Jest framework have asserted that the learning curve is pretty hard.
* Leveraging auto-mocking can make tests slow. This is because the more dependencies a module has, the more work needs to be done by Jest to mock it, which comes at the cost of performance.
* Snapshot testing with Jest is not so feasible for larger snapshot files containing thousands of lines.
* Its debugging capabilities need improvement.

## Market - Current Adoption
Jest has over 10 million [dependent repos on GitHub](https://github.com/jestjs/jest/network/dependents).
Prominent companies that reportedly adopt Jest in their tech stack are: Facebook, Airbnb, Spotify, The New York Times, Travel Perk, Twitter, Instagram, etc.
[Stateofjs](https://stateofjs.com/en-us/) collects data from thousands of front-end developers in its annual surveys. 
[Here’s](https://2021.stateofjs.com/en-US/libraries/testing/) their most recent ranking of most popular JS testing frameworks, sorted by their usage and Jest is at the top 3.
