"# MOODDAIRY"
#Basic Details
#Team Name:
Tech Titans
#Team members
1.Aiswarya V A-[SCHOOL OF ENGINEERING CUSAT]
2.Arya jayaprasad-[SCHOOL OF ENGINEERING CUSAT]
#Hosted Project Link
https://mooddairy-6yoe.vercel.app/
#Project Description
This project is a Mood Diary and Calendar Tracker that allows users to record daily moods and visualize them on a calendar. It helps users reflect on their emotions and track mood patterns over time.
#The problem statement
Many people struggle to remember their emotional patterns or reflect on their mental well-being. There is no simple, visual way to track daily moods and understand emotional trends.
#The solution
This project provides a calendar-based mood tracker where users can:
-Select mood for each day
- Add notes
- Visualize mood trends
- Reflect on emotional patterns
-It makes mood tracking simple and visual.
#Technical Details
#Technologies/components used
For software:
-Languages used:[HTML,CSS,Javascript]
Frameworks used:
- No framework (vanilla web development)
Libraries used:
- LocalStorage (for mood storage)
- JavaScript DOM manipulation
Tools used:
- VS Code
- Browser Developer Tools
-Git (optional)
For Hardware: (Not applicable for this project)
- No hardware components required
- Works on any modern browser
#features
Mood Calendar Tracking – Users can select a date and record mood
- Color-Coded Calendar – Each mood is shown with different colors
- Mood Notes & Messages – Simple messages for emotional reflection
- Refresh & Clear Options – Users can reset or update moods easily
- Responsive Design – Works on mobile and desktop
#Implementation
Installation
No installation required. Just open the HTML file in a browser.
If using Git (optional):
Bash
Copy code
git clone <repository-link>
Run
Open the project folder and double-click:
Copy code

index.html
OR
Open with live server in VS Code:
-Install Live Server extension
-Right-click index.html
-Click “Open with Live Server”
#No Dependencies for hardware
- Pure HTML, CSS, JavaScript
- Works in modern browsers
-No npm or backend needed
#Project Documentation
For software:
![Screenshot_21-2-2026_182229_127 0 0 1](https://github.com/user-attachments/assets/c82807ab-6f2c-40a1-9ab3-8e2e44bbb05e)
This shows the main calendar view where users can select dates and view mood colors.
![Screenshot_21-2-2026_181630_127 0 0 1](https://github.com/user-attachments/assets/eccf9ae5-fc3b-43c3-b6ee-2abb980a0d71)
This shows the mood selection modal where users can pick a mood and save it.
![Screenshot_21-2-2026_181939_127 0 0 1](https://github.com/user-attachments/assets/ba9e0a65-4cc7-491a-bcb6-3ef81428a491)
This shows how the mood is saved and reflected in the calendar.
#Diagrams
#System Architecture:
#Architecture Diagram
+----------------------+
            |     User Browser      |
            | (HTML, CSS, JavaScript) |
            +----------+------------+
                       |
                       v
            +----------------------+
            |   Mood Calendar UI     |
            | (Calendar & Modal)      |
            +----------+------------+
                       |
                       v
            +----------------------+
            |  LocalStorage (Browser) |
            | Stores mood data locally |
            +----------+------------+
                       |
                       v
            +----------------------+
            |  Data Rendering Layer   |
            | Colors calendar cells    |
            +----------------------+
  The system consists of:
- Frontend (HTML, CSS, JavaScript)
- Browser LocalStorage (stores mood data)
- Calendar Grid (visual representation)
- User Interaction Layer (select date & mood)
Explanation
User selects a date
Mood is stored in LocalStorage
Calendar updates color
Data remains in browser (no server needed)
Tech Stack Interaction
Frontend → LocalStorage → Calendar UI
Application Workflow:
+-------------------+
       |   Open Calendar    |
       +---------+---------+
                 |
                 v
       +-------------------+
       |   Click a Date     |
       +---------+---------+
                 |
                 v
       +-------------------+
       |  Select Mood       |
       +---------+---------+
                 |
                 v
       +-------------------+
       |   Save Mood        |
       +---------+---------+
                 |
                 v
       +-------------------+
       | Update Calendar    |
       | with Color & Note  |
       +---------+---------+
                 |
                 v
       +-------------------+
       |  Mood Stored in    |
       |  LocalStorage      |
       +-------------------+
  The system consists of:
-Frontend (HTML, CSS, JavaScript)
- Browser LocalStorage (stores mood data)
- Calendar Grid (visual representation)
- User Interaction Layer (select date & mood)
Explanation
User selects a date
Mood is stored in LocalStorage
Calendar updates color
Data remains in browser (no server needed)
Tech Stack Interaction
Frontend → LocalStorage → Calendar UI
Additional Documentation
🔹 Current Version (Frontend Only)
This project does not use a backend server.
All mood data is stored locally in the browser using LocalStorage.
There are no external APIs or database connections in the current implementation.
✅ Sample API Documentation (If You Add Backend Later)
If you upgrade your project with backend (Node.js / Express), your API section can look like this:
🔹 API Documentation
Base URL
Copy code

https://api.moodwall365.com
🔹 Endpoints
1️⃣ GET /api/moods
Description:
Fetch all saved moods for the user.
Parameters:
date (string) – Optional – Get mood for specific date
Response:
JSON
Copy code
{
  "status": "success",
  "data": [
    {
      "date": "2026-02-21",
      "mood": "happy",
      "note": "Feeling positive today!"
    }
  ]
}
2️⃣ POST /api/moods
Description:
Save a new mood entry.
Request Body:
JSON
Copy code
{
  "date": "2026-02-21",
  "mood": "happy",
  "note": "Had a productive day"
}
Response:
JSON
Copy code
{
  "status": "success",
  "message": "Mood saved successfully"
}
3️⃣ DELETE /api/moods/:date
Description:
Delete mood entry for a specific date.
Response:
JSON
Copy code
{
  "status": "success",
  "message": "Mood deleted"
}
💡 Caption for README
This API enables storing, retrieving, and managing mood data securely through backend services.
App Flow Explanation
User opens the MoodWall 365 website.
The calendar is displayed.
User selects a specific date.
User chooses a mood (Happy, Sad, Angry, Excited, Neutral).
Mood is saved.
Calendar cell changes color.
A motivational note appears.
Data is stored in LocalStorage for future visits.
✅ Installation Guide
Since your project is a Web Application, installation is simple.
🌐 For Web Version
Run Locally
Download or clone the project folder
Open index.html
The app runs in your browser
OR
Use VS Code Live Server:
Install Live Server extension
Right-click index.html
Click "Open with Live Server"
📱 Optional: Android APK Version (If You Convert It)
If you wrap it using tools like Capacitor or Cordova:
For Android (APK)
Download APK from [Release Link]
Go to Settings > Security
Enable Install from Unknown Sources
Open APK file
Install and open app
🍎 For iOS (TestFlight – If Published)
Download TestFlight
Open TestFlight invite link
Click Install
Open from Home Screen
💡 Important
Currently, MoodWall 365 is a browser-based web app, not a native mobile app.
Command Reference (CLI Version – Optional)
🔹 Basic Usage
Bash
Copy code
python moodwall.py [options] [arguments]
🔹 Available Commands
Copy code

add [date] [mood]      - Add mood for a specific date
view [date]            - View mood for a specific date
list                   - List all saved moods
delete [date]          - Delete mood for a date
🔹 Options
Copy code

-h, --help             Show help message and exit
-v, --verbose          Enable verbose output
-o, --output FILE      Specify output file path
-c, --config FILE      Specify configuration file
--version              Show version information
✅ Examples
Example 1: Add Mood
Bash
Copy code
python moodwall.py add 2026-02-21 happy
Output:
Copy code

Mood added successfully!
Date: 2026-02-21
Mood: Happy 😊
Status: Saved
Example 2: View Mood (Verbose Mode)
Bash
Copy code
python moodwall.py -v view 2026-02-21
Output:
Copy code

[VERBOSE] Fetching mood data...
Date: 2026-02-21
Mood: Happy 😊
Note: Keep smiling and stay positive!
Status: Success
Example 3: List All Moods
Bash
Copy code
python moodwall.py list
Output:
Copy code

Saved Mood Entries:
--------------------------------
2026-02-20 - Sad 😔
2026-02-21 - Happy 😊
2026-02-22 - Excited 🤩
✅ Demo Output (Advanced JSON Mode)
Bash
Copy code
python moodwall.py -v --format json data.json
Output:
Copy code

[VERBOSE] Loading data...
[VERBOSE] Processing entries...

{
  "status": "success",
  "total_entries": 3,
  "latest_mood": "happy",
  "timestamp": "2026-02-21T10:30:00"
}

[VERBOSE] Operation completed in 0.18s
💡 Important
If your project is only:
✔ HTML
✔ CSS
✔ JavaScript
Then you can simply write:
This project is a web application and does not include CLI tools.
https://github.com/user-attachments/assets/a5238ead-c198-4393-ac56-6060fac656bb
AI Tools Used
d (For Transparency Bonus)
🔹 Tool Used
ChatGPT
🔹 Purpose
UI/UX improvement suggestions
Debugging JavaScript issues
Generating boilerplate code
Designing mood note messages
Improving documentation and README formatting
Suggesting aesthetic styles (colors, gradients, animations)
🔹 Key Prompts Used
“How to refresh only calendar without refreshing whole page?”
“Add snow falling animation using CSS”
“Generate mood note messages for happy, sad, angry, excited, neutral”
“Create system architecture diagram for web app”
“Improve README for hackathon submission”
🔹 Percentage of AI-Generated Code
Approximately 30–40% (mainly UI suggestions and formatting assistance).
🔹 Human Contributions
✔ Complete project idea and concept
✔ Architecture planning
✔ Calendar logic implementation
✔ LocalStorage integration
✔ Mood tracking functionality
✔ Styling customization
✔ Testing and debugging
✔ UI positioning adjustments
✔ Feature decisions and enhancements
🔹 Transparency Note
AI tools were used as assistive development support, not as a replacement for understanding or implementation. All final integration, testing, and feature decisions were done manually.
Arya Jayaprasad
Frontend Implementation
Code Integration & Customization
UI Styling and Layout Adjustments
Testing and Debugging
Aiswarya V A
Code Research & Collection
Feature Integration
Design Improvements
Final Review & Presentation Preparation
  Recommended: MIT License
Very simple and short
Anyone can use, modify, and share your code
They just need to give credit
No complicated rules
