# Automated Data Collection using n8n

An automated data collection workflow built with **n8n, Google Forms-style web forms, and Google Sheets**. This project collects user information through a web form, processes the submitted data, and automatically stores it in Google Sheets.

## 🚀 Project Overview

The purpose of this project is to automate the process of collecting and organizing user information without manually entering data into a spreadsheet.

Whenever someone submits the form, n8n automatically processes the information and adds a new record to Google Sheets.

## 🛠️ Technologies Used

- **n8n** – Workflow automation platform
- **n8n Form Trigger** – Collects user information
- **Edit Fields (Set)** – Processes and organizes submitted data
- **Google Sheets** – Stores collected information
- **Google OAuth2** – Authenticates the Google Sheets connection

## ⚙️ Workflow Architecture

```text
       User
        |
        ▼
  Form Submission
        |
        ▼
   Form Trigger
        |
        ▼
    Edit Fields
        |
        ▼
   Google Sheets
        |
        ▼
  Data Successfully Saved
```

## 📋 Data Collected

The Google Spreadsheet is configured with the following columns:

| Field | Description |
|---|---|
| Full Name | User's full name |
| BOD | Date of birth |
| Email Address | User's email |
| Gender | User's gender |
| Police | User's police-related form field |
| Image | Uploaded image information |

## ✨ Key Features

- Automated data collection through a web form.
- Automatic processing of submitted information.
- Integration with Google Sheets.
- Automatic insertion of new records.
- No need for manual spreadsheet data entry.
- Production URL for real-time form submissions.

## 🔧 How to Set Up

### 1. Install n8n

Create an account or install n8n:

https://n8n.io/

### 2. Create a New Workflow

Create a new workflow and add these nodes in order:

1. Form Trigger
2. Edit Fields (Set)
3. Google Sheets

### 3. Configure Form Trigger

Create your form and add the required fields.

### 4. Configure Edit Fields

Map the incoming form data to the appropriate output fields.

### 5. Connect Google Sheets

- Create a Google Spreadsheet.
- Add your column headings.
- Connect your Google account using Google OAuth2.
- Select the spreadsheet and worksheet.
- Choose the **Append Row** operation.
- Map the form fields to the corresponding spreadsheet columns.

### 6. Activate the Workflow

Save and publish your workflow.

Use the Production URL to receive real form submissions.

## 📸 Project Screenshots

project screenshots here:

- <img width="1092" height="483" alt="Screenshot 2026-11-22 124334" src="https://github.com/user-attachments/assets/1b5fdcf3-48a6-4706-9377-9a68699943a1" />
 – Complete n8n workflow.
- <img width="483" height="874" alt="Screenshot 2026-11-22 124400" src="https://github.com/user-attachments/assets/db1424e1-428f-445f-96c7-2f88b0126528" />
 – User submission form.
-<img width="989" height="325" alt="Screenshot 2026-11-22 124540" src="https://github.com/user-attachments/assets/2a37e516-340c-4b40-86a4-738ac6f4d7c9" />
 – Collected data in Google Sheets.

## 🎯 Learning Outcomes

Through this project, I learned:

- How workflow automation works.
- How to create forms using n8n.
- How to process data using Edit Fields.
- How to integrate Google Sheets with n8n.
- How to configure OAuth2 authentication.
- How to automate data collection and storage.

## 🔮 Future Improvements

- Email notifications after successful submissions.
- Form data validation.
- Duplicate submission detection.
- Automatic timestamps.
- Improved error handling.
- Additional data processing and reporting.

## 👨‍💻 Author

**Sayed Monawar Rakib**

Computer Science & Technology | Automation Enthusiast

GitHub: https://github.com/sayedmonawarrakib

## 📄 License

This project is available for educational and learning purposes. You may modify and extend it for your own automation projects.
