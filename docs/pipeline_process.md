# Pipeline Process

The service used in pipeline process is `CircleCi`. It connects to `GitHub` repos and detects changes and triggers the pipeline to deploy the new code.

### CircleCi Orbs

- circleci/node@5.0.2
- circleci/aws-elastic-beanstalk@2.0.1
- circleci/aws-cli@3.1.1

### Pipeline Jobs

- Install Front-End Dependencies through the command `npm run frontend:install`
- Install API Dependencies through the command `npm run api:install`
- Front-End Lint through the command `npm run frontend:lint`
- Front-End Build through the command `npm run frontend:build`
- API Build through the command `npm run api:build`
- Deploy App through the command `npm run deploy`

### Pipeline Workflows

- **build:**
  - Spin up environment
  - Prepare environment variables
  - Install Node.js
  - Checkout code
  - Install Front-End Dependencies
  - Install API Dependencies
  - Front-End Lint
  - Front-End Build
  - API Build
- **hold:** (requires approval)
- **deploy:**
  - Spin up environment
  - Prepare environment variables
  - Install Node.js
  - Set up Elastic Beanstalk CLI
  - Install AWS CLI
  - Configure AWS Access Key ID
  - Checkout code
  - Deploy App
