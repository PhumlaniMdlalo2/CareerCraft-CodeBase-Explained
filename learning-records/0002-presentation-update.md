# 0002 - Presentation Update

## Date
2025-10-12

## What Was Added
- 0005-auth-resume-notifications-errors.html: Covers auth flow (users + role profiles), resume upload/download, notifications (side effects), global error handling, route guards
- 0006-live-demo-checklist.html: Demo script, talking points, files to show, backup plan
- Updated quick-reference.html with notifications, resume, errors, guards, presentation must-shows

## Why
User needs comprehensive coverage for week presentation. Added missing pieces: resume handling, notifications as side effects, GlobalExceptionHandler, auth.guard/role.guard, and concrete demo checklist.

## Key Coverage for Presentation
- Auth: users/login + enrich with jobseeker/employer; localStorage; guards
- Resume: multipart POST/GET in JobSeekerController + frontend blob download
- Notifications: created in JobServiceImpl on new job, in ApplicationsServiceImpl on apply/status change
- Errors: GlobalExceptionHandler centralizes errors
- Full end-to-end demo with Network tab
