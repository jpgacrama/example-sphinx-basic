=========================================
Workflow Engine
Technical Specifications Document
=========================================

---

Version History
===============

+------------+-------------+------------------------------------+-----------------------------+
| **Date**   | **Version** | **Changes**                        | **Authors**                 |
+============+=============+====================================+=============================+
| 2024-10-03 | 1.0         | Initial draft                      | Jonas Gacrama               |
|            |             |                                    | Eydrin John De Vera         |
+------------+-------------+------------------------------------+-----------------------------+

---

Initiative Background
======================

Problem Statement
-----------------

In modern enterprise systems, business processes often involve complex and dynamic workflows with multiple decision points, approvals, and dependencies across various teams or systems. If all business logic is hardcoded into the source code, this approach can lead to several challenges:

- **Limited Flexibility**: Hardcoding business logic requires modifying and redeploying the application whenever these rules change, making the system less agile in responding to evolving requirements.
- **Scalability Issues**: As workflows grow in complexity, managing them within the source code can become increasingly difficult, leading to bloated codebases and dependencies.
- **Error-Prone Updates**: Updating hardcoded business logic increases the risk of bugs and inconsistent behavior across the system.
- **Lack of Transparency and Monitoring**: Hardcoded workflows often lack visibility, making it hard for non-technical stakeholders to monitor or track progress.
- **Complex Maintenance**: Managing multiple workflows entangled within the source code increases the complexity of maintenance, making the system harder to scale or extend.

Unique Selling Point
--------------------

Using a **workflow engine** separates workflow management from core application logic. This externalization leads to:

- Increased flexibility to modify workflows without redeployments.
- Scalability, allowing for complex workflows to be added or modified dynamically.
- Enhanced monitoring and transparency for both technical and non-technical stakeholders.
- Simpler maintenance of the codebase with better modularity and a reduced risk of introducing bugs during updates.

Proposed Solution
-----------------

A **Workflow Engine** is proposed to address these challenges by:

- Enabling dynamic updates to business logic without redeployment.
- Improving scalability, allowing the system to handle more complex workflows without bloating the codebase.
- Offering better monitoring and visibility tools, providing insights into the workflow execution process and bottlenecks.
- Providing a cleaner separation between business logic and code, making the system easier to maintain and extend.

Metrics
=======

Change Management Efficiency
----------------------------

- **Average Time to Implement Workflow Changes**:
  - Measures the average duration required to implement changes in workflows. Shorter times indicate a more agile and responsive system.
- **Number of Hotfixes Post-Workflow Changes**:
  - Tracks the frequency of urgent fixes required after deploying workflow changes. A lower number suggests better initial quality and stability of workflow implementations.

System Flexibility and Scalability
----------------------------------

- **Time to Deploy New Workflows**:
  - Assesses how long it takes to deploy new workflows into the system. Faster deployment times indicate a more flexible system capable of adapting quickly to business needs.
- **Number of New Workflows Deployed Without System Downtime**:
  - Counts the number of workflows deployed without causing interruptions to the system's operations. A higher number reflects better scalability and reliability.

Codebase Maintainability
------------------------

- **Lines of Code (LoC) Reduction**:
  - Measures the decrease in lines of code due to the implementation of a workflow engine. A reduction suggests improved maintainability and simpler code structure.
- **Code Complexity (Cyclomatic Complexity)**:
  - Evaluates the complexity of the codebase by measuring the number of linearly independent paths through the code. Lower complexity indicates easier maintenance and fewer bugs.

Operational Efficiency
----------------------

- **Error Rate in Workflow Execution**:
  - Calculates the frequency of errors occurring during workflow execution. A lower error rate suggests more reliable and efficient workflows.
- **Mean Time to Resolve (MTTR) Workflow Issues**:
  - Measures the average time taken to resolve issues that arise within workflows. Shorter MTTR indicates a more responsive support system.
- **Throughput of Workflow Processes**:
  - Assesses the number of workflows processed in a given timeframe. Higher throughput reflects better efficiency and productivity.

Monitoring and Visibility
-------------------------

- **Percentage of Workflow Processes Monitored**:
  - Indicates the proportion of workflows that are actively monitored for performance and issues. A higher percentage means better oversight and control.
- **Average Time to Detect Workflow Bottlenecks**:
  - Measures the time taken to identify slowdowns or issues in workflow processes. Quicker detection times lead to faster resolutions and improved performance.

Stakeholder Autonomy
--------------------

- **Percentage of Workflow Changes Handled by Non-Developers**:
  - Tracks the proportion of workflow changes that can be made by non-technical staff. A higher percentage indicates greater empowerment and autonomy for stakeholders.
- **Reduction in Developer Hours for Workflow Changes**:
  - Assesses the decrease in developer time required for making workflow changes. Less reliance on developers suggests a more user-friendly system.

System Performance
------------------

- **Workflow Latency**:
  - Measures the delay between initiating a workflow and its completion. Lower latency indicates a more efficient and responsive system.
- **System Resource Usage During Workflow Execution**:
  - Monitors the amount of system resources (CPU, memory, etc.) consumed during workflow execution. Optimal usage reflects a well-optimized system.

Compliance and Auditability
---------------------------

- **Percentage of Workflows with Full Audit Trails**:
  - Evaluates the proportion of workflows that maintain complete records of their execution for compliance purposes. A higher percentage indicates better accountability.
- **Number of Compliance Violations Due to Workflow Errors**:
  - Tracks the frequency of compliance violations resulting from workflow issues. Fewer violations suggest a more compliant and reliable system.

User Satisfaction
-----------------

- **User Satisfaction Score (Internal Users)**:
  - Measures the satisfaction level of internal users with the workflow system. Higher scores indicate better usability and effectiveness.
- **Feedback on Workflow Change Requests**:
  - Collects qualitative and quantitative feedback on requests for workflow changes. Positive feedback reflects the system's ability to meet user needs and expectations.

Detailed Workflow Designs
=========================

See the following pages for detailed workflow designs:

- `Account Opening <./AccountOpening.rst>`_
- `Cash Deposit <#cash-deposit>`_
- `Check Deposit <./CheckDeposit.rst>`_
