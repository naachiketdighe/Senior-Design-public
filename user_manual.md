# User Documentation and User Manual

## Overview
Welcome to the **Custom CRM System** user guide. This document provides step-by-step instructions on installing, using, and troubleshooting our CRM system. It is designed for both beginners and advanced users, ensuring seamless navigation and usability.

---
## I. Installation Guide

### **System Requirements**
- Operating System: Windows 10, macOS, Linux
- Python 3.8+
- Django 4.0+
- SQLite 3.0+
- Node.js (for frontend development with TailwindCSS)

### **Installation Steps**
1. Clone the repository:
   ```bash
   git clone https://github.com/naachiketdighe/Senior-Design-public
   cd customcrm
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For macOS/Linux
   venv\Scripts\activate  # For Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run migrations to set up the database:
   ```bash
   python manage.py migrate
   ```
5. Start the server:
   ```bash
   python manage.py runserver
   ```
6. Open a browser and visit `http://127.0.0.1:8000/`

---
## II. User Guide

### **Logging In**
1. Open the CRM system in your web browser.
2. Enter your **username** and **password**.
3. Click **Login** to access the dashboard.

### **Adding a Customer**
1. Navigate to the "Customers" section.
2. Click **Add New Customer**.
3. Fill in the required details (Name, Email, Phone, Address).
4. Click **Save** to store the customer record.

### **Editing a Customer Record**
1. Go to the "Customers" list.
2. Click **Edit** next to the desired customer.
3. Modify the information as needed.
4. Click **Update** to save changes.

### **Assigning a Customer to a Team**
1. Select a customer from the "Customers" section.
2. Click **Assign to Team**.
3. Choose a team member from the dropdown list.
4. Click **Confirm Assignment**.

### **Generating Reports**
1. Navigate to the "Reports" section.
2. Choose the type of report you want (e.g., Customer Interactions, Team Performance).
3. Click **Generate Report**.
4. Download or print the report as needed.

---
## III. Frequently Asked Questions (FAQ)

### **1. How do I reset my password?**
- Click **Forgot Password** on the login page.
- Enter your registered email.
- Follow the instructions sent to your email.

### **2. Can I export customer data?**
- Yes. Go to the "Customers" section, click **Export**, and choose CSV or Excel format.

### **3. How can I add multiple users?**
- Admins can go to "User Management" and click **Add User**.

### **4. What should I do if I get a server error?**
- Restart the server by running:
  ```bash
  python manage.py runserver
  ```
- Check the logs for any error messages and troubleshoot accordingly.

### **5. How do I update my CRM system?**
- Pull the latest updates from the repository:
  ```bash
  git pull origin main
  ```
- Apply migrations if needed:
  ```bash
  python manage.py migrate
  ```

---
## IV. Troubleshooting

### **Common Issues and Fixes**
| Issue | Possible Cause | Solution |
|------|--------------|----------|
| Unable to log in | Incorrect username/password | Reset password via email |
| Page not loading | Server not running | Start server using `python manage.py runserver` |
| Data not saving | Database issue | Run `python manage.py migrate` |

For further support, contact **dighent@mail.uc.edu**.

---
This user guide aims to provide clear instructions and troubleshooting tips to help users effectively navigate the CRM system.
