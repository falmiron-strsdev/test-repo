# Home Bot Dev System

A development and testing repository for the Home Bot worker pipeline.

---

## Overview

Home Bot Dev System is a test repository used to validate the worker pipeline infrastructure. It serves as a smoke-test target to verify that build, CI, and deployment workflows function correctly end-to-end.

- Worker pipeline success test passed.
- Lenovo worker smoke test passed.

---

## Prerequisites

- Git
- Access to the Home Bot CI/CD pipeline
- Appropriate repository permissions

---

## Setup / Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd home-bot-dev-system
   ```

2. Verify your environment is connected to the CI system — no additional dependencies are required for this test repository.

---

## Usage

This repository is primarily used to trigger and validate CI/CD pipeline runs.

- **Push to a branch** to trigger the worker pipeline.
- **Open a pull request** against `main` to run the full validation workflow.
- Review pipeline logs to confirm all smoke tests pass before merging.

---

## Troubleshooting

**Pipeline job does not trigger**
- Confirm that your branch is pushed to the remote and that CI webhooks are configured.

**Smoke test fails**
- Check the CI job logs for the specific error.
- Ensure the worker node has the correct permissions and network access.
- Re-run the job after confirming infrastructure is healthy.

**Unexpected merge conflicts**
- This repository is managed by an automated worker system. Pull the latest `main` before creating a new branch.
