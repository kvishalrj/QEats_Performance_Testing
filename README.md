# QEats Performance Testing

## Overview
**QEats** is a food delivery application, and the purpose of this project is to monitor the performance of the application under high load and ensure it meets expected benchmark metrics.

### Project Highlights:
- Wrote and executed **JMeter** tests to validate the **happy flow** of the application under various load conditions.
- Tested the application under different **load scenarios** to evaluate business metrics and application performance.
- Used **SigNoz** for monitoring the host machine's metrics where the test-bed was set up, ensuring comprehensive visibility of the system’s health during tests.
- Focused on performance validation for critical application functionalities, ensuring they could handle expected user traffic without degradation in performance.
- Provided insights into system behavior under load, identifying areas for performance optimization.

## Tools and Technologies Used:
- **JMeter**
- **SigNoz**
- **Postman**

## Project Structure:
The project is organized into the following modules:

1. **JMeter Test Scripts**:
   - Contains the test scripts that simulate various user activities and actions on the QEats application to test its performance under load.
   - Includes tests for user login, placing orders, browsing menu items, and checking order statuses.

2. **Performance Metrics**:
   - In-depth performance metrics collected from **SigNoz** to track resource utilization and system health during the tests.
   - Host machine metrics (CPU, memory, network) monitored throughout the test runs to provide a full picture of performance.

3. **Test Execution Reports**:
   - Contains the results of each test, providing detailed logs, performance graphs, and insights into how the application performed under various conditions.

4. **Postman Collections**:
   - A collection of **Postman** API tests used for validating backend API performance and response times, providing a comprehensive view of the application's behavior under load.

## Features Implemented:
- **Load Testing**:
  - Simulated different load scenarios with varying numbers of concurrent users to measure response times, throughput, and system stability.
- **Performance Monitoring**:
  - Integrated with **SigNoz** to monitor system health and resource usage during the tests.
- **Business Metrics Testing**:
  - Validated critical business metrics like order placement time, browsing response time, and transaction processing under load.
- **Test Results Reporting**:
  - Detailed test execution reports, including **response times**, **throughput**, and **error rates** under various load conditions.
- **Scalability Validation**:
  - Ensured the system could scale under increasing traffic loads and meet expected service levels.

## How to Run:
1. Clone the repository:
   ```bash
   git clone https://github.com/kvishalrj/QEats_Performance_Testing.git
   ```
2. Ensure **JMeter** and **SigNoz** are installed and configured.
3. Import the JMeter test plan into **JMeter** for executing the load tests.
4. Run the tests and observe performance metrics in **SigNoz**.

### Running Tests:
#### Using JMeter:
- Open the JMeter test plan (`.jmx` file) in **JMeter**.
- Configure the number of threads (virtual users) to simulate various load scenarios.
- Run the tests and analyze the results in the **Summary Report** and **Graphs**.

#### Monitoring Performance with SigNoz:
- Access the **SigNoz** dashboard to monitor host machine metrics in real time while tests are running.
- Review the metrics to identify potential bottlenecks and areas of improvement.

## Reporting:
After the test run, detailed reports are generated:
- **Performance Graphs**: Found in the `reports/` directory, showing metrics like response times, throughput, and errors.
- **Test Logs**: Detailed logs for each test, including timestamps and actions performed.
- **System Metrics**: Collected data on CPU, memory, and network usage during test execution, available through **SigNoz**.

## Future Scope:
- Enhance test coverage to include stress and spike testing scenarios.
- Integrate performance tests with CI/CD pipelines to continuously validate performance with every code change.
- Optimize performance based on identified bottlenecks and resource consumption patterns.
