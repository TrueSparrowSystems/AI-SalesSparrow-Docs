# Salesforce Configuration Guide

## Giving Permissions to Users

Configure Salesforce to give the necessary permissions to your Salesforce users for API access. API Only Users require specific configuration to access objects.

## Steps:

1. **Log in to Salesforce:**
   - Log in to your Salesforce account using your credentials.

2. **Navigate to Permission Sets:**
   - Click on the settings icon near the profile picture in the top right corner.
   - Select "Setup" from the dropdown menu.
   - In the search box, type "Permission Sets" and select it.

3. **Create a New Permission Set:**
   - Click the "New" button.
   - Fill in the required details:
     - **Label:** Give your permissions set a unique name.
     - **API Name:** This will be auto-filled based on the label.
     - **Description:** You can fill in the description.
   - Click on Save button

### Step 4: Configure Object Settings

1. **Navigate to the Permission Set Page**
   - After creating your new permission set, go to the permission set details page.
   
2. **Access Object Settings**
   - Under the **Apps** section, click on **Object Settings**.
   - You need to give permissions to Accounts, Contacts, Tasks, Users, and any other objects you want to access.
   
   #### For Accounts
   1. Click on **Accounts**
   2. Click the **Edit** button.
      - **Object Permissions:** Check the **Read** and **View All** checkboxes.      
   3. Click the **Save** button.

   #### For Contacts
   1. Click on **Contacts**
   2. Click the **Edit** button.
      - **Object Permissions:** Check the **Read** and **View All** checkboxes.
   3. Click the **Save** button.
   
   #### For Tasks
   1. Click on **Tasks**
   2. Click the **Edit** button.
      - **Object Permissions:** Check the **Read** and **View All** checkboxes.
   3. Click the **Save** button.

5. **Configure System Permissions:**
   - Under System, of the newly created permission set page, click on System Permsissions
   - Click on Edit button
      - **Edit Tasks:** Check the checkbox
      - **View All Data**: Check the checkbox
   - Click on Save button      

5. **Assign permission to Users:**
   - Click on the permission set you created
   - Click on Manage Assignments button
   - Click on Add Assignments button
   - Select the users you want to give permissions to
   - Click on Next button



# Add API only Users

You can add upto 5 API only users in your salesforce account. You can use these users to access the salesforce API. You can add these users by following the below steps:

1. **Log in to Salesforce:**
   Log in to your Salesforce account using your credentials.

2. **Navigate to Users:**
   - Click on the settings icon near the profile picture in the top right corner.
   - Select "Setup" from the dropdown menu.
   - In the search box, type "Users" and select it.

3. **Create a New User:**
   - Click the "New User" button.
   - Fill in the required details:
     - **First Name:** Give your user a first name.
     - **Last Name:** Give your user a last name.
     - **Email:** Give your user an email address.
     - **Username:** Give your user a unique username.
     - **Alias:** Give your user an alias.
     - **Role:** Select a role for your user. You can leave it as None specified.
     - **Profile:** Select a profile for your user. You can select Salesforce API Only System Integrations.
     - **User License:** Select "Salesforce Integration".
   - Click on Save button

4. **Give Permission Set License Assignments**
   - Click on the user you created
   - Click on Permission Set License Assignments
   - Click on Edit Assignments button
   - Enable the "Salesforce API Integration"
   - Click on Save button