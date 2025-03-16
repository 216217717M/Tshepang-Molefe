
# Test Case Development

## Functional Test Cases  
| Test Case ID | Requirement ID | Description | Steps | Expected Result | Actual Result | Status |
|-------------|---------------|-------------|-------|-----------------|---------------|--------|
| TC-001 | FR-001 | Barber sets and manages schedule | 1. Barber logs in. 2. Navigates to "Manage Schedule". 3. Updates availability. 4. Saves changes. | System updates the schedule, blocking off unavailable slots. | - | - |
| TC-002 | FR-002 | Client updates profile | 1. Client logs in. 2. Navigates to "Profile". 3. Updates personal details. 4. Saves changes. | Profile details are updated and displayed correctly. | - | - |
| TC-003 | FR-003 | Client views booking history | 1. Client logs in. 2. Navigates to "Booking History". 3. Selects filter (upcoming, canceled, completed). | System displays sorted booking history. | - | - |
| TC-004 | FR-004 | Check barber availability | 1. Client selects a barber. 2. System displays available slots. | Only available slots are shown for selection. | - | - |
| TC-005 | FR-005 | Confirm booking via SMS/email | 1. Client books an appointment. | System sends confirmation via SMS and email with full details. | - | - |
| TC-006 | FR-006 | Payment processing | 1. Client selects service. 2. Chooses payment method. 3. Completes transaction. | System successfully processes payment and issues a receipt. | - | - |
| TC-007 | FR-007 | Modify or cancel appointment | 1. Client attempts to reschedule/cancel. 2. System checks 24-hour restriction. | System allows changes if within the permitted timeframe. | - | - |
| TC-008 | FR-008 | Client books an appointment | 1. Client selects a barber and service. 2. Chooses available slot. 3. Confirms booking. | System successfully books appointment. | - | - |
| TC-009 | FR-009 | Automated reminders sent | 1. Appointment is scheduled. 2. System sends reminder 24 hours before the appointment. | Client receives email and SMS reminder with full details. | - | - |
| TC-010 | FR-010 | Admin manages appointments | 1. Admin logs in. 2. Opens dashboard. 3. Filters appointments by date/client. | System displays filtered appointments accurately. | - | - |

---

## Non-Functional Test Scenarios  
| Test Case ID | Requirement | Description | Test Steps | Expected Result | Actual Result | Status |
|-------------|------------|-------------|-----------|----------------|---------------|--------|
| TC-NF-001 | Security | **Data Encryption (AES-256)** | 1. Capture sensitive data (payment, passwords). 2. Inspect database and data transmission. | Data is encrypted, unreadable in storage and transit. | - | - |
| TC-NF-002 | Security | **User Authentication (2FA)** | 1. Client/admin logs in. 2. System requests 2FA code. 3. User enters correct code. | System grants access only after successful 2FA verification. | - | - |
| TC-NF-003 | Performance | **Page Load Time** | 1. Open system homepage. 2. Measure load time. | System loads in **≤2 sec for 90% of users**. | - | - |
