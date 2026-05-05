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

## OPERATOR-1: Add Operator
Admin can add system operator
- Operator name required
- Role assigned
**Status: Implemented**
