
# parcelLab SRE challenge - “Hello World”

- Create a “Hello World” greetings service (REST-API) which responds with different salutations for customers (there won’t be further purpose for this API, just one GET endpoint is fine)
    - Customer A wants to say “Hi”, customer B wants to say “Dear Sir or Madam”, customer C wants to say “Moin” and so on.
    - Choose whatever programming language and framework you think might be the best fit
    - Describe or implement the necessary things to ensure “good quality“ for your product
- Create a build pipeline/script to create a docker image for this API and register it at a container registry (local registry is fine)
- Implement a deployment pipeline script which deploys the container to a kubernetes cluster (local is fine) and exposes endpoints
    - your application should greet with “Hi” on the service for customer A
    - your application should greet with “Dear Sir or Madam” on the service for customer B
    - your application is deployed for each customer individually

## Our expectations

You might be wondering after reading the above scenario, how much effort and time we expect you to invest in this task. We know that you likely have a job, a life, further open job applications and other things that require some of your valuable time. Therefore you should **not** **spend more than** **5-6 hours** on this task. If you feel, that you spend too much time on one topic, it is fine for us if you describe or comment, what you next steps would look like. 

## In the end you should have

- [ ]  a solution containing a Dockerfile and a script to build and register the docker image
- [ ]  a pipeline script to deploy your solution to a (local) Kubernetes cluster
- [ ]  a short description how we could test the endpoints

## What really makes us happy 😍

- [ ]  You provide us with a README.md that explains how we can build and deploy your solution
- [ ]  Your code is well structured, clean and readable
- [ ]  You add comments and documentation
- [ ]  You handle any common errors that could occur
- [ ]  You use automated tests where appropriate