# User Management Screen - User Interface Specification


## UI Components and Layout

1. **User List View:**
   - Display a table listing existing users with columns for Username, Email, Role, Status, and Actions (Edit and Deactivate/Activate).
   - Include a search bar at the top to allow users to search for specific users by name or email.

2. **Create/Edit User Form:**
   - Provide input fields for entering the user's Full Name, Email Address, Password, Role (dropdown), and Active/Inactive status (checkbox).
   - Add buttons for "Save" and "Cancel" actions.

3. **Confirmation Modal:**
   - For actions like deleting a user or deactivating an account, display a confirmation modal with "Yes" and "No" buttons.

## Page Behavior

1. **On Load:**
   - Upon loading the User Management screen, fetch the list of existing users from the backend API and populate the User List View table.
   - Display the search bar at the top of the table with a placeholder text like "Search by name or email."

2. **Creating a New User:**
   - Clicking the "Create New User" button will open the Create User Form as a modal.
   - When the "Save" button is clicked, perform form validation to ensure all required fields are filled.
   - If the form is valid, send the data to the backend API to create the new user.
   - Display a success message and refresh the User List View with the updated user list.
   - If the form is invalid, display appropriate error messages next to the respective fields.

3. **Editing User Information:**
   - Clicking the "Edit" button in the User List View for a specific user will open the Edit User Form as a modal, pre-filled with the user's information.
   - Allow administrators to modify the user's details and click the "Save" button to update the user information.
   - Perform form validation as done during user creation.

4. **Deactivating/Activating a User:**
   - Clicking the "Deactivate/Activate" button in the User List View for a specific user will display the Confirmation Modal.
   - Upon confirming the action, send the request to the backend API to deactivate or activate the user account.
   - Display a success message and update the user's status in the User List View.

## Initial UI View

- When the User Management Screen is accessed, the User List View table will be displayed.
- The table will show the list of existing users, and the search bar will be available at the top for filtering users.
- Below the table, there will be a "Create New User" button to add new users.
- The table will contain data such as Username, Email, Role, and Status, along with "Edit" and "Deactivate/Activate" buttons for each user.


