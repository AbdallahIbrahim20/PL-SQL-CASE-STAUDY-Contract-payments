Here’s a more polished and professional version of your project description:  

---

### **Project Overview:**  
This project demonstrates the application of concepts learned in SQL and PL/SQL by working with a relational database consisting of three tables: **Clients**, **Contracts**, and **Installments_Paid**. The primary goal of the project is to calculate and manage installment payments for each contract.  

---

### **Project Setup and Execution:**  

1. **Prepare the Environment:**  
   - Download the `project_script.rar` file and extract its contents. The archive contains the table creation scripts and a sequence used for the insertion process.  
   - Note: You may skip the first step if you directly execute the creation script file.  

2. **Run the Creation Script:**  
   - Open the creation script file using an SQL editor, such as **Toad**, and execute it as a script. This will create the required tables, sequence, and initial database structure.  

3. **Create and Execute Supporting Functions:**  
   - **Calculate Years Between:** This script defines a function to calculate the number of years between the contract’s start and end dates based on the provided **contract_id**.  
   - **Calculate Installments Per Year:** This script defines a function to determine the number of installments to be paid annually for a given **contract_id**.  
   - **Calculate Total Installments:** This script defines a function to calculate the total number of installments to be paid over the entire duration of the contract.  

4. **Run the Main Program:**  
   - The main program utilizes a cursor to iterate through each contract, calculating the installment amount using the formula:  
     \[
     \text{Installment Amount} = \frac{\text{Contract Total Fees} - \text{Contract Deposit Fees}}{\text{Total Number of Installments}}
     \]  
   - The program stores the contract's start date in a variable and loops through the dates, inserting the calculated installment amounts and their corresponding payment dates into the **Installments_Paid** table, until the end date of the contract is reached.  

---

### **Key Highlights:**  
- **Dynamic Functions:** The project incorporates dynamic PL/SQL functions to calculate essential metrics such as contract duration, annual installments, and total installment counts.  
- **Cursor-Based Processing:** Efficient looping through contract records ensures accurate calculation and insertion of installment data.  
- **Automated Data Management:** The project demonstrates practical database automation by managing recurring payments for multiple contracts.  

This project showcases a robust application of SQL and PL/SQL skills in building and managing database-driven financial operations.
