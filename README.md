# sgd_control

In this repository, you can see my progress in creating and implementing a DMS (Document Management System). A manager who, in theory, should be able to manage the documentation that enters the company's workflow, classify it manually or automatically into a category, and apply the relevant retention list. I will keep the README updated. 

# Key Functionalities

1. Document Category Management

* Implements the complete retention schedule with codes, descriptions, and retention periods.

* Supports adding, updating, and querying document categories.

2. Automated Retention Processing

* Periodically checks documents that have reached their retention end date.

* Applies the required post-retention action:

    * Destroy (EL): Permanently deletes expired documents.

    * Archive (SAM/SEL, TNA): Moves documents to a secondary archive.

    * Permanent Preservation (PP): Transfers to a historical archive.

3. Employee Management

* Tracks document ownership with employee records (name, department, hire/termination dates).

* Links documents to their creators/owners for accountability.

4. Access Control & Audit Logging

* Logs all document interactions (view, download, edit) with timestamps.

* Tracks who accessed which documents and when.

5. Document Lifecycle Management

* Stores metadata (title, description, creation/modification dates, file path, format, size).

* Flags confidential documents with restricted access.

6. Search & Filtering

* Retrieves documents by:

    * Category (e.g., files for HR selection procedures).

    * Employee (e.g., all documents owned by a specific staff member).

7. Compliance Reporting

* Generates reports on retention actions (e.g., "X documents destroyed, Y archived this month").

* Provides audit trails for regulatory reviews.

8. Integration Readiness

* Designed to connect with:

    * Web interfaces (Flask/Django for user access).

    * Authentication systems (role-based permissions).

    * File storage (automated scans for new documents).
