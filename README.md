# Oracle-internship
Loan Creation Based on the Debit balance in the EOD batch with Secure Pl/SOL Deployment Utility (Uses Java code)

**1. Title and Introduction**

# CASA EOD Loan Logic Refactor & PL/SQL Deployment Utility

This project addresses a critical logic flaw in the EOD (End of Day) batch process by refactoring the loan creation function to use the current balance instead of the available balance. It also introduces a robust PL/SQL deployment utility to automate, secure, and streamline all future database changes.

**2. Features**

Corrected Business Logic: The core loan creation logic was refactored to accurately assess an account's true balance, preventing incorrect loans and ensuring compliance.

Automated PL/SQL Deployment: A custom utility was developed to automate the deployment of all PL/SQL units (packages, functions, procedures).

Pre-Deployment Validations: The utility automatically performs Virus, Sonar, and Dependency scans on new code, ensuring security and quality.

Resilient Deployment with Rollback: A full backup of existing units is taken before deployment. In case of any compilation or deployment error, the utility automatically rolls back to the previous stable state.

Full Auditability: Upon successful deployment, the new code is automatically checked into Git, creating a permanent, version-controlled record of all changes.

