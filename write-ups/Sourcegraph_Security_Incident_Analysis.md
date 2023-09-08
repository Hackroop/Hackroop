# Sourcegraph Security Incident Analysis
## Penetration Tester's Viewpoint

### Table of Contents
1. [Introduction](#introduction)
2. [Incident Overview](#incident-overview)
3. [Data Exposure](#data-exposure)
4. [Analysis](#analysis)
5. [Recommendations](#recommendations)

---

### Introduction
As a penetration tester, security incidents like the recent one at Sourcegraph offer valuable insights into potential vulnerabilities and the effectiveness of existing security measures. This document provides an analysis of the incident along with recommendations for avoiding similar occurrences in the future.

---

### Incident Overview
On August 30, 2023, Sourcegraph experienced a security breach. An unauthorized user gained admin access to Sourcegraph's public instance via a leaked admin token.


---

### Data Exposure
While no sensitive data such as passwords or private code was exposed, the attacker had access to some customer metadata:
- **Paid Customers**: License key recipients' names and email addresses.
- **Community Users**: Email addresses.

---

### Analysis
1. **Human Error**: The root cause was a human mistake, where an engineer committed a sensitive token to a public repository.
2. **Monitoring Gaps**: Sourcegraph detected the breach quite late, suggesting that their monitoring systems may need improvement.
3. **Swift Response**: After detecting the breach, Sourcegraph acted quickly to neutralize the threat.


---

### Recommendations
- Implement more stringent code review processes.
- Enhance monitoring systems to catch unauthorized admin-level activities.
- Conduct a full security audit to identify any other potential vulnerabilities.

:wq
