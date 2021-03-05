# SQLproject
Practicing some SQL by querying a table in a database I found. 
This table is called "students_performance" and compares the test scores of students (male & female) who took test prep courses as well as seeing if there is a correlation between test scores and the educational background of their parents. Each student is broken into groups based on their parents education level.
The groups are as follows:
GROUP A: Associate's degree
GROUP B: Bachelor's degree
GROUP C: Some college
GROUP D: High School
GROUP E: Master's Degree

I took some screenshots of the table - keep in mind there are 1000 rows of data so I limited the return to 20. When I write the queries, it still extracts data from all 1000 rows. I want to see if there is a correlation between taking a test prep course vs. not, but also if the educational background of your parent plays a part in the test scores. I picked this dataset because I thought is relevant to the current state of our education system and could open a serious dialogue. The data also includes whether the student recieved a free/reduced rate lunch vs. a standard meal plan. I believe that could play a part in test scores too - poverty has an overwhelming affect on the quality of education. 

1. Created a database called "students" ![image](https://user-images.githubusercontent.com/75811937/110142546-47582680-7da4-11eb-85ee-3579d6d48013.png)

2. Verified the table was created - here's the table schema
![image](https://user-images.githubusercontent.com/75811937/110142398-1f68c300-7da4-11eb-88ae-78841d3b457c.png)

3. Writing a query to select all columns from the table limiting to 20 for space (there are 1000 rows)
![image](https://user-images.githubusercontent.com/75811937/110142911-a9b12700-7da4-11eb-9a15-05cd01eb507a.png)

4. Writing a query to find out how many students are male & female - should equal 1000 since there are 1000 entries
![image](https://user-images.githubusercontent.com/75811937/110144329-37d9dd00-7da6-11eb-9e6e-a431edcc6e26.png)

5. Writing a query using the count() function to count the educational level of each parents
![image](https://user-images.githubusercontent.com/75811937/110146195-47f2bc00-7da8-11eb-8446-b8c5978e5bc4.png)

6. Finding the average test scores (all 3 subjects) for male students with all parental education backgrounds. Placed levels of education alphabetically
![image](https://user-images.githubusercontent.com/75811937/110148426-cb151180-7daa-11eb-8b8d-0602632f3f6a.png)

7. Same as #6 for females
![image](https://user-images.githubusercontent.com/75811937/110148713-29da8b00-7dab-11eb-9f3a-26baf0241799.png)

8. How many students have a free/reduced rate lunch and standard lunch
![image](https://user-images.githubusercontent.com/75811937/110149856-88eccf80-7dac-11eb-8f5c-6b24497c340a.png)

9. How many students didn't complete a test preperation course
![image](https://user-images.githubusercontent.com/75811937/110150797-a9695980-7dad-11eb-9ba1-c839cc4bc007.png)

10. How many students completed a test preperation course
![image](https://user-images.githubusercontent.com/75811937/110150977-e3d2f680-7dad-11eb-8c54-313a86c7edff.png)

11. the average scores of those who took the test preperation course vs. those who didn't
![image](https://user-images.githubusercontent.com/75811937/110151844-f437a100-7dae-11eb-9c45-22a9ff5f2af4.png)

12. If we want to know the first 20 scores of each subject
![image](https://user-images.githubusercontent.com/75811937/110152412-b38c5780-7daf-11eb-8608-e2de394a90cf.png)

13. Writing a query to find all scores greater(>) than 70
![image](https://user-images.githubusercontent.com/75811937/110152887-4dec9b00-7db0-11eb-9df9-97ebbead0c08.png)

14. Writing a query to find the highest math score
![image](https://user-images.githubusercontent.com/75811937/110153370-f6026400-7db0-11eb-8fed-c6526f3ed7b4.png)

15. Finding the lowest math score
![image](https://user-images.githubusercontent.com/75811937/110153470-1500f600-7db1-11eb-93f0-6ac745d33223.png)

16. How many students are male & female
![image](https://user-images.githubusercontent.com/75811937/110153893-9c4e6980-7db1-11eb-842f-3fecf75138c6.png)
 




