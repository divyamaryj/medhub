
<p align="center">
  <img src="https://github.com/user-attachments/assets/a4c1d91b-e67f-4e39-9679-171b6fea2b30" alt="Screenshot_22-2-2026_153419 " width="100%">
</p>

# MedHub 🎯

## Basic Details

### Team Name: SYNTAX ERROR

### Team Members
- Member 1: Devika Anil - College of Engineering,Kallooppara
- Member 2: Divya Mary John - College of Engineering,Kallooppara

### Hosted Project Link
https://medhub-phi.vercel.app/

### Project Description
MedHub is a web-based hospital resource management system that provides real-time visibility into critical resources like ICU beds, ventilators, and medicines. It enables administrators to update availability and allows patients to quickly check hospital status for better decision-making during emergencies.



### The Problem statement
Hospitals often lack a centralized, real-time system to share resource availability, causing delays, confusion, and difficulty for patients in finding timely care.



### The Solution
MedHub offers a simple platform where hospitals can update resource data instantly and patients can view availability in one place, improving transparency and reducing response time.


## 🔄 Application Workflow

1. Admin logs in
2. Admin enters resource data
3. Server stores data in database
4. Patients open dashboard
5. System fetches live data via API
6. Resources displayed instantly

---


## Technical Details

### Technologies/Components Used

- Frontend: HTML, CSS, JavaScript
- Backend: Node.js, Express
- Database: SQLite
- Styling: Glass UI + CSS


## 🚀 Features

- 👨‍⚕️ Admin portal to update hospital resources
- 🧑‍🤝‍🧑 Patient dashboard for live viewing
- 🏥 Multi-hospital support
- 📊 Department ranking display
- 💾 Persistent database (SQLite)
- 🌗 Dark / Light theme toggle
- 🔒 Admin login
- ⚡ Real-time data access via API
- 🎨 Premium glass UI



#### Screenshots (Add at least 3)

![Screenshot1]Homepage
It shows the main homepage of the web 'MEDHUB'
<img width="1910" height="915" alt="1" src="https://github.com/user-attachments/assets/b929c744-63f5-4501-b260-1b0ed468fbf1" />



![Screenshot2]Login Page-Admin
It shows the login page for the admin corner
<img width="1910" height="915" alt="2" src="https://github.com/user-attachments/assets/7f45ade0-82af-48a2-aec7-3debbb03fb23" />



![Screenshot3]Login page-Patient
it shows the login page for the patient/user corner
<img width="1910" height="915" alt="3" src="https://github.com/user-attachments/assets/13371bd8-d847-4fc0-8b1e-7efa3f0ecad5" />


#### Diagrams

**System Architecture:**
        ┌──────────────┐
        │   User        │
        │ (Browser)     │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │  index.html   │
        │ Landing Page  │
        └──────┬───────┘
        ┌──────┴───────────────┐
        │                      │
        ▼                      ▼
┌──────────────┐      ┌────────────────┐
│ signup.html  │      │ patient.html   │
│ Admin Login  │      │ Patient View   │
└──────┬───────┘      └──────┬─────────┘
       │                      │
       ▼                      │
┌──────────────┐              │
│ admin.html   │              │
│ Admin Panel  │              │
└──────┬───────┘              │
       │                      │
       └──────────┬───────────┘
                  ▼
            ┌───────────┐
            │  app.js   │
            │ JS Logic  │
            └─────┬─────┘
                  ▼
            ┌───────────┐
            │ server.js │
            │ Backend   │
            └─────┬─────┘
                  ▼
            ┌───────────┐
            │ database  │
            │ SQLite DB │
            └───────────┘

**Application Workflow:**

START
  │
  ▼
User opens website
(index.html)
  │
  ├───────────────┐
  │               │
  ▼               ▼
Admin chooses     Patient chooses
Admin Corner      Patient Corner
  │               │
  ▼               ▼
signup.html       patient.html loads
(Admin login)     │
  │               │
Login success     App requests data
  │               │
  ▼               ▼
admin.html        server.js fetches
(Admin dashboard) database records
  │               │
Admin enters      ▼
ICU / Beds /      Patient sees
Antivenom /       live resources
Departments       │
  │               │
  ▼               │
app.js sends      │
update request    │
  │               │
  ▼               │
server.js updates │
database.db       │
  │               │
  └───────Data available────────┘
  │
  ▼
END


Admin Workflow

Admin logs in through signup page

Admin opens dashboard

Enters hospital resource data

System sends update to backend

Database stores information

Patient Workflow

Patient opens dashboard

System fetches data from server

Live hospital resources displayed

### GET /hospitals

**Description:** Fetch all hospital resource data

**Response:**
```json
[
  {
    "id": 1,
    "name": "City Hospital",
    "icu": 10,
    "beds": 50,
    "antivenom": 5,
    "emergency": "Active",
    "departments": "Cardiology, ICU"
  }
]
---
{
  "name": "City Hospital",
  "icu": 10,
  "beds": 50,
  "antivenom": 5,
  "emergency": "Active",
  "departments": "Cardiology, ICU"
}
{
  "status": "success"
}
```

## AI Tools Used (Optional - For Transparency Bonus)

If you used AI tools during development, document them here for transparency:

**Tool Used:**  GitHub Copilot ,ChatGPT, Claude

**Purpose:** [What you used it for]
  Debugging assistance for async functions
  Code review and optimization suggestions

**Key Prompts Used:**
- "Create a REST API endpoint for user authentication"
- "Debug this async function that's causing race conditions"
- "Optimize this database query for better performance"

**Percentage of AI-generated code:** [Approximately X%]

**Human Contributions:**
- Architecture design and planning
- Custom business logic implementation
- Integration and testing
- UI/UX design decisions

*Note: Proper documentation of AI usage demonstrates transparency and earns bonus points in evaluation!*

---

## Team Contributions

- Devika Anil - Frontend development, API integration,documentation
- Divya Mary John - Backend development, Database design,testing

---

## License

This project is licensed under the [LICENSE_NAME] License - see the [LICENSE](LICENSE) file for details.

**Common License Options:**
- MIT License (Permissive, widely used)

---

Made with ❤️ at TinkerHub
