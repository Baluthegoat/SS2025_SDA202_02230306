# Assignment Submission and Grading System

## Interaction Overview Diagram

1. **Student Submits Assignment**:
   - **Actors**: Student
   - **Interaction**: Student uploads code to the GitHub repository.

2. **Automated Grading System**:
   - **Actors**: Professor
   - **Interaction**: Professor clones the student's repository, runs the code locally and grades it based on predefined criteria.

3. **Plagiarism Detection**:
   - **Actors**: Plagiarism Detection System (TurnItIn)
   - **Interaction**: The system compares the student's submission with other submissions and checks for plagiarism using a web-based service.

4. **Grade Submission**:
   - **Actors**: LMS
   - **Interaction**: The system submits the grades to the university's LMS.

5. **Audit**:
   - **Actors**: Admin
   - **Interaction**: The grades and submissions are audited by a state-based regulatory body each year.

### Context Viewpoint

- **Students**: Uploads assignments to GitHub and can submit multiple attempts to improve the grades.
- **Professor**: Runs and grades the student's code, checks for plagiarism, and submits grades to the LMS.
- **Plagiarism Detection System**: Compares submissions for plagiarism.
- **LMS**: Receives and stores grades.
- **Regulatory Body**: Audits grades annually.

### Functional Viewpoint

- **Assignment Submission**: Student uploads the code to GitHub.
- **Professor**: Clones the repository, runs the code, and grades it based on metrics/tests set
- **Plagiarism Detection**: The system checks for plagiarism by comparing submissions and using a web-based service.
- **Grade Submission**: The system submits grades to the LMS.
- **Audit**: Grades are audited by a regulatory body each year.

### Summary

The university's automated grading system for SWE courses involves multiple actors and interactions. Students submit assignments to GitHub, where professor clones the repository, runs the code, and grades it based on criteria set. The system also checks for plagiarism using a web-based service like Turnitin. Grades are then submitted to the university's LMS, which is mainframe-based and difficult to modify. Professors set the grading criteria and due dates, and students can submit multiple attempts to improve their grades. The grades are audited annually by a state-based regulatory body. Despite budget constraints, the university aims to maintain its high performance in SWE education.

[Click to view interaction overview diagram](./IoD.jpg)

[Click to view Use case diagram](./Use_case.jpg)

[Click to view functional Viewpoint](./Functional%20Viewpoint.jpg)
