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

## WAIT-1: Wait Module
Receptionist adds patients to a waiting queue so doctors can see order and manage appointments easily.

## AUTH-1: User Signup Module
## ROUND-1: round Module
Users can THE WAITING TIME 

## WAIT-2: Waite 2 Module
Doctor or receptionist monitors patient queue and waiting time.

## BED-1-1: User Bed -1 Module

## BED-2: User Bed -2 Module

## SHIFT-1: shift Module
Shift Swap Staff
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

## BILL-1: Create Invoice
Receptionist and Staff can generate invoices for patients
- Patient must be selected from database
- Add service items with quantity and price
- Auto-calculate total (qty × price - discount + tax)
- Invoice ID auto-generated
- Payment method must be selected
- Mark invoice as paid or partial payment
- Balance tracking for partial payments
- Download invoice as PDF
## PROFILE-1: Profile Management & Change Password
All users can view and edit their profile information

### View/Edit Profile:
- Profile data pre-filled from database
- Email is read-only (cannot be changed)
- Phone must be valid (11 digits)
- Profile photo upload (JPG/PNG only, max 2MB)
- License number required for medical staff
- Updated data saved in database
- Success message shown after update

### Change Password:
- Current password must match database
- New password must be ≥ 8 characters
- Confirm password must match new password
- Old and new password cannot be the same
- Password updated in database
- Session invalidated on change
- Redirect to login after change
- Success message shown
**Status: Implemented**
