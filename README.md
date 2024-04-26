# Greeting Web Application

## Overview
This web application allows users to enter their name in a form, then greets them by name and displays the number of times the greeting page has been viewed. This is a serverless application designed to run with AWS services.

## Features
- **Greeting by Name**: Users can enter their name to receive a personalized greeting.
- **View Counter**: Displays the number of times the greeting has been viewed.

## Technologies Used
- HTML/CSS/JavaScript for frontend.
- AWS Lambda and DynamoDB for backend operations.
- API Gateway for serverless endpoint.

## File Structure
- `index.html`: Contains the HTML structure of the greeting application.
- `style.css`: Provides the CSS styling for the application.
- `script.js`: Manages the frontend logic for greeting the user and updating the view counter.
- `lambda_function.py`: Handles the backend logic, interfacing with DynamoDB to manage view counts.

## Setup and Deployment
1. **Deploy AWS Resources**:
   - Set up a DynamoDB table named `serverless-webapp-table-av`.
   - Deploy the Lambda function from `lambda_function.py`.
   - Configure an API Gateway to trigger the Lambda function.

2. **Configure Frontend**:
   - Update the API endpoint in `script.js` to point to the deployed API Gateway URL.

3. **Run Locally**:
   - Open `index.html` in any web browser to view the application.

## Usage
- Enter your name in the form and click submit to see a personalized greeting and view count.

## Dependencies
- AWS SDK for Python (Boto3) for interacting with AWS services from the Lambda function.
- Modern web browser with JavaScript enabled for frontend interaction.

