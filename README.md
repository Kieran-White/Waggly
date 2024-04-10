# Waggly Deployment Guide

This guide provides step-by-step instructions for deploying Waggly, a full-stack web application, utilizing AWS as its core controller. Waggly enables users to interact with a DynamoDB database through Python Lambda functions hosted on AWS Lambda. The application is fronted by an AWS API Gateway and managed using AWS Amplify.

## Prerequisites

Before deploying Waggly, ensure you have the following:

- An AWS account
- Basic knowledge of AWS services such as DynamoDB, Lambda, API Gateway, and Amplify
- Python environment set up for editing Lambda functions
- Access to Waggly's GitHub repository

## Deployment Steps

### 1. Set up DynamoDB Database

Create a DynamoDB database in your AWS account to store Waggly's data.

### 2. Deploy Lambda Functions

- Download all Python Lambda function files from the repository.
- Import each function into AWS Lambda.
- Set up the IAM inline policies for each function.
- Configure the connection within each function to connect to your DynamoDB database.

### 3. Configure API Gateway

Set up an AWS API Gateway and create a method for each Lambda function.

### 4. Frontend Setup

- Download the `index.zip` file from the GitHub repository.
- Edit the `index.js` file to include the correct ARN links for the API methods.
- Ensure the API methods are correctly mapped in the file.

### 5. Deploy with AWS Amplify

Create an AWS Amplify application and upload the modified `index.zip` file.
Follow the Amplify deployment process to deploy your application.

## Additional Notes

- Make sure to configure appropriate security measures for your AWS resources.
- Test the application thoroughly after deployment to ensure its functionality.
- Monitor your AWS resources for any potential issues or performance optimizations.
