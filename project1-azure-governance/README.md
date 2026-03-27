# Project: E-Commerce Web App Infrastructure
## Overview
This project manages the Azure resources for the development environment of the new e-commerce web application. It ensures a centralized location for all related services and enforces access control for the dev and test teams.

## Access Control (RBAC)
Access is managed at the Resource Group level:

Developers: Assigned the Contributor role for full resource management.

Testers: Assigned the Reader and Virtual Machine Contributor roles.

## Deployment Instructions
To recreate or update this environment:

Log in to the Azure Portal.

Ensure you are in the [Your-Subscription-Name] subscription.


## Naming & Tagging
Environment: Dev

Department: IT-Ecom

Naming Convention: [resource-type]-[app-name]-[env]-[region]