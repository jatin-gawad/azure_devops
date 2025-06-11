# Azure DevOps – User Access & Role Management Documentation

## Purpose
To provide a step-by-step guide for adding users to Azure DevOps, assigning appropriate access levels (e.g., Basic + Test Plans), and setting project-level roles such as Contributor or Project Administrator.

---

## Prerequisites
- You must have **Organization Administrator** permissions in Azure DevOps.
- The user(s) must have a valid email (preferably already in the Microsoft Entra ID/AAD if using enterprise directory sync).
- Required access licenses (e.g., Basic, Basic + Test Plans) must be available in the Azure DevOps license pool.

---

## Step-by-Step Instructions

### 1. Add a User to the Azure DevOps Organization

1. Go to: `https://dev.azure.com/{your_organization}`
2. In the lower-left corner, click on **Organization settings**.
3. In the left menu, click **Users**.
4. Click the **+ Add users** button.
5. Fill out the form:
   - **Users**: Enter the user's email (e.g., tom@example.com).
   - **Access level**: Choose one:
     - Basic
     - Basic + Test Plans (if test suite access is needed)
   - **Add to projects**: Select the appropriate project (e.g., Agile CAB, Bestlov, etc.).
   - **Azure DevOps Groups**: Choose:
     - Contributor
     - Reader
     - Project Administrators (only if full permissions are needed)
6. Click **Add**.

> Note: If the user is not part of the Azure AD tenant, you may first need to invite them as a guest user through Microsoft Entra ID.

---

### 2. Assign or Verify Access Level

1. Go to **Organization Settings** > **Users**.
2. Find the user by name or email.
3. Check the "Access level" column:
   - If incorrect, select the checkbox next to the user.
   - Click **Change access level** on the top bar.
   - Choose the correct level (e.g., Basic + Test Plans).
   - Click **Save**.

> Only Organization Admins can change access levels. Project Admins cannot do this.

---

### 3. Add a User to a Specific Project (If Not Done During Initial Add)

1. Go to the project (e.g., Agile CAB).
2. Click **Project settings** (bottom-left).
3. Under **General**, click **Permissions**.
4. Choose the desired group:
   - Contributors
   - Readers
   - Project Administrators
5. Click the **Members** tab > **+ Add**.
6. Search for and select the user.
7. Click **Save**.

---

### 4. Confirm Project Role and Access

1. Go to **Project Settings** > **Permissions**.
2. Click the appropriate group (e.g., Contributors).
3. Under the “Members” tab, confirm the user is listed.
4. You may also verify permissions under the **Security** settings for Area Paths and Repos, if needed.

---

### 5. Optional: Add User to Project Team (for Boards)

1. Go to **Project Settings** > **Teams**.
2. Click the appropriate team (e.g., Agile CAB Team).
3. Under **Members**, click **+ Add** and select the user.

---

## Access Summary Table

| Action                          | Required Role             |
|---------------------------------|----------------------------|
| Add user to org                 | Organization Admin         |
| Assign access level (Basic/Test)| Organization Admin         |
| Add user to project             | Project Admin or Org Admin |
| Assign project role             | Project Admin              |
| Create new project              | Organization Admin         |

---

## Notes
- Stakeholder users are free but have limited access.
- Basic + Test Plans requires a paid license.
- If a user reports they can’t access a feature, always check:
  - Are they in the organization?
  - Do they have the correct access level?
  - Are they added to the project and correct group?


