# CI/CD

- CI/CD is automated methodologies **that prepare, test, deliver, or deploy code** onto a servers
- **production** (prod) an environment which is intended to be used by paying users
- **staging** an environment which is intended to simulate a production environment for last stage debugging
- continuous integration (CI)
  - automating the review of developer's code
  - e.g. run test suites with a build server to e.g. codebuild
- continuous delivery (CD)
  - automating the prepration of the developer code for release
  - e.g. run test suites with a build server to e.g. codebuild and if tests pass create, pull requests or merge branch into staging
- continuous deployment (CD)
  - automatically deploying developers code which is ready for release
  - e.g. automatically merge pull requests with all tests passing and deploying into production
  - continuous deployment can refer to the entire pipeline e.g. codepipline using codecommit + codebuild + codedeploy
