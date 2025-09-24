CUTM Result Portal

A web application built with Flask and MongoDB to manage and view student exam results for CUTM (Central University of Technology & Management). Administrators can insert, update, delete exam records and backlog data, and students can securely view their results, backlogs, and cumulative GPA/batch-specific stats.

🚀 Key Features

Admin dashboard to add / modify / remove exam and backlog records

Student dashboard for secure result viewing and backlog status

GPA calculation and academic statistics

Filtering by batch / semester / course

Export or download data (e.g. results/backlogs) in convenient formats

Role-based access control (admin vs student)

Real-time updates and responsive UI


📁 Repository Structure
.
├── app.py                   # Main Flask application entry point  
├── requirements.txt         # Python dependencies  
├── templates/               # HTML templates (Jinja)  
│   ├── admin_dashboard.html  
│   ├── login.html  
│   └── student_view.html  
├── static/                   # CSS, JS, images  
├── .env                      # Environment configuration (e.g. DB settings)  
└── vercel.json               # Deployment config (if using Vercel)  


🛠️ Setup & Installation
Below are instructions to run the project locally:

Prerequisites:
*Python 3.8+
*MongoDB (local or cloud)
*pip

Steps
1.Clone the repository

git clone <repo-url>
cd Cutm-Result-Portal

2.Create and activate a virtual environment

python -m venv venv
source venv/bin/activate    # (Linux / macOS)
venv\Scripts\activate       # (Windows)

3.Install dependencies

pip install -r requirements.txt

4.Configure environment variables

Copy .env.example (if provided) to .env
Add your MONGODB_URI, SECRET_KEY, and any other needed settings

5.Run the Flask app

python app.py

6.Visit http://localhost:5000 in your browser

🧭 Usage
1.Admin

Log in using admin credentials

Navigate to “Manage Results / Backlogs”

Add, edit, delete exam records

View batch-wise summaries, export data

2.Student

Log in using student credentials

View semester-wise results, GPA, backlog status

Filter results by batch / semester

📦 Dependencies
Notable libraries used:
| Package                | Purpose                                           |
| ---------------------- | ------------------------------------------------- |
| Flask                  | Web framework                                     |
| pymongo / Motor        | Connecting to MongoDB / async ops                 |
| python-dotenv          | Load `.env` settings                              |
| werkzeug / flask-login | Authentication & session handling                 |
| (others)               | Any additional utilities, e.g. export, validation |

