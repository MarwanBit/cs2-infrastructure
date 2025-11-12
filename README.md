# CS2 Match Predictor - Infrastructure Orchestration


# Project Overview

**cs2-match-predictor** is a Full-Stack application built on top of a End-to-End Machine Learning Pipeline which enables users to make and view predictions for upcoming cs2 matches, alongside viewing ML powered match prediction. It makes deep use of AWS services in order to regularly scrape and dump data into an PostgresSQL relational database, enabling regularly scheduled model training, served on a backend Django server.

# Tech Stack

* **Frontend:** React, NextJS, TailwindCSS, ShadcnUI, Clerk.
* **Backend:** Django, Python, BeautifulSoup, Scrapy, PostgresSQL, pyscopg2, Alembic, Poetry, Pandascore API, Pandas, Numpy, Tensorflow
* **Infrastructure:** Terraform, Docker, LocalStack, Amazon S3, Amazon VPC, Amazon EC2, Amazon Lambda Functions, Amazon CloudWatch, Amazon IAM Identity Center, Amazon API Gateway.
* **CI/CD:** Github Actions, Vercel Deployment.
* **Monitoring & Logging:** Prometheus + Grafana.
* **Testing:**  PyTest, Jest, react-testing-library, Cypress.
* **Documentation:** TypeDoc, PyDoc.

# Screenshots

[TBA]

# Quick Start

Checkout out [DEPLOYMENT.md](./docs/DEPLOYMENT.md) for instructions on how to simulate and run each of the microservices together.

# Documentation Links

#### Code Documentation

For code documentation checkout the **/docs** folder inside each individual microservice. Each microservice is resonsible for documenting their own functions and services.

#### Design Documentation

For design documentation checkout [ARCHITECTURE.md](./docs/ARCHITECTURE.md) which contains the high level system design for the project. For more detailed information about particular microservices and their design, checkout the **/docs** folder inside each individual microservice, which have their own **ARCHITECTURE.md** file.

# Testing

#### Unit and Integration Testing

For instructions on how to unit test each individual microservice checkout the **TESTING.md** file inside the corresponding microservices **/docs** folder. Each microservice documents how to perform unit tests.

#### End-To-End Testing with Cypress

We utilize Cypress for End-To-End Testing, to run cypress after deployment of the services make sure to run the following command.

```bash
npx cypress run
```

A terminal should appear running the individual tests with a resulting test coverage report, and test report after completion, make sure each of these tests pass before pushing or deploying (after changes).

For more detailed instructions on running the End-To-End testing suite, checkout [TESTING.md](./docs/TESTING.md).

# Deployment and Development

Deployment of the frontend is done using Vercel, for details on how to deploy the project to AWS/ production and how to work with the project locally, checkout out [DEPLOYMENT.md](./docs/DEPLOYMENT.md) and [DEVELOPMENT.md](./docs/DEVELOPMENT.md) for details on how to deploy to AWS, and locally respectively.
