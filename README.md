# AlmaMate

About the Project

College placement seasons are stressful, and students often struggle to find actionable advice or secure referrals from alumni working in their target companies. Existing platforms suffer from the "cold start" problem—getting graduates to sign up for a new platform is difficult.

AlmaMate solves this by capturing users during their college years. By integrating into daily campus life, students build their profiles early. Upon graduation, the system automatically transitions their roles from "Student" to "Alumni," retaining the user base and creating a rich, self-sustaining database of professional connections.

✨ Key Features

🔄 Automated User Lifecycle: Profiles seamlessly transition from "Junior" to "Senior" to "Alumni" based on the graduation year, preventing data duplication and retaining users.

🏢 Company & Alumni Discovery: Search for alumni by their current company, industry, or role to seek targeted guidance.

🤝 Mentorship & Referrals: Built-in workflows for students to request mock interviews, resume reviews, or professional referrals.

💬 Real-Time Chat: Secure, in-app messaging powered by Socket.io, allowing students and alumni to connect without sharing personal phone numbers.

🧠 Smart Matching: Python-driven recommendation engine suggesting relevant alumni based on a student's skills and target career path.

🛠️ Technology Stack

Frontend (Mobile App):

Kotlin (Android Native)

Retrofit (API Networking)

EncryptedSharedPreferences (Security)

Backend (API & Logic):

Python & Flask

Flask-JWT-Extended (Authentication)

Flask-Limiter (Rate Limiting & Security)

Database & Real-Time:

MySQL (Relational Data & Unified User Schema)

SQLAlchemy (ORM)

Socket.io (Real-Time Messaging)

📂 Project Structure

├── android-app/          # Kotlin source code, XML layouts, and Retrofit interfaces
├── backend/              # Python Flask APIs, auth logic, and recommendation scripts
├── database/             # MySQL schema definitions and dummy data scripts
└── docs/                 # Architecture diagrams and API documentation


🚀 Getting Started

Prerequisites

Android Studio

Python 3.9+

MySQL Server

Local Setup

Clone the repository:

git clone https://github.com/yourusername/AlmaMate.git


Database Setup:
Run the schema.sql file located in the /database folder in your local MySQL instance.

Backend Setup:

cd backend
pip install -r requirements.txt
flask run


Frontend Setup:
Open the /android-app folder in Android Studio, sync Gradle, and run it on an emulator.

🔒 Security Implementations

DPDP Act Compliant: Explicit consent flows and strict data minimization.

Encrypted Storage: JWTs are stored securely on the device using Google Tink.

Brute-Force Protection: IP-based rate limiting on all authentication and search endpoints.
