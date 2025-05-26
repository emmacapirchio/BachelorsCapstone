# BachelorsCapstone

BreakScheduleApp
A role-based iOS app for managing staggered break schedules, shift swaps, and internal team messaging — powered by SwiftUI and CloudKit.

Overview
BreakScheduleApp is designed to help retail and team-based workplaces manage break schedules more efficiently. Team Members can view and request shift swaps, while Team Leads and Store Directors can approve or deny those requests. The app includes built-in messaging and role-based access control.

Features
Role-Based Login (Apple Sign-In and username/password)
Shift & Break Scheduling
Shift Swap Requests and Approvals
Team Messaging by Department
iCloud Sync via CloudKit
(Planned) PDF export and AWS integration

Technology Stack
Layer	Tech
Front-End	SwiftUI
Back-End	CloudKit (Apple's iCloud DB)
Language	Swift
Database	CloudKit NoSQL Records
Versioning	GitHub
Deployment	Xcode + CloudKit
(Optional)	AWS S3, Lambda, Cognito

Folder Structure
BreakScheduleApp/
├── App/
├── Extensions/
├── Models/
├── Services/
├── ViewModels/
├── Views/
└── README.md

CloudKit Schema
Record Type and	Description
User - Stores account info & role
BreakSchedule - Stores employee shifts and breaks
SwapRequest - Records shift swap proposals
Message - Stores in-app messages by department

iCloud container ID: iCloud.com.ecapirchio.BreakSchedule

Setup Instructions
1. Clone the Repo
git clone https://github.com/emmacapirchio/BreakScheduleApp.git
2. Open in Xcode
Open BreakScheduleApp.xcodeproj

Set your signing team under Signing & Capabilities

Enable CloudKit and select the container:
iCloud.com.ecapirchio.BreakSchedule

3. Build & Run
Use a physical device or simulator

Sign in with Apple ID or use test credentials (if applicable)

Team & Contributors
Name	Role
Emma Capirchio	Developer, Designer, Project Lead

License
This project is for academic use as part of the Senior Project course. Not licensed for commercial use.
