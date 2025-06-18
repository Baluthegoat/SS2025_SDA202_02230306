## Update Car Use Case - Detailed Flow Description

### **Basic Flow (Happy Path)**

**Step 1: Car Plate Number Entry**

- The Desk Officer initiates the update process by entering a car plate number into the system
- This serves as the unique identifier to locate the specific vehicle record that needs to be updated
- The input is typically entered through a user interface form or search field

**Step 2: Data Format Validation**

- The system immediately validates the entered plate number against predefined format rules
- This includes checking for proper length, character patterns, and compliance with regional plate number standards
- Format validation prevents invalid data from being processed further and ensures data integrity
- If validation fails, the system stops processing and displays a format error message

**Step 3: Car Record Retrieval**

- Upon successful format validation, the system queries the car database using the plate number as the search key
- The system performs a database lookup to locate the corresponding car record
- This step involves a database transaction to fetch the complete car information

**Step 4: Car Details Display**

- If the car record is found, the system retrieves all associated details (make, model, year, owner information, registration details, etc.)
- The system presents these details in an editable format on the user interface
- The display typically includes all modifiable fields that the Desk Officer can update
- The interface is designed to clearly show current values and allow for easy modification

**Step 5: Details Modification**

- The Desk Officer reviews the displayed information and makes necessary changes
- This could include updating owner information, changing registration status, modifying vehicle specifications, or correcting any inaccurate data
- The officer can modify multiple fields as needed during this step
- The system may provide validation for individual fields during data entry

**Step 6: Record Update**

- Once the Desk Officer completes the modifications and confirms the changes, the system processes the update
- The system performs a database update operation, replacing the old values with the new ones
- This involves a database transaction that ensures data consistency and integrity
- The system may also log the changes for audit trail purposes, recording who made the changes and when

**Step 7: Success Confirmation**

- After successfully updating the database, the system displays a confirmation message
- This message assures the Desk Officer that the changes have been saved successfully
- The system may also display the updated information for final verification

### **Alternate Flow: Car Not Found**

**Trigger Point:** Step 3 of the Basic Flow

**Flow Description:**

- When the system attempts to retrieve the car record from the database, no matching record is found for the entered plate number
- This could occur if:
    - The plate number doesn't exist in the system
    - The plate number was entered incorrectly despite passing format validation
    - The car record was previously deleted from the system
- Instead of proceeding to display car details, the system immediately displays an error message
- The error message typically indicates "Car not found" or "No record exists for the entered plate number"
- The process terminates at this point, and the Desk Officer must either:
    - Re-enter the correct plate number
    - Verify the plate number and potentially create a new car record if needed