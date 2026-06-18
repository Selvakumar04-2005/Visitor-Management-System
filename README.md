<div align="center">

# 🚀 Smart Visitor Management System
### AI-Powered Visitor Registration & Tracking Platform using ServiceNow

<img src="https://img.shields.io/badge/Platform-ServiceNow-brightgreen?style=for-the-badge">
<img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge">
<img src="https://img.shields.io/badge/AI-Recommendation-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/Dashboard-Analytics-orange?style=for-the-badge">

---

### 🏢 Digital Visitor Management Solution
Automating Visitor Registration, Validation, Notifications, Check-In/Check-Out, Reports and Dashboard Analytics.

</div>

---

# 📖 Project Overview

The **Smart Visitor Management System** is a ServiceNow-based application developed to simplify and automate visitor management within an organization.

The system allows users to:

✅ Register Visitors

✅ Validate Visitor Information

✅ Generate AI-Based Recommendations

✅ Send Automated Email Notifications

✅ Perform Visitor Check-In

✅ Perform Visitor Check-Out

✅ Generate Reports

✅ Monitor Visitor Analytics through Dashboards

---

# 🎯 Project Objectives

The primary objective of this project is to digitize visitor management and reduce manual work.

### Key Goals

- Improve Security
- Reduce Paper-Based Records
- Automate Visitor Tracking
- Enhance User Experience
- Generate Smart Recommendations
- Enable Real-Time Reporting

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| ServiceNow Studio | Application Development |
| ServiceNow Tables | Data Storage |
| Client Scripts | Validation |
| Business Rules | Automation |
| Flow Designer | Workflow Automation |
| Email Notifications | User Communication |
| Reports | Analytics |
| Dashboards | Visualization |
| UI Actions | Check-In & Check-Out |

---

# 🏗 System Architecture

```text
Visitor
   │
   ▼
Registration Form
   │
   ▼
Client Validation
   │
   ▼
Visitor Request Table
   │
   ▼
Business Rules
   │
   ▼
AI Recommendation
   │
   ▼
Flow Designer
   │
   ▼
Email Notification
   │
   ▼
Check-In / Check-Out
   │
   ▼
Reports
   │
   ▼
Dashboard
```

---

# 📂 Project Modules

## 1️⃣ Visitor Registration Module

Collects visitor information:

- Visitor Name
- Mobile Number
- Email
- Purpose
- Visit Date

---

## 2️⃣ Validation Module

Ensures correct data entry.

### Mobile Validation

```javascript
function onSubmit() {

    var mobile =
    g_form.getValue('mobile_number');

    if(!/^[0-9]{10}$/.test(mobile)) {

        g_form.addErrorMessage(
        'Enter valid 10 digit number');

        return false;
    }

    return true;
}
```

---

## 3️⃣ AI Recommendation Module

Automatically suggests actions based on visitor purpose.

### Example

| Purpose | Recommendation |
|----------|--------------|
| Interview | Schedule HR Meeting Room |
| Delivery | Route to Security Desk |
| Client Meeting | Arrange Conference Room |

### Business Rule

```javascript
(function executeRule(current){

if(current.purpose == 'Interview'){

current.ai_recommendation =
'Schedule HR Meeting Room';

}

})(current);
```

---

## 4️⃣ Email Notification Module

Automatically sends confirmation emails after visitor registration.

### Email Contains

- Visitor Name
- Purpose
- Visit Date
- Status

---

## 5️⃣ Check-In Module

Updates Visitor Status:

```text
Requested
      ↓
Checked In
```

---

## 6️⃣ Check-Out Module

Updates Visitor Status:

```text
Checked In
      ↓
Checked Out
```

---

## 7️⃣ Dashboard & Reporting Module

### Dashboard Widgets

📊 Visitor Status Report

📈 Visitor Purpose Report

📉 Monthly Visitor Report

---

# 📊 Database Design

## Table: Visitor Request

| Field Name | Type |
|------------|------|
| Visitor ID | String |
| Visitor Name | String |
| Mobile Number | String |
| Email | String |
| Purpose | Choice |
| Visit Date | Date |
| Status | Choice |
| AI Recommendation | String |

---

# 🔄 Workflow Process

```text
Visitor Registration
         ↓
Input Validation
         ↓
Record Creation
         ↓
AI Recommendation
         ↓
Email Notification
         ↓
Check-In
         ↓
Check-Out
         ↓
Dashboard Update
```

---

# 📈 Reports Created

### Visitor Status Report

Shows:

- Requested
- Approved
- Rejected
- Checked In
- Checked Out

---

### Visitor Purpose Report

Shows:

- Interview
- Client Meeting
- Business Meeting
- Delivery
- Other

---

### Monthly Visitor Report

Shows visitor count month-wise.

---

# 📧 Automated Email Sample

```text
Hello,

Your Visitor Request has been submitted successfully.

Visitor Name: Ram

Purpose: Interview

Visit Date: 23/06/2026

AI Recommendation:
Schedule HR Meeting Room

Status: Requested

Thank You,
Visitor Management Team
```

---

# 🧪 Testing

| Test Case | Expected Result | Status |
|------------|----------------|---------|
| Valid Mobile Number | Record Saved | ✅ Pass |
| Invalid Mobile Number | Error Message | ✅ Pass |
| Past Date | Validation Error | ✅ Pass |
| Interview Purpose | AI Recommendation | ✅ Pass |
| Email Notification | Email Sent | ✅ Pass |

---

# 🌟 Key Features

✅ Smart Visitor Registration

✅ Mobile Number Validation

✅ Date Validation

✅ AI-Based Recommendations

✅ Email Notifications

✅ Visitor Status Tracking

✅ Check-In / Check-Out

✅ Reports

✅ Interactive Dashboard

---

# 🚀 Future Enhancements

- QR Code Visitor Pass
- Face Recognition
- SMS Notifications
- Mobile Application
- Visitor Badge Printing
- Security Gate Integration

---

# 👨‍💻 Developed By

### Selvakumar K
**B.Tech Information Technology**

Karpagam Institute of Technology

---

# 📜 Project Title

### Smart Visitor Management System Using ServiceNow with AI-Powered Recommendations, Automated Notifications, and Dashboard Analytics

---

<div align="center">

### ⭐ If you like this project, give it a star ⭐

🚀 Built with ServiceNow

</div>
