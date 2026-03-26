# TA-Website
This repository contains the public-facing TrialAmicus marketing website.

## Purpose
The website is used to:
- present the TrialAmicus brand
- explain the product and value proposition
- capture pilot interest and contact inquiries
- direct users to the product application

## Domain
Production domain:
- https://trialamicus.com

## Scope
This repository should contain:
- landing page
- product overview pages (V-Reg page)
- company/about content
- contact or pilot interest forms
- public navigation and branding assets

## Out of Scope
This repository should NOT contain:
- product application logic
- user authentication flows for the app
- study workspaces
- document ingestion logic
- AI backend logic

## Tech Stack
- Next.js / React
- TypeScript
- Tailwind CSS

## Notes
This repo is intentionally separated from the product application so that marketing changes and product changes can be developed and deployed independently.
2. trialamicus-app
Repo purpose

Frontend application for actual TrialAmicus users.

Suggested README
# TrialAmicus App

This repository contains the frontend application for the TrialAmicus platform.

## Purpose
The application is used by:
- Clinical Research Coordinators (CRCs)
- Clinical Research Associates (CRAs)
- Project Managers (PMs)
- Sponsor / CRO study teams

## Domain
Production domain:
- https://trialamicus.io
or
- https://app.trialamicus.io

## Scope
This repository should contain:
- login and authenticated user flows
- study workspace UI
- document intake portal
- question and answer interface
- citations display
- role-aware user experiences
- product dashboards and settings

## Out of Scope
This repository should NOT contain:
- public marketing pages
- backend API logic
- infrastructure-as-code
- raw AI model orchestration

## Tech Stack
- Next.js / React
- TypeScript
- Tailwind CSS

## Notes
This repo is the core product interface and should remain separate from the public website for cleaner deployment and development workflows.
3. trialamicus-backend
Repo purpose

Backend services and AI orchestration for TrialAmicus.

Suggested README
# TrialAmicus Backend

This repository contains the backend services that power the TrialAmicus application.

## Purpose
The backend is responsible for:
- study and user APIs
- document ingestion workflows
- document parsing and chunking
- retrieval and citation logic
- AI answer generation
- protocol intelligence extraction
- database interactions

## Scope
This repository should contain:
- REST API endpoints
- document upload processing
- integration with S3, PostgreSQL, and vector storage
- retrieval-augmented generation (RAG) logic
- answer generation with source citations
- audit and usage logging

## Out of Scope
This repository should NOT contain:
- public marketing website code
- frontend application UI code
- infrastructure provisioning scripts

## Tech Stack
- Python
- FastAPI
- PostgreSQL
- pgvector
- AWS S3
- OpenAI / Anthropic / Bedrock integrations

## Notes
This repo is the intelligence and application logic layer of TrialAmicus. It should remain clearly separated from the frontend repos.
4. trialamicus-infra
Repo purpose

Infrastructure, environments, deployment, and cloud configuration.

Suggested README
# TrialAmicus Infrastructure

This repository contains infrastructure and environment configuration for TrialAmicus.

## Purpose
This repo is used to manage:
- AWS environment configuration
- development and production infrastructure
- deployment configuration
- networking and storage setup
- domain and DNS documentation
- environment-level architecture references

## Scope
This repository should contain:
- infrastructure-as-code (if used)
- environment configuration for dev and prod
- AWS setup documentation
- S3 / RDS / ECS / Cognito references
- deployment notes for trialamicus.com and trialamicus.io

## Environments
- Management
- Development
- Production

## Domains
- trialamicus.com → marketing website
- trialamicus.io → product application

## Out of Scope
This repository should NOT contain:
- frontend product code
- website code
- backend business logic

## Notes
This repo should remain focused on cloud infrastructure and deployment concerns only. Application logic belongs in the frontend and backend repositories.
Optional short repo descriptions for GitHub

These are the one-line descriptions you can put under each repo name.

trialamicus-website

Public marketing website for TrialAmicus.

trialamicus-app

Frontend application for TrialAmicus users and study teams.

trialamicus-backend

Backend APIs, document ingestion, and AI orchestration for TrialAmicus.

trialamicus-infra

AWS infrastructure and deployment configuration for TrialAmicus.

My recommendation for branch discipline

Once the repos are created, set this simple rule:

main = stable branch
feature branches for all new work
no direct pushes to main unless absolutely necessary

That alone will save you pain later.

If you want, I can next provide the exact first folder structure inside each repo so your CTO and engineer can initialize them cleanly.
