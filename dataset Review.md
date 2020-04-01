
# hrdata
Column Name | Column Descriptions
 -------------- |  -----------------
Employee_Name | name of the employee
EmpID | Employee ID
MarriedID | Maried Status
MaritalStatusID | Marital Status
GenderID | Gender ID
EmpStatusID | Employee Status ID
DeptID | Department ID
PerfScoreID | Performance Score ID
FromDiversityJobFairID | diversity job ID
PayRate | Payed per hour
Termd | Served that termed  Terminated date - date of hired date
PositionID | position ID
State | State name
Zip | Zip Code
DOB | Date of birth
CitizenDesc | citizen type
HispanicLatino | Type of race
RaceDesc | Race Type
DateofHire | Hire date 
DateofTermination | termination date
TermReason | reason of quitting
ManagerID | ID of his reporting manager
RecruitmentSource | Source of the recuirment where the employee has been hired
EngagementSurvey | engagment survey
EmpSatisfaction | Employement satisfication
SpecialProjectsCount | Project count that he has been worked
LastPerformanceReview_Date | Last performance review
DaysLateLast30 | any late has been accounted

# departments
Column Name | Column description
 ----------------- |  -----------------
DeptID | Admin Offices
Department | Executive Office

# employmentstatus
*unique employee status*
Column Name | Column description
 ----------------- |  -----------------
EmpStatusID | Active
EmploymentStatus | Terminated for Cause

# gender
*Unique Gender code*
Column Name | Column description
 ----------------- |  -----------------
GenderID | F
Sex | M 

# manager
*manager unique code*
Column Name | Column description
 ----------------- |  -----------------
ManagerID | Brandon R. LeBlanc
ManagerName | Janet King

# maritalstatus
*maritial status code*
Column Name | Column description
 ----------------- |  -----------------
MaritalStatusID | Married
MaritalDesc | Divorced

# performanceScore
*performance of the metrics of each employee*
Column Name | Column description
 ----------------- |  -----------------
PerfScoreID | position ID of each role
PerformanceScore | Position name
 | 

# recruitingcosts
*Recurinting cost involved in monthly basis*
Column Name | Column description
 ----------------- |  -----------------
Employment Source | Source name
January  | month
February | month
March | month
April | month
May | month
June | month
July | month
August | month
September | month
October | month
November | month
December | month
Total | sum of all month

# position
*unique position of the company*
Column Name | Column description
 ----------------- |  -----------------
PerfScoreID | position ID of each role
PerformanceScore | Position name

# productionstaff
*Production of each employee*
Column Name | Column description
 ----------------- |  -----------------
EmpID | 
Abutments/Hour Wk 1 | total charged per week 1
Abutments/Hour Wk 2 | total charged per week 1
Daily Error Rate | error rate on quality detections
90-day Complaints | quality of work

# salarygrid
*salary structure of each employee*
Column Name | Column description
 ----------------- |  -----------------
Position DI | position ID 
Min | salary min range
Mid | salary mid range
Max | salary max range
Min | Hourly Min range
Mid | Hourly mid range
Max | Hourly max range

# hrcore
*all informations of the HR*
Column Name | Column description
 ----------------- |  -----------------
Employee Name | position ID 
Employee Number | Employee Number
State | State
Zip | Zip
DOB | DOB
Age | Age
Sex | Sex
MaritalDesc | MaritalDesc
CitizenDesc | CitizenDesc
Hispanic/Latino | Hispanic/Latino
RaceDesc | RaceDesc
Date of Hire | Date of Hire
Date of Termination | Date of Termination
Reason For Term | Reason For Term
Employment Status | Employment Status
Department | Department
Position | Position
Pay Rate | Pay Rate
Manager Name | Manager Name
Employee Source | Employee Source
Performance Score | Performance Score
