## **Submission Reminder System**

*A little helper to keep us on track!*

This simple yet powerful shell script keeps tabs on assignment submissions, showing who’s submitted their work and who still needs a friendly nudge. It’s a no-pressure reminder system to help everyone stay ahead of deadlines.

---

### **How It Works**

Our reminder system follows a straightforward process:

* **`startup.sh`** → The big red “Start” button. Run this to kick things off.

* **`app/reminder.sh`** → The brain. Reads our config and checks who’s submitted what.

* **`modules/functions.sh`** → The toolbox. Contains functions like `check_submissions` that handle the core logic.

* **`config/config.env`** → Our settings board. Here we define which assignment to check and how many days remain.

* **`assets/submissions.txt`** → Our class list. Contains all names, assignments, and submission statuses.

---

### **File Structure**

```
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
```

---

### **Prerequisites**

* Unix-like OS (Linux or macOS)
* Bash shell installed

---

### **Getting Started**

To run the script, simply execute:

```
./startup.sh
```

---

### **Example Output**

```
Assignment: Shell Navigation
Days remaining to submit: 2 days
--------------------------------------------
Checking submissions in ./assets/submissions.txt
Reminder: Chinemerem has not submitted the Shell Navigation assignment!
Reminder: Divine has not submitted the Shell Navigation assignment!
Reminder: Daniel has not submitted the Shell Navigation assignment!
Reminder: Olivia has not submitted the Shell Navigation assignment!
```

---

### **Our Student List**

This is the current dataset in use:

```
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
```

---

### **Updating the Student List**

To make changes, edit the `assets/submissions.txt` file using the same format shown above.

---

### **Customization**

To adjust which assignment the script checks and set the deadline, edit the `ASSIGNMENT` variable in `config/config.env`.

---

### **Contact**

**Name:** Arjuna Caleb Gyan

**Email:** a.gyan@alustudent.com
