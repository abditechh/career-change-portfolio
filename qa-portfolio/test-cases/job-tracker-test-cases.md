# Job Application Tracker — Test Cases

| ID | Area | Scenario | Steps | Expected result | Priority |
|---|---|---|---|---|---|
| JT-001 | Registration | Create an account with valid details | Enter a new email and valid password; select **Create Account** | Account is created and the authenticated application view opens | High |
| JT-002 | Registration | Attempt registration with an invalid email | Enter an invalid email format and a password; select **Create Account** | Registration is rejected and a useful error appears | High |
| JT-003 | Login | Log in with valid credentials | Enter registered credentials; select **Login** | User sees only their own application data | Critical |
| JT-004 | Login | Log in with the wrong password | Enter a registered email and incorrect password | Access is refused without exposing sensitive information | High |
| JT-005 | Create | Add a complete application | Enter date, company, role, contact, status and notes; save | A new row appears with the entered information | High |
| JT-006 | Create | Save with required information missing | Leave company or role empty; save | Application is not saved and the missing field is explained | High |
| JT-007 | Search | Search by company name | Add multiple records; enter part of one company name | Only matching records are shown | Medium |
| JT-008 | Filter | Filter by interview status | Create records with different statuses; select **Interview** | Only interview records are shown | Medium |
| JT-009 | Update | Edit an existing record | Change the role or status and save | The correct record updates and persists after refresh | High |
| JT-010 | Delete | Delete a record | Select delete on an existing record and confirm | Correct record is removed and remains deleted after refresh | High |
| JT-011 | Security | Confirm user data isolation | Create data in account A; log into account B | Account B cannot read or alter account A's records | Critical |
| JT-012 | Export | Export visible data to CSV | Create records and select **Export CSV** | Valid CSV downloads with correct headings and values | Medium |
| JT-013 | Notes | Store a job-posting URL | Add an HTTPS URL to notes and save | URL is displayed safely and opens in a new tab | Medium |
| JT-014 | Responsive UI | Use application on a narrow mobile screen | Open at approximately 375 px width and use core actions | Content remains usable without hidden controls or unreadable text | Medium |

## Regression checklist

- Registration, login and logout work.
- Every user sees only their own records.
- Add, edit and delete persist after refresh.
- Dashboard counts match the table.
- Search and status filters work together.
- Links in notes are safely encoded.
- CSV export preserves special characters.
- Core workflows remain usable on phone and desktop.
