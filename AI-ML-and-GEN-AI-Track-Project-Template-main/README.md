# Import Data using Transform Maps (Spreadsheet) & Visual Analytics

**Program:** TN Skills (Vetri Thiran Payirchi Thittam)  
**Track:** ServiceNow Certified System Administrator (CSA)  
**Team ID:** SWTID-2026-7960  
**Team Members:** 
* Parvathi P (Team Lead)
* Yuvasri T
* Manjula K
* Kalaiyarasi K
* Jayalakshmi S

---

## **Repository Structure**

This repository is structured phase-by-phase according to the project development lifecycle:

1. **Brainstorming & Ideation**
   * *Deliverables:* Problem statement analysis, customer journey mapping, and empathy mapping for automated enterprise data imports.

2. **Requirement Analysis**
   * *Deliverables:* Functional and Non-Functional Requirements (FR/NFR), data flow diagrams, and external interface specifications.

3. **Project Design Phase**
   * *Deliverables:* Solution architecture diagrams, technology stack selection, and Problem-Solution Fit Canvas.

4. **Project Planning Phase**
   * *Deliverables:* Project proposal report, resource allocation, milestone timelines, and task distribution among team members.

5. **Project Development Phase**
   * *Deliverables:* 
     * Spreadsheet preparation (`Sample Spreadsheet.xlsx`)
     * Custom target table creation (`u_employee_test`)
     * Staging import set configuration (`u_employee_import`)
     * Table Transform Map setup with **Coalesce** enabled on `u_employee_id` to prevent duplicate records.

6. **Project Testing**
   * *Deliverables:* Data validation logs, transform history execution records, and target table inspection reports confirming successful batch processing of records.

7. **Project Documentation**
   * *Deliverables:* Comprehensive project documentation templates covering solution architecture, execution steps, scalability plans, and component descriptions.

8. **Project Demonstration**
   * *Deliverables:* Team demo planning schedule, individual member contributions, employee analytics dashboard configuration, and presentation walkthrough links.

---

## **Project Overview**
This project demonstrates an end-to-end data integration workflow within the ServiceNow platform. Raw employee records from external spreadsheets are ingested into a staging import set table and accurately transformed into a custom production table using Table Transform Maps. To ensure enterprise reliability, the **Coalesce** feature is configured on the `u_employee_id` field to intelligently update existing records instead of creating redundant duplicates during repeated imports. Additionally, an interactive **Employee Analytics Dashboard** was built using the Platform Analytics Workspace to deliver real-time visual insights.

---

## **Getting Started & Execution Guide**

1. **Access Instance:** Log into your ServiceNow Personal Developer Instance (PDI).
2. **Load Data:** Navigate to **Load Data** and upload the sample spreadsheet (`Sample Spreadsheet.xlsx`) targeting the staging table (`u_employee_import`).
3. **Configure Transform Map:** Create a Table Transform Map, map source fields to target table fields, and set **Coalesce = true** on `u_employee_id`.
4. **Transform & Verify:** Run the transformation and verify successful record population in the `u_employee_test` table.
5. **View Dashboard:** Open the **Employee Analytics Dashboard** under Self-Service to review active reports and charts.

---