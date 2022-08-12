# CircleCI Pipeline Process

## Trigger

To start the deployment process, push new commits into the `master`-branch from the GitHub Repo that is linked with CircleCI.

## Build Process Steps

### 1. Install

- Installing Node on system
- Installing the front-end and then the back-end dependencies

### 2. Lint

- Lint the front-end code

### 3. Build

- Runs the build script for the front-end and then the back-end

## Manual Approval

After the build steps are successfully done, the pipeline process goes on hold and wait for manual approval.

If the building process failed, the deployment process ends till the building process completed successfully.

## Deployment Process Steps

### 1. Install

- Installing Node on system
- Installing and setup eb-cli & aws-cli

### 2.Deploy

- Deploy the back-end
  - Installing dependencies
  - Build
  - Set environment variables
  - Deploy with eb-cli
- Deploy the front-end
  - Installing dependencies
  - Build
  - deploy with aws-cli

## Workflow

1. Build
2. Manual approval after successful completed building process
3. Deploy
