# AI-SDLC-APP-TEST-REPO

This repository is a sandbox for the Ticket Cockpit app. It gives the app a safe, disposable place to create branches, make commits, open pull requests, and exercise the development and deployment flow end to end without touching a real project. Changes here are expected to be experimental, so nothing in this repo should be treated as production code.

## Getting started

Run the project with Python 3:

```bash
python3 main.py
```

## Deployments

The repo has two GitHub Actions workflows:

- **`deploy-dev.yaml`**: runs on every push to `main`, deploying the latest code to the dev environment.
- **`promote-stage.yaml`**: runs by hand (`workflow_dispatch`), promoting the current build to the stage environment.
