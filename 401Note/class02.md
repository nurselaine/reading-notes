## Class02 Reading: Express, NPM, TDD, CI/CD

#### [An introduction to NodeJS and Express](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)
1. Explain middleware, answer as though I were a non-technical recruiter.
  - middleware in express are functions that help to modify the request and response objects. Middleware is used in the server when the client sends a request and before sending a response back to the client
2. Express the most popular **Node web framework**
3. Express is “unopinionated.” What does that mean?
  - unopinionated frameworks like express have less restrictions on how to build components making it easier for developers to use tools to achieve a task
4. What is a module and why is modularity useful to us as developers?
  - a module is a library or file that can be imported into main code 
  - Express is a module because it's a library which is required into server
  Modularity is good because it keeps code compartmentalized and organized. It sorts code by common themes which makes code easier to clearn, refactor, and understand

#### [What is NPM](https://docs.npmjs.com/getting-started/what-is-npm)
1. What version of npm are you running on your machine?
  - currently running v8.12.1
2. What command would you type to install a library/package called ‘jshint’ into your node project?
  - npm i <library> or npm install <library>


#### [What is TDD?](https://www.agilealliance.org/glossary/tdd/)

1. Explain why tests are important. Please explain as though I were your non technical elder.
  - Whenever you teach something, a good way to check if it was learned is through testing! Just like teaching, validating a coding program is best done through a test. Sometimes it's nice to make the test before you teach/write the program. It's like having a set of requirments before creating the content 
2. What are three expected benefits of testing
  - Less defects/bugs 
  - smoother final project phase
  - improved design qualities and internal/technical improvement
3. Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.
  - writing tests that are too details or too broad
  - not runnning tests enough
  - Not everyone runs tests on the team
  - poor maintenance of tests


#### [CI/CD](https://www.youtube.com/watch?v=xSv_m3KhUO8)

1. What are three benefits of Continuous Integration?
2. What is the difference between Continuos Delivery and Continuous Deployment?
3. Explain how GitHub fits into this process assuming the listener comes from a non-technical background

## Good reference links 
[HTTP status codes](https://www.restapitutorial.com/httpstatuscodes.html)
[Supertest](https://github.com/visionmedia/supertest)

docs
- [nodejs](https://nodejs.org/en/docs/)
- [NPM](https://docs.npmjs.com/)
- [Express](https://expressjs.com/en/4x/api.html)