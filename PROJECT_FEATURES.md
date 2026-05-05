# Implemented Features

## AUTH-2: User Signin & Forgot Password
Users can login with email and password
- Email & password must match DB
- If correct → dashboard
- Else show 'Invalid email or password'
- Remember me option available
- Forgot password with email code verification
## AUTH-1: User Signup Module
Users can register as Admin, Doctor, Patient, Staff, Lab Technician, Receptionist, Operator
- Email must be unique
- Password must be ≥ 8 characters
- Re-password must match
- User type must be selected
- On signup → save in DB & redirect to dashboard
- Confirmation email sent
**Status: Implemented**

## DOC-1: Add Doctor
Admin can add doctor with name, specialization, schedule
- Doctor name required
- Specialization required
- Schedule must be valid
**Status: Implemented**

## APP-1: Create Appointment
Receptionist can book appointments for patients
- Patient and Doctor must be selected from database
- Date cannot be in the past
- Time slot must be available (no double booking)
- Reason for appointment optional
- Confirmation notification sent to patient and doctor
- Appointment saved in database
- Success message shown after booking
**Status: Implemented**

## APP-2: View/Manage Appointments
Admin and Staff can view and manage all appointments
- All appointments listed with correct details
- Filter by date, doctor, status
- Cancel appointments with reason
- Reschedule appointments to new time slot
- Notification sent on status change
- Export appointments to PDF/CSV
- Success message on update
**Status: Implemented**
