# Locksmith & Son's

## Scenario

All customer contact is handled through a central helpdesk. Trained operatives receive incoming calls and process them as follows:

1. If the caller is not an existing customer, a new Customer record is created.
2. An Incident is logged against the customer to capture the reported issue.
3. Flow automation monitors incidents for repeated problems of the same category occurring at the same address. When a pattern is detected, the automation escalates the related incidents into a Problem record for root cause investigation and resolution.
4. Planned maintenance and upgrade work is handled separately through Change Management, ensuring scheduled work follows a controlled approval and implementation process.

## Tables and Artifacts

The activity makes use of the following ServiceNow tables and artifacts:

- **Customer** (custom table): stores customer contact and address details.
- **Incident**: records individual reported issues linked to a customer.
- **Problem**: created via flow automation when repeated incidents share category and address; used to track root cause and permanent fix.
- **Change Request**: used for planned maintenance and system or service upgrades, including approval and scheduling.
- **Flow Designer flow(s)**: automation logic for detecting repeated incidents and generating associated Problem records.

## Purpose

This repository is intended for training purposes only. The company, its operations, and all associated data are fictional and used solely to illustrate ServiceNow application development and process automation concepts.
