# Club-VIP-Android-App-
# Club VIP - Android Application QA Project

## 📌 Project Overview
**Club VIP** is a premium club booking Android application developed for a generic foreign client (Logic Unit). This repository contains the complete Quality Assurance (QA) documentation, detailing the testing lifecycle from test planning to execution and bug reporting.

The primary objective of this project was to ensure the functional stability and usability of the application, focusing on high-value features such as Event Booking, VIP Table Reservations, and Social Connectivity.

## 📂 Repository Structure
This repository organizes the testing artifacts into the following categories:
* **Test Plans & Scenarios:** High-level overview of testing scope (TS_001 to TS_015).
* **Test Cases:** Detailed step-by-step procedures for modules (Login, Sign Up, Home, Events, etc.).
* **Execution Results:** Actual outcomes (Pass/Fail) recorded during the testing phase.
* **Bug Reports:** Documented defects with severity levels and reproduction steps.

## 📊 Test Statistics & Analysis

Based on the execution of the test suites, here is a statistical breakdown of the application's current stability:

### **Test Coverage**
| Metric | Count |
| :--- | :--- |
| **Total Test Scenarios** | 15 (covering 3 distinct modules) |
| **Total Test Cases Executed** | 400+ |
| **Testing Type** | Manual Functional Testing, UI/UX Validation |
| **Device Tested** | Android (APK Environment) |

### **Module Stability Status**
| Module | Priority | Status | Observations |
| :--- | :--- | :--- | :--- |
| **Auth (Login/Signup)** | P0/P1 | 🟢 **STABLE** | OTP, Registration, and Login flows work as expected. |
| **Home Screen** | P2 | 🔴 **UNSTABLE** | Navigation buttons (Profile, Notifications) non-responsive. |
| **Events & Tables** | P3 | 🟠 **RISK** | Filters (City/Month) returning incorrect data; Logic errors. |
| **UserProfile** | P2 | 🟡 **MIXED** | Password updates work, but validation for Names is weak. |

### **Defect Distribution**
Analysis of the `ClubVIP bug report.xlsx` reveals the following distribution of issues:

* **Functional Bugs:** 60% (e.g., Filters not sorting events, Buttons not navigating).
* **Validation Bugs:** 25% (e.g., Numeric characters accepted in Name fields).
* **UI/UX Bugs:** 15% (e.g., Slider dots not indicating active screen).

## 🛠 Bug Tracking & Efficiency
This project utilized a strict defect lifecycle. Below are highlights of the critical bugs identified during the QA process:

1.  **Critical Logic Failure (TS_012):** The "Apply Filter" functionality on the *All Tables* page failed to filter events by City or Month, displaying all events regardless of selection.
2.  **Navigation Blockers (TS_006):** Top navigation elements on the Home Screen (Profile Image, Bell Icon, Three-dot menu) were found to be non-functional, preventing user access to settings.
3.  **Data Integrity (TS_011):** The "Edit Profile" section incorrectly saved numeric integers in the "Full Name" field without throwing a validation error.

## 🧪 Methodologies Used
* **Black Box Testing:** Testing functionality without looking at the internal code structure.
* **Regression Testing:** Re-running test cases to ensure new features didn't break existing functionality (specifically performed on Auth flows).
* **Negative Testing:** Intentionally entering invalid data (e.g., invalid emails, empty fields) to test system resilience.

## 📝 Author
**Meesum** *QA Engineer* 

---
*This project serves as a portfolio piece demonstrating proficiency in Test Case Design, Defect Reporting, and Manual Mobile Application Testing.*
