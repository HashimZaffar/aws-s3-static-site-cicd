# Static Website Deployment to AWS S3 with GitHub Actions

This project deploys a static website to Amazon S3 and automatically updates the live site whenever changes are pushed to the `main` branch on GitHub.

## Tech Stack

- Ubuntu 24.04.3 LTS
- AWS S3
- AWS CLI
- Git and GitHub
- GitHub Actions

## Project Structure

- `index.html` — homepage
- `error.html` — error page
- `.github/workflows/deploy.yml` — CI/CD workflow for deployment

## How It Works

1. Website files are stored in this GitHub repository.
2. A GitHub Actions workflow runs on every push to `main`.
3. The workflow authenticates to AWS using GitHub Secrets.
4. The workflow syncs website files to the S3 bucket.
5. The live website updates automatically.

## Live Website

S3 bucket website endpoint:

```text
http://myusername-devops-website-2026.s3-website-us-east-1.amazonaws.com
