 # Feature Flag Management System for Elisa Oyj
 
 > A scalable feature flag management system built through team collaboration, with the goal of improving release control, 
safety, and speed without heavy production deployment cycles.
> The solution follows the **OpenFeature standard** to support interoperable and vendor-neutral feature flag 
management. 
 > **Source code is private due to a client non-disclosure agreement (NDA).**

 ## Reference / Product Owner
 > "Great job! I'm looking forward to getting the Feature Flag system integrated into our services soon."
 > — **[Santeri Auvinen](https://www.linkedin.com/in/santeri-auvinen-7234552/)**, Product Owner at Elisa Oyj

 ## Project Background
 
 In Elisa’s environment, we needed a unified way to manage features across projects:
 - safe on/off switching of features
 - role-based access control
 - better visibility into which feature flag keys are actually used and what their status is
 
 To solve this, we built a system consisting of two parts:
 - **Backend** (Go): API, data model, authorization, integrations
 - **Frontend** (React + TypeScript): UI for managing projects and flags
 
 ## What the System Does
 
 The system enables:
 - project-scoped feature flag management
 - role-based permissions (**ADMIN / EDITOR / VIEWER**)
 - flag metadata, descriptions, and tagging
 - targeting rules, percentage rollouts, and progressive rollouts
 - automatic scanner integration that detects new/obsolete flags and marks outdated ones
 - relay/proxy use cases where applications fetch their own flag configuration by AppKey
 
 ## Architecture at a Glance
 
 - **Backend** provides an OpenAPI-based API, handles authorization, and stores data in PostgreSQL.
 - **Frontend UI** provides a clear management view for projects, flags, tags, and rule editing.
 - **Microsoft Entra integration** brings user/group-based permissions into the access model.
 - **Deployment** was done on **OpenShift (Kubernetes)**.
 - **CI/CD + testing** ensures quality at multiple levels (lint, unit, integration/application, BDD, frontend unit).
 
 ## Teamwork and Scrum
 
 The project was delivered as a team following **Scrum principles**:
 - sprint planning and backlog prioritization
 - dailies
 - sprint reviews and retrospectives
 - breaking work into specified tasks and continuously iterating based on feedback
 
 This workflow supported transparency, fast adaptation to change, and continuous improvement of technical solutions 
sprint by sprint.
 
 ## Why This Project Matters in My Portfolio
 
 This project represents how I approach software development:
 - I build solutions that work from both technical and business perspectives
 - I consider architecture, security, maintainability, and usability as a whole
 - I can work effectively in a cross-functional team and drive end-to-end delivery in sprint-based development
 
 ## Outcome
 
 The Feature Flag Management System introduced a unified operating model for feature flag governance and reduced 
release risk.  
 At the same time, it improved cross-project manageability, role-based security, and the team’s ability to deliver 
controlled, incremental releases.
