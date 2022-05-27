# Pewlett-Hackard-Analysis

## Overview

The Purpose of this analysis was to use pgAdmin 4 to determine the number of retiring employees per title, as well as to identify the employees who are eligible to participate in a mentorship program. 

My objective is to create a report to help prepare for the "silver tsunami", i.e. the retirement exodus, due to the amount of current employees reaching retirement age.

## Focal Pain Points for Deliverable 1:

For Deliverable 1, the task at hand is to create tables that hold all the titles of the employees born between January 1, 1952 and December 31, 1955. There also was a determination to me made to the amount of retirement age employees by their recent job titles (i.e. to_date = '9999-01-01'...meaning "still employed")

According to the data, there are 72,458 total positions that will be available due to the amount of employees retiring.  As expected, Senior positions, such as Senior Engineer, Senior Staff, etc are approximately 2/3 the sample set.  This would make sense, since the elder statesmen in a company tend to have senior positions, due to the plethora of experience they come with.

![retiring_titles](https://user-images.githubusercontent.com/8845050/170622953-2b94a2c7-5a92-4b17-aaf0-49e9dfe6b379.PNG)

On the other side, I see that only 2 Managers, 1,090 Asst. Engineers, and 3.603 Technique Leaders are up for retirement.  This could be explained similar to above sentiment, where many have migrated to more senior roles, have already retired, etc.  Further analysis would be to examine eaqch position without current status as a factor, to see when the average age(or count(YEAR(TO_DATE)) to assess if there has been a recent "silver tsunami" broken out by position.   This could lead to forecasted hiring events being needed.

## Focal Pain Points for Deliverable 2:

![image](https://user-images.githubusercontent.com/8845050/170624931-3bb590a9-949b-4715-9a72-f3b11f1707a3.png)

Above is an illustration of a more customized view of Deliverable 1's RETIREMENT_TITLES analysis.  I have highlighted that there have been title changes amongst the staff, and sorted from most recent to least recent, to show that a career's natural progression, from "Staff" to "Senior Staff" happens, which would explain the Deliverable 1 conjecture of majority of retirees being from senior positions.

## Unique Titles:

This is exactly the assessment that I was talking about!  The below picture shows where the HOT ZONES of positions with potential retirement exodus may exist.  This is important for corporations to maintain productivity and backfill staff employment....but no counts.  Just a preliminary staging table for the analysis to follow.  This is the RAW DATA for the next analysis, where tabulation would occur.

![unique_titles](https://user-images.githubusercontent.com/8845050/170625390-e3960e3e-65d1-470c-9c09-74bcfcab2061.PNG)

As you can see, duplicates have been removed, i.e. employees only showing CURRENT ROLE and all fields, respectively,  to allow for a thorough analysis.

# WRAP UP

Based on the large amount of employees retiring, it is suggested that Pewlett-Hackard attempt to recoup the expected "silver tsunami" of lost employees to retirement.  The mentorship eligibility program has 1549 eligible "internal replacements", but that does NOT begin to address the vast amount 72,458 employees.  That is a ration of about 47:1, employees : mentor.  That is not a lot of hands on internal cultivation.  Possible remedies could be 1) internal training for staff to move up 2) external recruitment for more qualified backfill employment, and 3) widen the job scopes to allow for overlapping and more peer to peer training, holistically.


###Resources

Postgres (PG ADMIN 6.8)
Postgres 11.16
Visual Studio Code

![image](https://user-images.githubusercontent.com/8845050/170626430-204531ad-b7bf-433c-b08f-a4fabba62993.png)

