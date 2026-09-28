# Accessibility Baseline & Repository Architecture Audit

## Project Overview

This repository contains the accessibility audit and repository architecture
skeleton for Task 02.

The project uses a monorepo-style structure to keep the frontend, backend,
documentation, tests, and accessibility audit evidence organized in one
repository.

## Repository Structure

task-02-accessibility-audit/
├── client/
│   ├── src/
│   └── README.md
├── server/
│   ├── src/
│   └── README.md
├── docs/
├── tests/
├── audit/
│   ├── screenshots/
│   └── accessibility-audit.csv
└── README.md


## Architecture Boundaries

### Client

The `client/` directory contains the frontend application.

Responsibilities:

* User interface and presentation
* Client-side navigation
* Form interactions
* Accessibility implementation
* Communication with backend APIs

### Server

The `server/` directory contains the backend application.

Responsibilities:

* API endpoints
* Business logic
* Data validation
* Communication with data storage
* Server-side error handling

### Docs

The `docs/` directory contains project documentation, design notes,
architecture decisions, and supporting documentation.

### Tests

The `tests/` directory contains automated and manual test documentation.

### Audit

The `audit/` directory contains accessibility audit results and supporting
evidence.

The `accessibility-audit.csv` file records identified accessibility issues,
their WCAG references, evidence, severity, impact, and recommended fixes.

The `screenshots/` directory contains screenshots supporting the audit
findings.

## Local Setup

### Prerequisites

* Git
* Node.js
* npm

### Setup

Clone the repository and enter the project directory:

git clone <repository-url>
cd task-02-accessibility-audit


Install dependencies after the client and server applications are initialized.

Start the client and server applications using their respective development
commands.

## First Vertical Feature Slice

The first vertical feature slice will be a basic service-information flow.

A user will be able to:

1. Open the client application.
2. View available service information.
3. Select a service.
4. Submit a basic request through the frontend.
5. Send the request to the server API.
6. Receive a validated response from the server.
7. Display the result accessibly to the user.

The feature will cross the client and server boundaries while keeping
presentation, business logic, and API responsibilities separated.

## Accessibility Audit

The public-facing website selected for the accessibility audit is the
Tamil Nadu e-Sevai Citizen Portal.

The audit combines:

* Lighthouse accessibility testing
* Keyboard-only navigation testing
* WCAG references
* Screenshot evidence
* Recommended remediation

The detailed findings are available in:

`audit/accessibility-audit.csv`

## Status

* [x] Accessibility audit completed
* [x] Audit evidence screenshots collected
* [x] Audit CSV completed
* [x] Repository skeleton created
* [x] Client/server boundaries documented
* [ ] Application implementation
* [ ] Automated tests