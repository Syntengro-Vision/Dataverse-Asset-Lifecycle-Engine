Automated Lifecycle & Compliance Engine
🚀 Overview
An enterprise-grade Asset Management system built on Microsoft Dataverse and Power Automate. This solution automates the Chain of Custody for hardware assets, ensuring audit readiness for CMMC Level 2 and NIST 800-171 standards.

🛠️ Key Technical Features
Automated Chain of Custody: Utilizing a N:1 relationship model, every asset assignment is logged into an immutable history table, capturing "Assignee," "Date Assigned," and "Date Returned."

State-Based Validation: Implemented Dataverse Business Rules to prevent "Ghost Assets" by locking assignment fields when hardware is marked as Retired or Disposed.

Self-Healing Data Logic: Power Automate "Auto-Return" workflows identify and close previous assignment records upon new user deployment, ensuring 100% data integrity for timestamps.

CUI Sanitization (The Janitor): Automated clearing of Controlled Unclassified Information (CUI) access flags and suppression of IT support tickets during maintenance windows.

📐 Logic Architecture
The system utilizes a Master Lifecycle Engine triggered by Dataverse row modifications.

Technical Specs:
Primary Table: cr42d_all_assets

History Table: cr42d_artemis_asset_assignments

Lookup Filtering: OData query logic using _value and null checks for high-performance record retrieval.

🛡️ Compliance Alignment (CMMC)
This engine directly addresses AC.L2-3.1.2 (Limit system access to authorized users) by maintaining an exact record of hardware custody and ensuring that retired assets are logically severed from user assignments.
