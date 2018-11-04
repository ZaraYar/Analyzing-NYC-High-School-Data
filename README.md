# Analyzing-NYC-High-School-Data
I am going to explore relationships between SAT scores and demographic factors in New York City public schools. For a brief bit of background, the SAT, or Scholastic Aptitude Test, is a test that high school seniors in the U.S. take every year. The SAT has three sections, each of which is worth a maximum of 800 points. Colleges use the SAT to determine which students to admit. High average SAT scores are usually indicative of a good school. 
New York City has published data on student SAT scores by high school, along with additional demographic data sets. We combine the following data sets into a single, clean pandas dataframe:

- SAT scores by school - SAT scores for each high school in New York City
- School attendance - Attendance information for each school in New York City
- Class size - Information on class size for each school
- AP test results - Advanced Placement (AP) exam results for each high school (passing an optional AP exam in a particular subject can earn a student college credit in that subject)
- Graduation outcomes - The percentage of students who graduated, and other outcome information
- Demographics - Demographic information for each school
- School survey - Surveys of parents, teachers, and students at each school

New York City has a significant immigrant population and is very diverse, so comparing demographic factors such as race, income, and gender with SAT scores is a good way to determine whether the SAT is a fair test. For example, if certain racial groups consistently perform better on the SAT, we would have some evidence that the SAT is unfair.

Before I move into coding, I'll need to do some background research. A thorough understanding of the data will help me avoid costly mistakes, such as thinking that a column represents something other than what it does. Background research will also give me a better understanding of how to combine and analyze the data.

In this case, I'll want to research:

- New York City
- The SAT
- Schools in New York City

Our data

I can learn a few different things from these resources. For example:

- Only high school students take the SAT, so we'll want to focus on high schools.
- New York City is made up of five boroughs, which are essentially distinct regions.
- New York City schools fall within several different school districts, each of which can contains dozens of schools.

Our data sets include several different types of schools. I'll need to clean them so that we can focus on high schools only.

Each school in New York City has a unique code called a DBN, or district borough number.

Aggregating data by district will allow me to use the district mapping data to plot district-by-district differences.

