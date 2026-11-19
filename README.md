# Analyzing_Students-_Mental_Health
Used data manipulation skills to perform exploratory data analysis on a dataset around student mental health.

## International Student Mental Health: How Length of Stay Relates to Depression, Isolation & Stress | SQL, PostgreSQL

Used PostgreSQL to explore how length of stay relates to three mental health measures among international students in a university survey: depression (PHQ-9), social connectedness (SCS) and acculturative stress (ASISS).

# CONTEXT
A Japanese international university surveyed its students in 2018. Published research linked social connectedness and acculturative stress to depression in international students. The question here was whether length of stay is also a factor.

# MY ROLE
I wrote and checked the query.

# WHAT I DID
• Filtered the students table to international students with a recorded length of stay
• Grouped by years of stay and counted students in each group
• Calculated the average depression, social connectedness and acculturative stress scores per group, rounded to 2 decimals
• Sorted by length of stay (longest first) to read the pattern across groups
• Returned a 9-row, 5-column summary table: stay, count_int, average_phq, average_scs, average_as

# RESULTS
• 204 international students across 9 length-of-stay groups; group sizes ranged from 1 to 95
• Depression scores were highest at 3 years of stay (9.09), when considering years with more than 5 students
• Depression scores were lowest at 8 years of stay (7.48), when considering years with more than 5 students
• Acculturative stress rise with longer stays until year 6; social connectedness fluctuates around a score of 38 but need more data for longer stays than 5 years
• The longest-stay groups have very few students

# TECH STACK
SQL, PostgreSQL, aggregate functions (COUNT, AVG, ROUND), WHERE, GROUP BY, ORDER BY
