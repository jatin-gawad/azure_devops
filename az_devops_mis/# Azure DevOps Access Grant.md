# Azure DevOps Access Grant for Peter

This document outlines the step-by-step process for granting Peter access to Azure DevOps with "Basic + Test" access level, adding him to the "test" project, and assigning him as an administrator for that project.

---

## Step 1: Add Peter to Your Azure DevOps Organization and Assign "Basic + Test" Access Level

1.  **Navigate to your Azure DevOps Organization:**
    * Open your web browser and go to `dev.azure.com/[YourOrganizationName]`.
    * *(Replace `[YourOrganizationName]` with the actual name of your Azure DevOps organization.)*

2.  **Go to Organization Settings:**
    * In the bottom-left corner of the page, click on **Organization settings**.

3.  **Go to Users:**
    * In the left-hand navigation pane, under "General," click on **Users**.

4.  **Add New User:**
    * Click on the blue button that says **Add new users**.

5.  **Enter Peter's Details:**
    * In the "Users" field, type Peter's email address. His name should auto-populate if he's part of your Azure Active Directory.
    * For "Access level," select **Basic + Test**.
    * For "Add to projects," you can leave this blank for now.
    * For "Azure DevOps Groups," you can leave the default or add him to any relevant default groups (e.g., "Project Contributors").

6.  **Add User:**
    * Click the **Add** button.

---

## Step 2: Add Peter to the "test1" Project and Make Him Admin

1.  **Navigate back to your Projects page:**
    * Click on the Azure DevOps logo in the top-left corner, or navigate to `dev.azure.com/[YourOrganizationName]`.

2.  **Select the "test1" Project:**
    * Find and click on the **"test1"** project from your list of projects.

3.  **Go to Project Settings:**
    * In the bottom-left corner of the page, click on **Project settings**.

4.  **Go to Permissions:**
    * In the left-hand navigation pane, under "General," click on **Permissions**.

5.  **Select Project Administrators Group:**
    * You will see a list of groups. Click on the **Project Administrators** group.

6.  **Add Peter to Project Administrators:**
    * Click the **Members** tab.
    * Click the **Add** button.
    * In the "Search for users or groups" field, type Peter's name or email address.
    * Select Peter from the search results.
    * Click **Save changes**.

---

## Step 3: Verify Peter's Access

1.  **Ask Peter to log in:** Have Peter log in to `dev.azure.com/[YourOrganizationName]` using his credentials.
2.  **Verify Access Level:** Peter should see the **"Test Plans"** hub available in his navigation, confirming the "Basic + Test" access level.
3.  **Verify Project Access and Admin Rights:** Peter should be able to navigate to the **"test1"** project and have full administrative control over it (e.g., modify project settings, manage teams, change permissions within the project).

---

**Important Note:** You must have **Project Collection Administrator** permissions in Azure DevOps to perform these actions.