# Job Application Tracker

A small web application I built to organise my job applications and keep the information available on my phone and computer.

## Features

- Email/password registration and login
- Private application records per authenticated user
- Add, edit and delete applications
- Track pending, interview, accepted and rejected statuses
- Search by company, role or email
- Filter by status
- Dashboard totals
- Export records as CSV
- Safe rendering of notes and job-posting links

## Technologies

- HTML
- CSS
- JavaScript
- Firebase Authentication
- Cloud Firestore

## Why I built it

I wanted a practical tool to help with my own career change. Building it gave me a reason to practise HTML, CSS, JavaScript and Firebase. I am now using it to learn how to write test cases, find problems and improve a project step by step.

## Quality and security checks

- Confirm Firestore rules restrict every user to `users/{uid}/applications` for their own UID.
- Test registration, login, logout and session changes.
- Test required-field validation before public release.
- Test CSV escaping with commas, quotes and new lines.
- Test add, update and delete persistence after refresh.
- Test mobile layouts and long content.

## Current status

This is a beginner's learning project and it still needs improvement. I will document problems honestly instead of presenting it as finished professional software.

## Screenshot

Add a screenshot here before publishing:

```markdown
![Job Application Tracker dashboard](docs/job-tracker-dashboard.png)
```
