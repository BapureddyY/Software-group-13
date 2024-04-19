# Hospital Management System Documentation

## Setup Instructions

### System Requirements
- Ensure Python 3.7.6 is installed and added to the system path.

### Installation Steps
- Open your terminal and execute the following commands to install necessary packages:
  ```
  pip install django==3.0.5
  pip install django-widget-tweaks
  pip install xhtml2pdf
  ```
- Download and extract the project ZIP folder.
- Navigate to the project directory in your terminal and run:
  ```
  py manage.py makemigrations
  py manage.py migrate
  py manage.py runserver
  ```
- Access the application via the following local URL:
  ```
  http://127.0.0.1:8000/
  ```

## Configuration for Contact Us Page
- Update your email settings in the `settings.py` file:
  ```
  EMAIL_HOST_USER = 'youremail@gmail.com'
  EMAIL_HOST_PASSWORD = 'your email password'
  EMAIL_RECEIVING_USER = 'youremail@gmail.com'
  ```
- Enable less secure app access by logging into your Gmail account and visiting:
  ```
  https://myaccount.google.com/lesssecureapps
  ```

## Potential Improvements and Security Concerns
- Anyone can become an Administrator without approval, which could be a security risk. Consider disabling open admin registration and opting for creating superusers through secure means.
- Ensure there is at least one doctor available in the hospital before patient admissions.
- Enforce password updates on the user information update pages to enhance security.


## Overview of Roles and Capabilities

### Administrator Role
- Create and log into an account without needing approval.
- Register, view, approve, reject, or remove doctors based on their job applications.
- Manage patient admissions, approvals, rejections, and discharges when treatment is complete.
- Generate and download invoices, incorporating costs like medicines, room charges, and doctor fees.
- Handle, book, and approve appointments as requested by patients.

### Doctor Role
- Submit job applications for hospital positions and log in once approved by the administrator.
- Access assigned patient information including symptoms, names, and contact details.
- View lists of patients who have been discharged.
- Manage their schedule and view appointments arranged by the administrator.
- Cancel appointments upon completion.

### Patient Role
- Register for hospital admission and log in once approved by the administrator.
- Access details of the assigned doctor such as specialization, contact information, and address.
- Monitor the status of booked appointments (whether pending or confirmed).
- Schedule new appointments, subject to administrator approval.
- Obtain and download invoices post-discharge.


Project Demo :


https://github.com/BapureddyY/Software-group-13/assets/154608567/0472c1bd-1833-4c43-b23f-74f7fcf76f56


---
