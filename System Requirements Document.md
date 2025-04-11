### System Requirements Document

#### Functional Requirements
- **Register and Login**: Users must register using a school domain; passwords must meet security requirements. No duplicate users allowed. Admin registration requires OTP verification.
- **Functional Buttons and Widgets**: Buttons such as INSERT, ADD, EDIT, BACK, FORWARD, SUBMIT, and DELETE must work.
- **Submission System**: Learners must submit work to the database or a repository. Teachers will mark assignments and provide feedback within the system.
- **Reports Generation**: System generates performance reports for learners.
- **Automatic Updates**: Updates will occur on school premises.
- **AI Integration**: Learners will be allowed to use AI with the system.
- **Instant Messaging System**: The system will include a messaging feature.
- **Admin Controls**: Admins can delete users.
- **Collaboration**: Learners can share work with peers.
- **Save and Resume**: Learners can save progress and continue later.
  
&nbsp;

#### Non Functional Requirements
- **Aesthetics**: Professional home page with high-quality login and register links.
- **Performance**: Fast application performance capable of handling concurrent users.
- **Navigation**: User-friendly interface with intuitive navigation.
- **Security**: Uses school emails with hashed passwords (MD5 or better).
- **Browser Compatibility**: Works across all major browsers.
- **Operating System Support**: Web version supports all OS; app version supports Android & iOS.
- **Hosting**: Hosted on a reliable provider like GoDaddy or HostGator.
- **Maintenance**: Scheduled during off-peak hours with prior user notifications.
- **Documentation & Updates**: Developers must maintain thorough documentation and collect user feedback.
- **Communication**: Channels between users, system administrators, and developers must be maintained.

&nbsp;

###  Traceability Matrix
| **Category**              | **Requirement ID** | **Requirement Description**                                | **Stakeholders Addressed**                                      |
|---------------------------|--------------------|------------------------------------------------------------|-----------------------------------------------------------------|
| Functional Requirements   | FR1               | Secure User Registration & Login via School Domain         | Learners, Teachers, System Administrators, Backend Developers  |
|                           | FR2               | Assignment Upload, Submission, and Feedback Workflow       | Learners, Teachers                                              |
|                           | FR3               | Instant Messaging System for Teacher-Learner Interaction   | Learners, Teachers                                              |
|                           | FR4               | AI Integration for Learning Support                        | Learners, Backend Developers                                    |
|                           | FR5               | Performance Reports Generation for Learners                | Learners, Teachers, Department of Education                    |
|                           | FR6               | Collaboration Feature for Learners to Share Work           | Learners                                                        |
|                           | FR7               | Save and Resume Work Capability                            | Learners                                                        |
|                           | FR8               | Functional UI Buttons (INSERT, ADD, SUBMIT, DELETE, etc.)  | Learners, Teachers, Frontend Developers                         |
|                           | FR9               | Admin Controls Including User Deletion                    | Teachers (Admins), System Administrators                       |
|                           | FR10              | Automatic System Updates within School Network             | System Administrators                                           |
| Non-Functional Requirements | NFR1.1           | Professional UI Design with Clear Navigation               | Learners, Teachers, Frontend Developers                         |
|                           | NFR1.2            | Cross-Browser Compatibility                                | Learners, Teachers                                              |
|                           | NFR2.1            | Web and Mobile Platform Support (Android & iOS)           | Learners, Teachers, IT Administrators                          |
|                           | NFR2.2            | Secure Hosting via Reliable Provider                       | IT Administrators, Backend Developers                           |
|                           | NFR3.1            | Strong Passwords and Email Hashing (MD5 or better)         | System Administrators, Regulatory Bodies                       |
|                           | NFR3.2            | Regular Maintenance with Advance Notifications             | System Administrators, Teachers, Learners                      |
|                           | NFR4.1            | High Performance with Fast Response Times                  | Learners, Teachers                                              |
|                           | NFR4.2            | Scalability for Concurrent Users                           | Developers, IT Administrators                                   |
|                           | NFR5.1            | POPIA Compliance and Data Security                         | Regulatory Bodies, System Administrators                       |
|                           | NFR5.2            | Continuous Feedback Collection and Developer Documentation | Developers, Teachers, Learners                                  |
|                           | NFR6.1            | Uptime Guarantee and Reliability (99.9% or higher)         | Learners, Teachers, System Administrators                      |
|                           | NFR6.2            | Consistent Communication Channels for Support              | Teachers, System Administrators, Developers                    |
