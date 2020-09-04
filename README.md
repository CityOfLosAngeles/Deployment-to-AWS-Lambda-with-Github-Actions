# Deployment to AWS Lambda with Github Actions

This is a simplified example of deploying source code (with CI/CD as the intended use case) directly from a **git push** to AWS Lambda using GitHub Actions.

## How to Use

To implement this into a project, create a **.github/workflows** directory at the project's root and create a YAML file (of any name) within the new workflows folder. Configure that YAML file using the YAML file included in this sample repository as a guide.

As indicated in **.github/workflows/deploy-aws-s3-lambda.yaml**, secrets values must be added to the GitHub repository (via Settings > Secrets) to properly authenticate and permit AWS operations, as well as specify the Lambda function resource and S3 bucket (if applicable).

## To-Do

* Verify functionality of deployment via S3 bucket