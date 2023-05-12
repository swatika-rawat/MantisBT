## MantisBT Custom Import 

When importing an external CSV file into MantisBT, the following fields are typically required:

- Summary: A brief description of the issue
- Description: A detailed description of the issue
- Category: The category to which the issue belongs (e.g. "Bug", "Feature Request", etc.) Examples include Documentation, Functionality, GUI, Installation, Performance, Security, Other
- Project: The project to which the issue belongs
- Priority: The priority of the issue (e.g. "High", "Medium", "Low", etc.) 
- Severity: The severity of the issue (e.g. "Critical", "Major", "Minor", etc.)  
- Status: The current status of the issue (e.g. "New", "Assigned", "Resolved", etc.)
- Reporter: The name or username of the person who reported the issue
- Assigned To: The name or username of the person who is responsible for resolving the issue
- Date Submitted: The date on which the issue was reported
- Last Updated: The date on which the issue was last updated
- view_state : Public or Private

When importing a CSV file into MantisBT, you should not choose the **“ID”** column as this is only used for updating existing bugs.

| CSV field | MantisBT field |
| ------ | ------ |
| Ticket Number | Summary |
| Issue Description | Description |
| Project/Dept Name | Category |
| Status | Status |
| Reason/Resolution | Resolution |
| Primary Contact From User (Name/Email/No.) | Additional Information (custom field) |
| Tech Support Team(Attended By) | Assigned To |
| Ticket Medium | Additional Information (custom field) |
| CUC/Cloud/NIC Coordinator (Name/email) | Additional Information (custom field) |
| Date/Received to CCC | Date Submitted |
| Remarks/External Issues (if any) | Additional Information (custom field) |
| OS Details | Additional Information (custom field) |

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
