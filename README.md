# CS211 Timetable Discrete

This Prolog project, named **timetable-fairness-system_discreteStructures**, aims to create a fair timetable for students enrolled in CS211, including the course "Discrete Structures." The system utilizes Prolog to enforce various constraints and provides solutions to specific queries related to exams, instructors, courses, and rooms.

## Getting Started

### Prerequisites

Ensure you have SWI-Prolog installed on your system. You can download it from [SWI-Prolog's official website](https://www.swi-prolog.org/).

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/cs211-timetable-discrete.git
   ```

2. Change into the project directory:

   ```bash
   cd cs211-timetable-discrete
   ```

### Running the Project

1. Load the Prolog environment using SWI-Prolog:

   ```bash
   swipl
   ```

2. Load the knowledge base file:

   ```prolog
   ?- [knowledge_base].
   ```

   Ensure all necessary data is loaded into the system.

3. Execute specific predicates to get answers to the provided queries.

## Project Structure

- `knowledge_base.pl`: Contains Prolog facts about students, instructors, courses, sections, enrollments, teaches relationships, room capacities, and exam timings.
- `queries.pl`: Prolog file with predicates to answer specific queries outlined in the project statement.

## Queries

1. **Query 1:**
   ```prolog
   ?- hasTwoExamsInOneDay(StudentName).
   ```
   
2. **Query 2:**
   ```prolog
   ?- isTeaching(InstructorName, CourseName).
   ```

3. **Query 3:**
   ```prolog
   ?- examsAtSameTime(CourseName1, CourseName2).
   ```

4. **Query 4:**
   ```prolog
   ?- examsAtSameTimeAndRoom(CourseName1, CourseName2).
   ```

5. **Query 5:**
   ```prolog
   ?- canSwitchRooms(Room1, Room2).
   ```

6. **Query 6:**
   ```prolog
   ?- isRoomUsedOnDate(Room, Date).
   ```

7. **Query 7:**
   ```prolog
   ?- haveCommonSection(StudentName1, StudentName2, CourseName).
   ```

8. **Query 8:**
   ```prolog
   ?- hasSameNameWithDifferentRoll(Name).
   ```

9. **Query 9:**
   ```prolog
   ?- teachesTwoSections(InstructorName, CourseName).
   ```

10. **Query 10:**
    ```prolog
    ?- teachesTwoCourses(InstructorName).
    ```

Happy coding!
