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

<img width="987" height="590" alt="Screenshot 2026-11-22 122609" src="https://github.com/user-attachments/assets/92746ce3-68d5-44d1-93a2-26e17ae46306" />
Complete n8n workflow.
<img width="559" height="267" alt="Screenshot 2026-11-22 123509" src="https://github.com/user-attachments/assets/6ec67a4e-2247-48c7-8ce4-953ea4efe530" />
Collected data in Google Sheets.

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

GitHub:https://github.com/sayedmonawarrakib

## 📄 License

This project is available for educational and learning purposes. You may modify and extend it for your own automation projects.
