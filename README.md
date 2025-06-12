# Project-2-Decomposing-to-Third-Normal-Form-solution

Download Here: [Project 2 Decomposing to Third Normal Form solution](https://jarviscodinghub.com/assignment/project-2-decomposing-to-third-normal-form-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

This project makes use of the database you installed for the first project. If you have not
modified the data or schemas associated with the original tables that were installed when
you imported the database, you should be able to begin with the existing database.
Otherwise, reinstall the employee database as described in Project 1.
This project will use interview grading. 40% of your grade will be based on the
submitted materials. The remaining 60% will come from the interview portion. You
must schedule an interview slot with a grader. If you do not schedule or attend a slot the
interview portion will be scored zero.
Procedure
You will be given a table derived from the employee database and a set of functional
dependencies. You should complete the following steps
1. Create the database table to be decomposed. Execute the following query:
create view base as select dept_manager.emp_no,
departments.dept_no,
dept_name,
dept_manager.from_date as
dept_mgr_from_date,
dept_manager.to_date as dept_mgr_to_date,
title,
titles.from_date as title_from_date,
titles.to_date as title_to_date
from departments, dept_manager, titles
where departments.dept_no =
dept_manager.dept_no and
dept_manager.emp_no = titles.emp_no;
This query yields a view called base that you will need to decompose.
2. What should be the key for this table?
3. You have as inputs the attributes of the base table, the key you just determined,
and the following functional dependencies:
a. If you know the department number, you know the department name.
b. There can only be one department manager at the same time.
c. Each employee can only hold one title at the same time.
4. Derive the 3NF form for this table. Write the proper queries to generate the
decomposed tables as views. You should be able to explain during the grading
interview how you applied the 3NF Synthesis algorithm.
5. Provide the output of each table in a separate file, tar these files together and
submit them to moodle.
There is ambiguity in this specification intentionally. The intent of the assignment is to
gauge your ability to execute this process with fuzzy specs, which is what will happen in
the real world. As a result, there will be variations in the final answers. Grading will be
done based on how you derive the 3NF and how well you execute each of the individual
steps. A sample solution will be published afterwards but this sample serves as a guide
for the grading rather than being the definitive solution.

