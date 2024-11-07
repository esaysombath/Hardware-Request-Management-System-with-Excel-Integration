# Hardware Request Management System with Location-Based Inventory Integration

## Project Overview
Develop a system that enables mechanics to submit hardware requests linked to specific locations. The system will leverage data from an Excel-based inventory and produce Excel reports detailing requested items by location for easy reference by the admin team.

## Project Structure

### 1. Initial Setup
   - **Objective**: Set up a Flask application with an SQLite database to store hardware requests.
   - **Steps**:
      - Install Flask, Flask-SQLAlchemy, Pandas, and OpenPyXL (for Excel operations).
      - Set up a basic Flask project structure.
      - Create the SQLite database with tables for `requests` and `locations`.

### 2. Database Integration
   - **Objective**: Import inventory data from an Excel file into the SQLite database to populate the locations and hardware items available.
   - **Steps**:
      - Design tables: `requests`, `locations`, and `inventory`.
      - Write a script to read inventory data from an Excel file and insert it into the `inventory` table.
      - Define relationships between the tables in SQLAlchemy models.

### 3. User Interface (UI)
   - **Objective**: Create user-friendly forms for mechanics to submit requests and for admins to view and manage these requests.
   - **Steps**:
      - Design the submission form for mechanics (with fields for item, quantity, and location selection).
      - Set up the admin interface to view and update requests and to export requests as Excel reports.

### 4. Email Notification System
   - **Objective**: Notify the admin team via email whenever a new request is submitted.
   - **Steps**:
      - Create a function to send email notifications using SMTP.
      - Trigger the email notification function upon successful request submission.

### 5. Excel Reporting
   - **Objective**: Generate an Excel report listing all hardware requests by location.
   - **Steps**:
      - Write a function to retrieve all requests grouped by location.
      - Use Pandas and OpenPyXL to format and export this data into an Excel file.
      - Allow the admin to download the report from the admin interface.

## Technical Skills Demonstrated
   - **Web Development**: Flask, HTML, CSS
   - **Database Management**: SQLite, SQLAlchemy
   - **Excel Operations**: Pandas, OpenPyXL for reading/writing data
   - **Email Integration**: SMTP for email notifications

## User Workflow
1. Mechanic submits a request for hardware, specifying item, quantity, and location.
2. Admin receives an email notification and can view the request details.
3. Admin exports all requests by location to an Excel report for efficient hardware fulfillment.

## Future Enhancements
   - Add real-time inventory updates based on requests.
   - Implement user authentication for admins and mechanics.
   - Add additional filters or search options in the admin interface.

---

This outline should help you build out the key features while keeping the project organized!
