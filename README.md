
# Table of Contents

1. [Problem Statement Details](#problem-statement-details)
2. [Technology Stack](#technology-stack)
3. [Main Idea](#main-idea)
   - [Features]
   - [UML Screenshot]
4. [Installation & Usage](#installion--usage)
   - [Prerequisites]
   - [Clone Repository]
   - [Virtual Environment]
   - [Install Dependencies]
   - [Apply Migrations]
   - [Create Superuser]
   - [Run the App]
   - [Demo User Setup]
   - [Logout]
   - [Home Page]
5. [Modules](#modules)
   - [Teams]
   - [Projects]
   - [Tasks]
   - [Dashboard](#the-dashboard)
      - [Graphs]
      - [Top Tasks]
      - [Unassigned Tasks]
      - [User's Projects]
      - [User's Teams]

# PROBLEM STATEMENT DETAILS
| Problem Statement ID              | 1369                           |
|-----------------------------------|--------------------------------|
| Problem Statement Title           | Online integrated platform for projects taken up by the students of various universities/colleges |
| Description                       | Innovation is the key to betterment of education and students in the Indian universities/colleges put a lot of efforts on the projects as a part of the academic requirements. If a common knowledge platform (with a facility for plagiarism) is created to bring all project works taken up at various levels by the students in Technical / Higher Educational Institutes and Universities throughout the country, then it will be a great source of knowledge and also will help the student community to take up unique/innovative project works Summary: An integrated platform should be developed where in all the universities/Colleges provide information about the projects done by the students. The information on this platform will help in the peer learning and this will also help in cross functional research between various universities/colleges. Objective: To develop an online integrated platform for projects taken up by the students of various universities/colleges. |
| Organization                      | Government of Jharkhand          |
| Category                          | Software                         |
| Domain Bucket                     | Smart Education                  |

# Technology Stack
| Python |
|--------|
| Django|
|Sqlite3 / Mysql|
|Bootstrap v4.5.0|




# Installion & Usage
## Make sure you have the following installed:
- Python3

## 1. **Clone the repository:**
   
## 2. Create a virtual environment (optional but recommended):
```
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```
## 3. Install dependencies:
```
pip install -r requirements.txt
```
## 4. Apply migrations:
```
python manage.py makemigrations
python manage.py migrate
```
## 5. Create Super user aka admin:
```
python manage.py createsuperuser
```
## 6. Run the App
Start the development server:
```
python manage.py runserver

Now make click on edit this user and click on checkbox which says Demo User.
## 7. Logout 
## 8. Home Page
Visit http://127.0.0.1:8000/ in your browser (This page is for users aka students).


# Modules
## Teams
Teams are made up of members, and every team has a leader. Team leaders have
special privileges like being able to assign tasks to other team members and
changing the members of the team. 

## Projects
Every project is assigned to a team and thus has members and a leader associated
with it. A project can only be assigned to one team but a team can have many
projects. Once a project is over it can be marked as completed.

user that the task is
assigned to, but may also be done by the team leader.

## The Dashboard
One of the main features of the site is the user's dashboard.
Currently this shows six key tables, though this may change in the
future.

### 1 & 2 ) Graphs
There are two graphs , 1st one shows technologies used in all projects and the 2nd one shows all active v/s completed projects.
Note: Graph data is independent of user, i.e it shows graphs for all available projects in database.

### 3) Top tasks
This is a list of the user's top seven tasks, tasks are ranked firstly by due
date and then by priority (in other words the highest priority task that is due
today is at the top).

### 4) Unassigned tasks
A list of the top seven unassigned tasks from projects where the user is the
team leader, again sorted by due date and priority.

### 5) User's projects
A list of all active projects the user is a part of.

### 6) User's teams
A list of teams the user is a part of.
