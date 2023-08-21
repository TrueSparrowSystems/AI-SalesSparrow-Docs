# Creating a Connected App on Salesforce

A connected app in Salesforce allows external applications to integrate securely with your Salesforce org. This guide will walk you through the process of creating a connected app.

## Steps:

1. **Log in to Salesforce:**
   Log in to your Salesforce account using your credentials.

2. **Navigate to App Manager:**
   - Click on the settings icon near the profile picture in the top right corner.
   - Select "Setup" from the dropdown menu.
   - In the search box, type "App Manager" and select it.

3. **Create a New Connected App:**
   - Click the "New Connected App" button.
   - Fill in the required details:
     - **Connected App Name:** Give your app a unique name.
     - **API Name:** This will be auto-filled based on the app name.
     - **Contact Email:** Enter an email address for notifications.
   - Under "API (Enable OAuth Settings)", check the box for "Enable OAuth Settings".
   - Check the "Enable for Device Flow" checkbox.

4. **Configure OAuth Settings:**
   - In the "Callback URL" field, provide the URL where Salesforce will redirect after authentication.
      - **Whitelisted Callback URLs For SalesSparrow:** `salessparrowdev://oauth/success` and `salessparrow://oauth/success`.
   - In the "Selected OAuth Scopes" section, choose the required scopes based on your integration needs.
      - **Scopes for SalesSparrow:**
         - Manage user data via APIs (api)
         - Perform requests at any time (refresh_token, offline_access)
         - Access unique user identifiers (openid)
   - Check the "Require Secret for Web Server Flow" checkbox.
   - Check the "Require Secret for Refresh Token Flow" checkbox.

5. **Save the Connected App:**
   - Click the "Save" button at the bottom of the page.

6. **Retrieve Consumer Key and Secret:**
   - After saving the connected app, you'll be redirected to its details page.
   - Note down the "Consumer Key" (also known as Client ID) and "Consumer Secret" (also known as Client Secret). These will be used for authentication from your external app.

For more detailed information, you can refer to the official Salesforce documentation on connected apps [here](#https://help.salesforce.com/s/articleView?id=sf.connected_app_create.htm&type=5).
