📘 Project Overview
This project focuses on load testing the Restful Booker API to evaluate its performance under stress. It simulates high user traffic, validates response stability, and ensures system reliability under load. The testing process is automated using Jenkins, and performance metrics are visualized using HTML reports.

🔍 Objective
-Measure API response times, throughput, and error rates under varying loads.

-Simulate multiple users accessing and performing operations simultaneously.

-Identify performance bottlenecks and ensure API scalability.

-Integrate load tests into a CI/CD pipeline for automated, repeatable execution.

-Generate detailed HTML reports for test result analysis.

🧪 Load Testing Approach
-Load test scripts are created to simulate real-world usage scenarios such as:

-User login (authentication)

-Booking creation (POST)

-Booking retrieval (GET)

-Booking update (PUT/PATCH)

-Booking deletion (DELETE)

-Tests are designed with configurable parameters like thread count, ramp-up time, and loop duration.

-Authentication tokens are dynamically generated and reused during test execution.

⚙️ Jenkins Integration
-Load test execution is fully automated through Jenkins pipelines.

-Jenkins fetches the latest test scripts from the repository, executes them, and publishes the results.

A Jenkinsfile defines the stages for:

-Running the load tests

-Generating and archiving HTML reports

-Integration ensures consistent performance testing in every build cycle or scheduled job.

📊 HTML Report Generation
-After every test run, HTML reports are generated for visualizing key performance metrics:

-Response times (min, max, average)

-Request success/failure rates

-Active threads over time

-Throughput and latency trends

-Reports help QA teams and developers interpret load test results quickly and effectively.

✅ Benefits
-Automation: Zero manual effort after initial setup; tests run automatically with each commit/build.

-Scalability Testing: Confirms how well the API scales with increased traffic.

-Early Feedback: Quick detection of performance regressions or slow endpoints.

-CI/CD Alignment: Fits seamlessly into Agile workflows and DevOps pipelines.

-Reporting: Easy-to-read visual reports for decision-making and optimization.

