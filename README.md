# Career Management System Database and Frontend


This project is designed to support a **Career Management System** (CMS), combining a **MySQL database** and a **React frontend**. The system analyzes students' skills, projects, academic performance, and other factors to generate tailored reports, scoring these against the requirements of a given company. 

## **Project Structure**

### **Backend**
The database schema consists of the following tables:

| Table Name                  | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| **academic_performance**    | Records detailed academic performance metrics for each student.            |
| **additional_info**         | Stores additional information about students or jobs, such as preferences or extra requirements. |
| **companies**               | Maintains a list of companies participating in the career system.          |
| **job_listings**            | Stores details about job openings posted by companies.                    |
| **job_summary**             | its a view which summarizes the status and statistics for jobs listed in the system.        |
| **match_history**           | Tracks the history of job applications and matching between students and jobs. |
| **projects**                | Captures information about projects completed by students.                 |
| **skills**                  | Defines the skills that students can list or jobs can require.             |
| **student_academic_summary**| A view which aggregates academic achievements for each student.                        |
| **student_skill_summary**   | A view which summarizes the skillsets for each student.                                 |
| **students**                | Core table holding primary details about students registered in the system. |

#### **Functions**   
- **`CalculateAcademicScore`**  
- **`CalculateProjectScore`**
- **`CalculateSkillScore.re`**
#### **Procedures**  
- **`CalculateCareerScore`**  
  Calculates using the above functions and returns the suitability score for a student against a specific job.


 





### **Frontend**
The React frontend provides an intuitive interface for interacting with the CMS. Key features include:

- **Dynamic Data Rendering:** Displays students, job listings, and reports in an interactive UI.
- **Form Management:** Allows users to input data such as student details, job postings, and academic records.
- **Tailored Reports:** Compares student profiles with company requirements and provides a match score.
- **Responsive Design:** Ensures compatibility across devices for a seamless user experience.



---

## **Key Functionalities**

1. **Student Data Management**  
   - Tracks detailed student information, academic performance, skills, and projects.
   - Supports a comprehensive summary of academic and skill metrics.

2. **Job Matching and Tracking**  
   - Enables matching students with job listings based on skills and academic profiles.
   - Records the history of job applications and outcomes.

3. **Company Engagement**  
   - Maintains company profiles and their associated job postings.

4. **Comprehensive Reporting**  
   - Aggregates data into summaries, aiding decision-making for students and recruiters.

---

## **Getting Started**

### **Installation**

1. **Clone the Repository**  
   Clone the project repository from GitHub:
   ```bash
   git clone 'https://github.com/Roshr2211/Career-Management-System.git'
   cd Career-Management-System
2. **Database Setup**

Ensure MySQL is installed on your system.
Import the database schema:
```bash
mysql -u your_username -p career_manage < database/schema.sql

```
3. **Backend Setup**
   Navigate to the backend directory and install dependencies:
   ```bash
   npm install
   npm install express mysql cors multer
   ```
   To start. [Run the frontend simultaneously]
   ```bash
   npm start
   ```
   OR install nodemon
   ```bash
   npm install nodemon
   nodemon server.js
   ```
3. Frontend Setup
   Open another terminal and navigate to the career directory and install dependencies:
   ```bash
   npm install
   npm install recharts axios
   ```

```bash
npm run dev
```

## Future Enhancements
AI Integration: Advanced recommendations for students and recruiters.
   
   
   
