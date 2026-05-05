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

## AUTH-3: Admin Dashboard
Admin can view system overview with panels
- Total Doctors, Total Patients, Total Staff counts
- Click panels redirect to respective lists
- Full navigation menu to all modules
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

## APP-2: View/Manage Appointments
Admin and Staff can view and manage all appointments
- All appointments listed with correct details
- Filter by date, doctor, status
- Cancel appointments with reason
- Reschedule appointments to new time slot
- Notification sent on status change
- Export appointments to PDF/CSV
- Success message on update
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

Receptionist and Admin can register new patients
- All required fields must be filled
- Fields: name, email, phone, gender, dob, blood group, address, emergency contact
- Email must be unique
- Phone must be valid (11 digits)
- Blood group must be selected from valid options
- Emergency contact is required
- Unique Patient ID auto-generated on save
- Data stored in database
## BILL-2: View Billing History
Staff and Patients can view billing history
- All invoices listed with correct details
- Filter by status (Paid/Unpaid/Partial)
- Filter by date range
- Filter by patient name
- View invoice details
- Download invoice as PDF
- Staff cannot delete invoices
- Patients see only their own invoices
- Unpaid invoices clearly marked
- Correct totals shown
**Status: Implemented**

## PAT-3: Upload Patient Report
Admin, Receptionist, and Lab Technician can upload medical reports
- Patient must be selected from database
- Doctor can be selected (optional)
- Report title is required
- Report date is required
- File upload: PDF, JPG, PNG only
- File size limit: max 10MB
- Notes field optional for additional comments
- Data stored linked to patient record
- Success message shown after upload
- LED indicator triggers when all reports for patient are complete
## PAT-2: Edit/View Patient List
Admin and Receptionist can view and edit patient information
- All patient data displayed correctly in table
- Columns: Name, Email, Phone, Blood Group, Status
- Search/filter by name, ID, blood group
- View button shows full patient details
- Edit button opens form with pre-filled data
- Validation same as Add Patient on edit
- Updated data saved to database
- Delete button with confirmation before delete
- Patient history preserved on delete flag
- Success message shown on update/delete
**Status: Implemented**

## MED-1: Med Stock - Update Stock
Operator, Pharmacy, and Admin can manage medicine stock
- Medicine name must be entered
- Quantity must be entered (positive number)
- Add new medicine to inventory
- Update existing medicine quantity
- Minimum stock level can be set for alerts
- Low stock alert (SMS notification) when below minimum
- Expiry date tracking for medicines
- Stock in and stock out records maintained
- Success message shown after update
**Status: Implemented**

## MED-2: Med Stock Panels
Dashboard panels for medicine inventory management

### Medicine Inventory Panel:
- Displays all medicines with current stock levels
- Columns: Medicine Name, Quantity, Expiry Date, Status
- Search/filter by medicine name
- Sort by stock level or expiry date

### Low Stock Medicines Panel:
- Shows medicines below minimum threshold
- Highlighted in red/orange for visibility
- Reorder button for quick restocking
- SMS alert sent automatically

### Recently Used Medicines Panel:
- Tracks medicines dispensed recently
- Shows date and quantity used
- Helps identify consumption patterns
- Export report option available
**Status: Implemented**

## DIAG-1: Diagnostic Test Queue
Manage diagnostic tests from request to completion

### Request Test (Doctor):
- Doctor enters Patient ID and Test Type
- Test request added to diagnostic queue
- Priority (Normal/Emergency) can be set
- Estimated completion time shown

### Pending Tests Panel:
- Shows all tests waiting to be processed
- Sort by priority, date, or test type
- Lab technician can start test

### Tests in Progress Panel:
- Shows tests currently being processed
- Estimated remaining time displayed
- Technician can mark as completed

### Completed Tests Panel:
- Shows all completed tests
- Lab technician uploads test results
- File types: PDF, JPG, PNG (max 10MB)
- LED triggers when all reports for patient are ready
- Patient history includes all previous test reports
**Status: Implemented**
