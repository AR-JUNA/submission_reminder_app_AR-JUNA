**Submission Reminder System**  
A little helper to keep us on track!  

This simple but mighty shell script checks who’s turned in their assignments and who still owes us their work. It’s our friendly, no-stress way to send gentle nudges before deadlines sneak up.

### How It Works  
Our reminder system follows a simple flow:

startup.sh → The big red “Start” button . Run this, and the whole process begins.

app/reminder.sh → The brain . Reads our configuration and checks the submissions.

modules/functions.sh → The toolbox . Holds functions like check_submissions that do the actual checking.

config/config.env → Our settings board . We tell it which assignment to check and how many days are left.

assets/submissions.txt → Our class list  with all names, assignments, and statuses.

### File Structure  
---  
submission_reminder_TEAM/  
├── app/  
│   └── reminder.sh  
├── assets/  
│   └── submissions.txt  
├── config/  
│   └── config.env  
├── modules/  
│   └── functions.sh  
└── startup.sh  

---

### Prerequisites  

Unix-like OS (Linux or macOS)  

Bash shell installed  

Getting Started  

Run the main script:  

---  
./startup.sh  

---  

What you’ll see:  

The script checks assets/submissions.txt and prints a list of who hasn’t submitted the chosen assignment yet.  

---  
Example Output:  

Assignment: Shell Navigation  
Days remaining to submit: 2 days  
--------------------------------------------  
Checking submissions in ./assets/submissions.txt  
Reminder: Chinemerem has not submitted the Shell Navigation assignment!  
Reminder: Divine has not submitted the Shell Navigation assignment!  
Reminder: Daniel has not submitted the Shell Navigation assignment!  
Reminder: Olivia has not submitted the Shell Navigation assignment!  

---  

### Our Student List  

Here’s the exact list we worked with:  

student, assignment, submission status  
Chinemerem, Shell Navigation, not submitted  
Chiagoziem, Git, submitted  
Divine, Shell Navigation, not submitted  
Anissa, Shell Basics, submitted  
Aline, Git Basics, submitted  
Kevin, SQL Queries, not submitted  
Naomi, HTML & CSS, submitted  
Patrick, Machine Learning, not submitted  
Grace, Cloud Computing, submitted  
Daniel, Shell Navigation, not submitted  
Clara, Data Visualization, submitted  
Victor, Shell Navigation, submitted  
Samuel, Artificial Intelligence, not submitted  
Olivia, Shell Navigation, not submitted  

### Customizing  

Change the assignment to check:  
---  

# config/config.env  
ASSIGNMENT="Python"  
DAYS_REMAINING=3  

---  
Update the list of students:  

Edit assets/submissions.txt in the same name, assignment, status format.  

### Contact:  

Made with  by the team  

Name: Arjuna Caleb Gyan  

Email: a.gyan@alustudent.com 
