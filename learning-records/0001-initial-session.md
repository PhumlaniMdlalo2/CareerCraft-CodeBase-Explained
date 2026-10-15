# 0001 - Initial Session

## Date
2025-10-12

## Mission Alignment
Established mission: understand how backend is consumed and how everything connects in CareerWise (Spring Boot + Angular).

## What I Learned
- Backend follows layered architecture: Controller -> Service (interface+impl) -> Repository -> Domain
- REST endpoints under /api/* (jobs, applications, users, jobseekers, employers)
- Frontend uses Angular HttpClient with environment.apiBaseUrl to call backend; maps DTOs to UI models
- Auth flow: users login via /api/users/login, then enriches with role-specific profile (jobseeker/employer)
- Key flows: job search/display, apply for job, create job (employer), profile/resume
- State: Angular signals + localStorage for auth

## Key Insights
- Clear separation between backend contracts and frontend UI models
- Side effects (notifications) happen in service layer on state-changing operations
- Constructor injection used throughout services
- Cross-origin enabled for dev

## Zone of Proximal Development
Next logical step: deepen understanding of specific entities (relationships), error handling, validation, and potentially security/guards. Also could trace employer posting flow.

## Questions to Follow Up
- How are validations enforced (Bean Validation, custom exceptions)?
- How does GlobalExceptionHandler work?
- Are there auth tokens/JWT, or is it sessionless simple auth?
- How does file upload for resume work end-to-end (storage)?

## Lessons Created
- 0001-backend-basics-and-architecture.html
- 0002-api-endpoints-and-request-flow.html
- 0003-full-request-flow-example.html
- 0004-frontend-consumption-how-it-connects.html

## Reference Created
- quick-reference.html
