# Output Screens (Website + Hall Allocation + Mobile Application)

This section contains the visual outputs of the **Integrated Exam Hub: QR Code Hall Ticket & Fingerprint Attendance System**.  
Each screenshot demonstrates a key function of the system and showcases the workflow across the Web Portal, Mobile Application, and Hall Allocation module.

---

## 1. Website Screenshots

(Include screenshots for all web pages like login, dashboard, timetable, hall ticket PDF)

| Screenshot Name | Description | File Location |
|-----------------|-------------|---------------|
| **Home_Page_of_Website** | Main landing page that provides access to Student and Staff login portals. | [View Screenshot](website/Home_Page_of_Website.jpg) |
| **Student_Portal_Login_Password** | Student login page where student enters Student ID and Password. | [View Screenshot](website/Student_Portal_Login_Password.jpg) |
| **Student_Portal_Email_Login** | Email verification screen for OTP-based second-level authentication. | [View Screenshot](website/Student_Portal_Email_Login.jpg) |
| **Student_OTP_Verification** | Screen where the student enters the received OTP to complete login. | [View Screenshot](website/Student_OTP_Verification.jpg) |
| **Student_Login_OTP_Sent** | Notification screen confirming OTP has been sent to registered email ID. | [View Screenshot](website/Student_Login_OTP_Sent.jpg) |
| **Student_DashBoard1** | Student dashboard showing hall ticket download, exam updates, and alerts. | [View Screenshot](website/Student_DashBoard1.jpg) |
| **Student_DashBoard2** | Alternate student dashboard view (additional options or exam details). | [View Screenshot](website/Student_DashBoard2.jpg) |
| **Student_Timetable** | Student's complete exam timetable with date, session, and hall allocation. | [View Screenshot](website/Student_Timetable.jpg) |
| **student_report_StudentID.pdf** | Auto-generated hall ticket PDF containing QR code and student identity information. | [View File](website/student_report_CYA01AAS1264.pdf) |
| **Staff_Login** | Staff login screen (ID + Password + OTP). | [View Screenshot](website/Staff_Login.jpg) |
| **Staff_Dashboard** | Dashboard showing invigilator responsibilities and exam monitoring details. | [View Screenshot](website/Staff_Dashboard.jpg) |
| **Staff_Timetable** | Detailed staff invigilation schedule across dates, halls, and sessions. | [View Screenshot](website/Staff_Timetable.jpg) |


## 2. Dynamic Exam Hall Allocation (Streamlit)

This section shows the **Streamlit-based visualization module** used for validating and demonstrating:
- Student distribution across halls
- Course-wise scheduling
- Staff invigilator assignment
- Disabled student seating adjustments
- Lab room allocation logic
- Room reuse efficiency and conflict checks

Each screenshot below represents a **verification step** from the hall allocation pipeline.

| Screenshot Name | Description | View Screenshot |
|-----------------|-------------|-----------------|
| **Student_Overview** | Shows total students and breakdown of disabled vs non-disabled students. | [View Screenshot](Hall_Allocation/Student_Overview.jpg) |
| **Student_Details_Filter** | Filters students by disability status (All / Disabled / Non-Disabled). | [View Screenshot](Hall_Allocation/Student_Details_Filter.jpg) |
| **Course_Overview** | Displays count of UG and PG courses available. | [View Screenshot](Hall_Allocation/Course_Overview.jpg) |
| **Course_Summary_Table** | Lists all courses included in exam scheduling. | [View Screenshot](Hall_Allocation/Course_Summary_Table.jpg) |
| **Subjects_Type** | Shows distribution of Core, Elective, and Lab subjects. | [View Screenshot](Hall_Allocation/hall_allocation_demo/Subjects_Type.jpg) |
| **Staff_Overview** | Shows staff distribution across all departments. | [View Screenshot](Hall_Allocation/Staff_Overview.jpg) |
| **Staff_Summary_Table** | List of all staff members of the university. | [View Screenshot](Hall_Allocation/Staff_Summary_Table.jpg) |
| **Password_Hash_Check** | Verifies that staff and student passwords are hashed, not stored in raw form. | [View Screenshot](Hall_Allocation/Password_Hash_Check.jpg) |
| **Rooms_Overview** | Displays buildings, floors, total rooms, and total seating capacity. | [View Screenshot](Hall_Allocation/Rooms_Overview.jpg) |
| **Rooms_Table** | Detailed list of rooms with seat capacity and accessibility attributes. | [View Screenshot](Hall_Allocation/Rooms_Table.jpg) |
| **Timetable_Main** | Main timetable filtering dashboard (select course/semester/session). | [View Screenshot](Hall_Allocation/Timetable_Main.jpg) |
| **Timetable** | Timetable for a specific course and exam session. | [View Screenshot](Hall_Allocation/Timetable.jpg) |
| **Timetable_Summary** | Complete timetable list for all courses and sessions. | [View Screenshot](Hall_Allocation/Timetable_Summary.jpg) |
| **Lab_Verification** | Confirms that lab exams are allocated to lab rooms only. | [View Screenshot](Hall_Allocation/Lab_Verification.jpg) |
| **Lab_Verification_Table** | Lists lab subjects and their assigned lab rooms. | [View Screenshot](Hall_Allocation/Lab_Verification_Table.jpg) |
| **Staff_Assignment_Verification** | Shows staff assigned to each exam hall and session. | [View Screenshot](Hall_Allocation/Staff_Assignment_Verification.jpg) |
| **Staff_Conflict_Check** | Detects if any staff is assigned to two halls in the same session. | [View Screenshot](Hall_Allocation/Staff_Conflict_Check.jpg) |
| **Staff_Multiple_Session_Details** | Lists staff handling multiple sessions to ensure workload balance. | [View Screenshot](Hall_Allocation/Staff_Multiple_Session_Details.jpg) |
| **Allocation_Chart** | Visual progress chart verifying 100% student seat allocation. | [View Screenshot](Hall_Allocation/Allocation_Chart.jpg) |
| **Allocation_Verification** | Checks for unallocated students and verifies seat mapping. | [View Screenshot](Hall_Allocation/Allocation_Verification.jpg) |
| **Disabled_Student_Floor_Verification** | Confirms disabled students are seated only on first floor. | [View Screenshot](Hall_Allocation/Disabled_Student_Floor_Verification.jpg) |
| **Room_Reusability_Analysis** | Shows efficient re-use of rooms across multiple sessions. | [View Screenshot](Hall_Allocation/Room_Reusability_Analysis.jpg) |
| **Room_Allocation_Details** | Displays seating assigned to each room per session. | [View Screenshot](Hall_Allocation/Room_Allocation_Details.jpg) |
| **Student_Details_Check_Filter** | Search/filter by Student ID to verify hall assignment. | [View Screenshot](Hall_Allocation/Student_Details_Check_Filter.jpg) |
| **Student_Details_Check** | Detailed student allocation (course, session, class). | [View Screenshot](Hall_Allocation/Student_Details_Check.jpg) |
| **Student_Timetable_Check** | Final student-specific timetable verification view. | [View Screenshot](Hall_Allocation/Student_Timetable_Check.jpg) |

## 3. Mobile Application Screenshots

| Screenshot Name | Description | File Location |
|-----------------|-------------|---------------|
| **App_Main_Page** | Main page with 3 options: Scan QR, Store Fingerprint, Authenticate Fingerprint. | [View Screenshot](output/mobile/App_Main_Page.jpg) |
| **StudentId_Verification** | Student ID entered before proceeding to QR/fingerprint actions. | [View Screenshot](output/mobile/StudentId_Verification.jpg) |
| **QR_Code_Scan** | QR code of hall ticket scanned; triggers dashboard display. | [View Screenshot](output/mobile/QR_Code_Scan.jpg) |
| **Student_Dashboard_Mobile** | Displays student details and timetable in app after QR scan. | [View Screenshot](output/mobile/Student_Dashboard_Mobile.jpg) |
| **Fingerprint_Stored_Success** | Fingerprint successfully stored. | [View Screenshot](output/mobile/Fingerprint_Stored_Success.jpg) |
| **Authentication_Success** | Fingerprint authentication successful. | [View Screenshot](output/mobile/Authentication_Success.jpg) |


## 4. Password Hash Verification
| Screenshot Name | Description | View Screenshot |
|-----------------|-------------|-----------------|
| **Password_Hash_Check** | Verifies that staff and student passwords are hashed, not stored in raw form. | [View Screenshot](Hall_Allocation/Password_Hash_Check.jpg) |

## 5. Access Log Monitoring
| Screenshot Name | Description | View Screenshot |
|-----------------|-------------|-----------------|
| **Access_Log** | Shows anonymized request logs including timestamp, user type, and action performed. | [View Screenshot](Other_Features/Access_Log.jpg) |

## 6. Real‑Time Exam Alerts
Sending instant email notifications to students showing their exam date, time, hall, and building.
(Upcoming enhancement: WhatsApp alerts)
| Screenshot Name | Description | View Screenshot |
|-----------------|-------------|-----------------|
| **Exam_Location_Details_And_Alerts** | Email notification sent to students with exam venue and alert details. | [View Screenshot](Other_Features/Exam_Location_Details&Alerts.jpg) |
