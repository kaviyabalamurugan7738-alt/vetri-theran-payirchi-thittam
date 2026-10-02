# Streamlining IT Procurement – Automating Standard Laptop Orders with Flow Designer

## Project Overview

This project focuses on automating the standard laptop procurement process using **ServiceNow Flow Designer**.

The workflow automatically creates a Catalog Task after a Standard Laptop request is approved and assigns the task to the **Hardware** assignment group for laptop configuration.

## Problem Statement

The current IT procurement process involves manual work and delays when handling standard laptop orders. Configuration requirements can be overlooked or delayed, which increases user waiting time and creates inefficient resource allocation within the IT department.

## Project Objective

The main objectives of this project are:

* Provide a seamless experience for users requesting standard laptops.
* Reduce manual intervention and potential errors.
* Automatically assign configuration tasks to the Hardware team.
* Improve resource utilization within the IT department.
* Increase efficiency and productivity in IT procurement operations.

## Technologies Used

* ServiceNow
* Flow Designer
* Service Catalog
* Catalog Tasks
* ServiceNow Automation

## Workflow

The project follows this workflow:

**Standard Laptop Request**
↓
**Service Catalog**
↓
**Request Approval**
↓
**Flow Designer Trigger**
↓
**Create Catalog Task**
↓
**Assignment Group – Hardware**
↓
**Laptop Configuration**

## Flow Designer Configuration

### Flow Name

`Standard Laptop Task`

### Application

`Global`

### Run As

`System User`

### Trigger

`Service Catalog`

### Action

`Create Catalog Task`

### Catalog Task Configuration

**Short Description:**
`Laptop need to Configured`

**Description:**
`Laptop need to Configured`

**Assignment Group:**
`Hardware`

**Approval:**
`Approved`

## Service Catalog Configuration

The **Standard Laptop** service is configured under the Hardware category.

The created Flow is assigned to the Standard Laptop service through the **Process Engine** configuration.

## Implementation Steps

1. Open ServiceNow.
2. Open **Flow Designer**.
3. Create a new Flow.
4. Name the Flow **Standard Laptop Task**.
5. Set the application to **Global**.
6. Set Run As to **System User**.
7. Add a **Service Catalog** trigger.
8. Add the **Create Catalog Task** action.
9. Map the Requested Item Record.
10. Set the short description and description.
11. Set Assignment Group to **Hardware**.
12. Set Approval to **Approved**.
13. Save and Activate the Flow.
14. Open **Maintain Items**.
15. Select the **Standard Laptop** service.
16. Under Process Engine, add the created Flow.
17. Place a Standard Laptop order through Service Catalog.
18. Approve the request.
19. Open the Requested Item.
20. Check the Catalog Tasks section to verify the generated task.

## Expected Result

After the Standard Laptop request is approved, a Catalog Task is automatically created.

The task contains the required laptop configuration information and is assigned to the **Hardware** group.

## Conclusion

By automating the standard laptop procurement process using ServiceNow Flow Designer, manual overhead can be reduced and laptop configuration tasks can be generated and assigned automatically.

This workflow helps improve procurement efficiency, reduce user waiting time, optimize resource allocation, and provide a more streamlined IT procurement process.

## Project Documentation

The complete project documentation is available in:
[Streamlining IT Procurement - Automating Standard Laptop Orders with Flow Designer.pdf]

`Streamlining-IT-Procurement.pdf`
