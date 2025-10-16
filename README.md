DocOnDemand is a lightweight telehealth prototype that allows patients to discover doctors by specialty and location, sign up and log in, and book appointments with client-side validation and availability checks.
Built with Node.js + Express for serving the frontend and browser localStorage as a mock data store.
This project showcases an end-to-end flow from doctor discovery → booking → confirmation with a modern, responsive UI.

Features:

👩‍⚕️ Patient Onboarding: Signup with duplicate email check and login using localStorage-based session.

🔍 Doctor Discovery: Filter doctors by specialty and location; book directly from listing.

📅 Appointment Booking:

Client-side validation for input and time slots.

Blocks past dates and enforces a daily cap of 6 appointments.

Supports rescheduling via URL parameters.

🔔 Notifications:

Doctor and patient notifications stored in localStorage.

Tracks new bookings, cancellations, and visit confirmations.

🧑‍⚕️ Doctor Portal:

Hardcoded doctor authentication.

View/sort bookings, manage notifications, and view profile.

💬 Confirmation Screen:

Booking + doctor details modal.

Basic chat widget to log “visit home/no visit” intents.

🎨 Modern UI:

Built with Bootstrap 5 + Google Fonts (Poppins).

Animated particles background for homepage.






| Category     | Technologies Used                                                                  |
| ------------ | ---------------------------------------------------------------------------------- |
| Frontend :   | HTML5, CSS3, Vanilla JavaScript, Bootstrap 5, Google Fonts (Poppins), particles.js |
|  Backend :   | Node.js, Express.js (static file serving)                                          |
|  Storage :   | Browser `localStorage` (patients, bookings, notifications)                         |
|  Tooling :   | npm (`npm start` runs `index.js`)                                                  |






├── index.js              # Express server (serves static files, main route → main.html)
├── package.json          # Node config (express dependency)
├── main.html             # Homepage
├── singup.html           # Patient signup
├── login.html            # Patient login
├── doctors.html          # Doctor discovery + portal
├── booknow.html          # Booking form (validations)
├── afterpayment.html     # Confirmation screen
├── About Us.html         # Static info page
├── Services.html
├── Mental Health.html
├── urgentcare.html
├── pay.html / pay1.html  # Legacy (unused)
├── assets/               # (Recommended) Screenshots, images, and media
└── node_modules/         # Dependencies


How to Run Locally

# Prerequisites
Node.js v18+ installed

# 1️⃣ Install dependencies
npm install

# 2️⃣ Start the server
npm start

# 3️⃣ Open in browser
http://localhost:3000



| Name                | Contribution                                                                                                           |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Srikar  Reddy       | Frontend logic (validation, booking flow, notifications), Express.js setup, and integration of Particles.js animation. 
| Shashi kumar Reddy  | Doctor portal (view/sort bookings, notification management) and appointment scheduling logic.                          |
| Varun Dev           | UI design, page layout (Bootstrap + Poppins), and responsive styling across all modules.                               |
