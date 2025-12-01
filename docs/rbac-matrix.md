
# KickPush Skate Co. – RBAC Access Matrix

This Role-Based Access Control (RBAC) matrix defines the standardized access model for users across the organization. Access is assigned based on department, job role, and least-privilege principles. All access is delivered through Entra ID security groups, allowing onboarding and role changes to be automated and auditable.

## Department Security Groups
- SG-Sales-Users  
- SG-Finance-Users  
- SG-Marketing-Users  
- SG-Engineering-Users  
- SG-Operations-Users  
- SG-IT-Users  
- SG-Executive-Users  
- SG-Privileged-Admins  

## Application Resource Groups (Example)
- APP-Sales-CRM  
- APP-Finance-ERP  
- APP-Engineering-Tools  
- APP-Marketing-SaaS  
- APP-Operations-SupplyChain  
- APP-Company-Intranet (All Users)

## RBAC Table (High-Level)

| Role / Department        | Base Access          | Apps & Resources                           | Privileged? |
|--------------------------|----------------------|---------------------------------------------|-------------|
| Sales Representative     | SG-Sales-Users       | APP-Sales-CRM, Intranet                     | No          |
| Sales Manager            | SG-Sales-Users       | APP-Sales-CRM, Intranet                     | No          |
| Finance Analyst          | SG-Finance-Users     | APP-Finance-ERP, Intranet                   | No          |
| Marketing Specialist     | SG-Marketing-Users   | APP-Marketing-SaaS, Intranet                | No          |
| Product Engineer         | SG-Engineering-Users | APP-Engineering-Tools, Intranet             | No          |
| Operations Coordinator   | SG-Operations-Users  | APP-Operations-SupplyChain, Intranet        | No          |
| IT Support Technician    | SG-IT-Users          | Intranet                                    | No          |
| System Administrator     | SG-IT-Users          | Intranet                                    | Yes (SG-Privileged-Admins) |
| Executive Leadership     | SG-Executive-Users   | Intranet, Selected SaaS apps                | No          |

## Notes
- Privileged roles must be manually approved and require MFA + Conditional Access restrictions.
- All access is granted through group assignment, not direct user-to-resource mapping.
- Changing an employee’s department automatically updates their access posture.
- Least privilege is enforced by ensuring each user receives only the groups tied to their role.

~

