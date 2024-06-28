# simple_flask

## Deployment Steps

### Step 1: Create Azure Web App

### Step 2: Configure Azure Web App

1. Once the Web App is created, navigate to the Web App's dashboard in the Azure Portal.
2. Go to "Deployment Center" under "Settings".
3. Click "Get publish profile" to download the publish profile.

### Step 3: Add GitHub Secret

1. Open the downloaded `.publishsettings` file with a text editor.
2. Copy the entire content of the file.
3. In your GitHub repository, go to "Settings" -> "Secrets" -> "Actions".
4. Click "New repository secret".
5. Name the secret `AZURE_WEBAPP_PUBLISH_PROFILE`.
6. Paste the content of the publish profile and save the secret.

### Step 4: GitHub Actions Workflow

Create a GitHub Actions workflow file in your repository at `.github/workflows/azure-webapp.yml` with the following content:

### Step 5: Commit and Push

### Step 6: Monitor Deployment

1. Go to the "Actions" tab in your GitHub repository to monitor the workflow execution.
2. Once the deployment is successful, navigate to your Azure Web App URL (e.g., `https://myflaskwebapp01.azurewebsites.net`) to verify that your application is running.

