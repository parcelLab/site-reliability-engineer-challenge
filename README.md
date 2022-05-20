
# parcelLab SRE challenge - “Hello World”

- Create a “Hello World” greetings service (REST-API) which responds with different salutations for customers (there won’t be further purpose for this API, just one GET endpoint is fine)
    - Customer A wants to say “Hi”, customer B wants to say “Dear Sir or Madam”, customer C wants to say “Moin” and so on. The system should identify users based on the salutation they send to the endpoint.
    - Choose whatever programming language and framework you think might be the best fit.
    - Describe and implement the necessary steps to ensure quality and security for your product.
- Create a build pipeline/script to create a docker image for this API and register it at a container registry (local registry is fine, a public registry like Github Packages or similar is a plus). Ideally put your scripts in a Makefile (or `package.json` if you decide to go with Node).
- Implement a deployment pipeline script which deploys the container to a kubernetes cluster (local is fine) and exposes endpoints
    - It must greet with “Hi there!” for customer A
    - It must greet with “Yours faithfully” for customer B
    - It must greet with "Moin moin!" for customer C
- Set up a CI system of your choice (for instance, Github Actions, Gitlab CI, CircleCI...). The CI should run at least with each push to the `main` branch.
    - It must run the tests for your application
    - It is a plus if it runs a linter and even better: it enforces the linter automatically
    - It is a plus if your CI builds and pushes the docker image to a public registry (e.g. Github Packages or Dockerhub)

## Our expectations

You might be wondering after reading the above scenario, how much effort and time we expect you to invest in this task. We know that you likely have a job, a life, further open job applications and other things that require some of your valuable time. Therefore you should **not** **spend more than** **5-6 hours** on this task (and we actually expect that this takes maximum 2 hours). If you feel, that you spend too much time on one topic, it is fine for us if you describe or comment, what you next steps would look like. The importan thing is to **document your ideas and approaches**. We value documentation as much as implementation.

## In the end you should have

- [ ]  a solution containing a Dockerfile and a script to build and register the docker image
- [ ]  a CI running when there is a push to the `main` branch
- [ ]  a documented script to deploy your solution to a (local) Kubernetes cluster
- [ ]  a README that explains how we could test the endpoints and deploy to the local cluster
- [ ]  a very simple automated test and linting rules

## What really makes us happy 😍

- [ ]  You provide us with a very extensive README.md that explains how we can build and deploy your solution, and any improvements that you might want to implement if you would have had more time.
- [ ]  Your code is well structured, clean and readable
- [ ]  You add comments and documentation in the code and docker image
- [ ]  You handle any common errors that could occur, and think about the security of your API endpoint
- [ ]  You extensively test your endpoint
- [ ]  You automatically format your code files based on a linter. As you might have expected, we value more the tooling regardingthe programming language of your choice than the actual implementation. There are no hidden traps in the implementation, it is simple for that reason.
