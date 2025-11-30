# KickPush IAM Lifecycle Automation Lab

A hands-on identity governance and lifecycle automation project designed to simulate how real organizations manage identities at scale using Microsoft Entra ID and PowerShell. This lab reflects the type of IAM engineering work I want to master: designing access models, automating user lifecycle tasks, implementing MFA and Conditional Access, and documenting identity governance decisions with clarity and structure.

This project is part of my transition from an IAM-heavy technical support role into a dedicated Identity and Access Management engineer position. I built this lab to deepen my understanding of identity lifecycle flows and to practice architecting a full IAM environment from scratch.

---

## Project Overview

Organizations often struggle with inconsistent onboarding, excessive privilege, manual account management, and unclear access logic.  
The KickPush lab addresses those challenges through:

- Automated user provisioning
- Department-based RBAC
- MFA and Conditional Access enforcement
- Privileged access workflows
- Documentation of identity governance decisions
- Clear identity architecture diagrams
- Realistic IAM test scenarios

This environment simulates a 500-employee company called KickPush Skate Co. with departments such as Sales, Finance, Marketing, Warehouse, IT, and Executive Leadership.

---

## Architecture

Identity architecture includes:

- Microsoft Entra ID tenant
- Department-based RBAC security groups
- Privileged Access Group (SG-Privileged-Admins)
- Conditional Access policies enforcing MFA
- Zero Trust-aligned identity controls
- Break-glass administrative account
- PowerShell-driven lifecycle automation

An identity architecture diagram will be added to illustrate user flows, RBAC relationships, Conditional Access logic, and privileged access separation.

---

## Repository Structure


---

## Automation Features

### Automated User Provisioning (PowerShell)
- Bulk creation of users from CSV
- Automatic assignment to department-based RBAC groups
- Job title, department, and location attributes set on creation
- Logging of lifecycle actions for audit and review

### RBAC Enforcement
- Security groups for each department
- Least privilege alignment
- Standardized entitlements that support automation and governance

### Conditional Access and MFA
- Tenant-wide MFA enforcement
- Conditional Access policies for risky sign-ins
- Restrictions on legacy authentication
- Privileged access policies for admin accounts

### Privileged Access Workflow (In Progress)
- Dedicated privileged access group
- Controlled membership process
- Documentation of approval flows
- Planned automation for request/approval simulation

---

## Test Scenarios

This project includes realistic IAM test cases, including:

- New Hire Provisioning: create a user from CSV and validate RBAC assignment
- Role Change: transition a user between departments
- Termination: deprovision access within a defined SLA
- Privileged Access Attempt: validate Conditional Access and MFA restrictions
- Break-Glass Scenario: confirm emergency administrative account behavior

Screenshots and documentation for these cases will be added to the repository.

---

## What I Have Learned (Ongoing)

This section will expand as the project develops. Current insights include:

- RBAC design must be clearly defined before automation can be effective
- PowerShell automation significantly improves lifecycle consistency
- Conditional Access requires careful planning to avoid unintended lockouts
- Identity governance relies heavily on documentation, not just scripting

More lessons will be added as the project continues.

---

## Contact

For questions or discussion related to Identity and Access Management, automation, Entra ID, or identity governance, feel free to reach out. I am actively building my IAM engineering skillset and open to collaboration and professional conversation.

