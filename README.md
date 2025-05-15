🛒 SalesDB – MySQL Sales Management System

This project is a fully functional sales database built using SQL and phpMyAdmin. It simulates a retail environment where products are sold to customers by system users (e.g., admin, cashier). The system includes real-world database design features such as views, foreign keys, and triggers.

📌 Project Goals

- Practice database creation using Data Definition Language (DDL)
- Simulate a real-world retail sales system
- Implement normalized table relationships
- Generate sales reports using SQL views
- Introduce triggers for logging actions automatically

🧱 Database Structure

📦 Tables:
- Customers – Stores customer records
- Products – Stores product details and pricing
- Sales – Stores transaction records (customer + product + quantity + date)
- Users – Simulates login info and roles
- SalesLog – Automatically logs sales using a trigger

👁️ View:
- CustomerSalesReport – Shows total spending per customer

🧰 Technologies Used

- MySQL (via phpMyAdmin)
- XAMPP on Windows 11
- dbdiagram.io (for ER diagram)

📸  Screenshots

![Screenshot 2025-05-16 003045](https://github.com/user-attachments/assets/e3dc9e78-e11f-4e2d-a876-c41e5a3ca78b)
![Screenshot 2025-05-16 003010](https://github.com/user-attachments/assets/e6320748-7099-40f2-b9d1-83f3a731e707)
![Screenshot 2025-05-16 002918](https://github.com/user-attachments/assets/443e13f9-81f3-4757-b2de-b320e92376fb)
![Screenshot 2025-05-16 002756](https://github.com/user-attachments/assets/26e051a9-b963-40c9-967c-996ccc94af9d)
![Screenshot 2025-05-16 002712](https://github.com/user-attachments/assets/06945181-4a61-45e2-a3af-583d414e0f2b)
![Screenshot 2025-05-16 002448](https://github.com/user-attachments/assets/a3473dbc-69b3-4f92-8916-90f4f59f314d)
![Screenshot 2025-05-16 002326](https://github.com/user-attachments/assets/694a849f-a55f-4156-aa98-d6ae3ceea2a9)
![Screenshot 2025-05-16 002031](https://github.com/user-attachments/assets/42cdcdc5-2d74-4834-856c-953616621fca)
![Screenshot 2025-05-16 001850](https://github.com/user-attachments/assets/9657818a-1f38-429e-8d7b-09c58940eaf1)
![Screenshot 2025-05-16 001710](https://github.com/user-attachments/assets/43f4bb13-3975-4102-89ce-5612de37c353)
![Screenshot 2025-05-15 232918](https://github.com/user-attachments/assets/aa69d51f-e7a4-4289-bb2c-1a6eb8009a3b)
![Screenshot 2025-05-15 232813](https://github.com/user-attachments/assets/52804b2c-d8cb-4c6f-9334-8f73439ddc2d)
![Screenshot 2025-05-15 232522](https://github.com/user-attachments/assets/12c2d12b-f20f-4696-919f-e40e9e5838f9)
![Screenshot 2025-05-15 232303](https://github.com/user-attachments/assets/4bc9bf6e-cd9d-44ee-a7aa-64af714cbc8c)
![Screenshot 2025-05-15 232127](https://github.com/user-attachments/assets/938e310e-aa43-471b-97cc-39d8a9a6dd92)
![Screenshot 2025-05-15 232115](https://github.com/user-attachments/assets/a4056f2f-e3a2-443e-a4e2-21dc2a528bb5)
![Screenshot 2025-05-15 231857](https://github.com/user-attachments/assets/d07cca63-78a6-45eb-abed-0ae8038cf353)
![Screenshot 2025-05-15 231603](https://github.com/user-attachments/assets/9f2e5f9d-9ab6-412d-9151-edfa2393cd8d)
![Screenshot 2025-05-15 231404](https://github.com/user-attachments/assets/094dca7b-f21b-4596-9aff-fc3a3bb562ed)
![Screenshot 2025-05-15 231106](https://github.com/user-attachments/assets/1655baaa-2036-43b2-a8d8-414a4484270a)
![Screenshot 2025-05-15 230811](https://github.com/user-attachments/assets/e30f1843-af19-4f9e-9b52-df2a47af6e95)

![ER Diagram (from dbdiagram io)-page-00002](https://github.com/user-attachments/assets/0cbd9d2f-6a8d-46d3-8e58-aa588f360271)
![ER Diagram (from dbdiagram io)-page-00001](https://github.com/user-attachments/assets/63425a15-2966-496c-ad46-b36f477b385f)

🧪 Example Queries

```sql
-- View total sales per customer
SELECT * FROM CustomerSalesReport;

-- Insert a new user
INSERT INTO Users VALUES ('U004', 'test_user', 'hash123', 'cashier');

-- Add a new sale (also triggers a log entry)
INSERT INTO Sales VALUES ('S006', 'C001', 'P002', '2025-05-10', 1);

-- Check the log
SELECT * FROM SalesLog;
---

👤 Author

Abu Bakr E. Ceesay  
Undergraduate Informatics Engineering Student  
Nusa Putra University – Second semester 2024/2025

