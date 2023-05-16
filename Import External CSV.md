## MantisBT Custom Import 

When importing an external CSV file into MantisBT, the following fields are typically required:

- Summary: A brief description of the issue
- Description: A detailed description of the issue
- Category: The category to which the issue belongs (e.g. "Bug", "Feature Request", etc.) Examples include Documentation, Functionality, GUI, Installation, Performance, Security, Other
- Project: The project to which the issue belongs
- Priority: The priority of the issue (e.g. "none", "low", "normal","high", "urgent", "immediate", etc.) 
- Severity: The severity of the issue (e.g. "feature", "trivial", "tweak","minor", "major", "crash", "block" etc.)  
- Status: The current status of the issue (e.g. "new", "feedback", "acknowledged", "confirmed", "assigned", "resolved", "closed")
- Reporter: The name or username of the person who reported the issue
- Assigned To: The name or username of the person who is responsible for resolving the issue
- Date Submitted: The date on which the issue was reported
- Last Updated: The date on which the issue was last updated
- Resolution: Includes the following values ("open","fixed","reopened")


When importing a CSV file into MantisBT, you should not choose the **“ID”** column as this is only used for updating existing bugs.

| CSV field | MantisBT field |
| ------ | ------ |
| Ticket Number | Ticket Number (Custom Field) |
| Issue Description | Description |
| Project/Dept Name | Project Name (Custom Field) |
| Status | Status |
| Reason/Resolution | Reason/Resolution (Custom Field) |
| Primary Contact From User (Name/Email/No.) | Primary Contact From User (Name/Email/No.) (Custom field) |
| Tech Support Team(Attended By) | Assigned To |
| Ticket Medium | Ticket Medium (Custom field) |
| CUC/Cloud/NIC Coordinator (Name/email) | CUC/Cloud/NIC Coordinator (Name/email) (Custom field) |
| Date/Received to CCC | Date Submitted |
| Remarks/External Issues (if any) | Summary |
| OS Details | OS |

Here is the suggested mapping of your CSV fields to the fields in MantisBT:

Based on the fields in your CSV, here are some suggestions for custom fields in MantisBT and their data types:

| field | Data Type |
| ------ | ------ |
| Primary Contact Name |  Text Field |
| Primary Contact Email |  Email Field |
| Primary Contact Number |  Text Field |
| Tech Support Team | User Field (to link to the user account of the support team member)|
| Ticket Medium | Enumeration Field (with values Phone, Email, Web, etc.)|
| CUC/Cloud/NIC Coordinator Name | Text Field|
| CUC/Cloud/NIC Coordinator Email | Email Field |
| Reason/Resolution | Text Field |
| Remarks/External Issues | Text Field |
| Viewstate | Text Field |

