# SQLproject
Practicing some SQL by querying a table in a database I found on Kaggle. 
I created a database called "students" and then crated a table called "students_performance". Then I imported the dataset into MySQL. This dataset compares the test scores of students (male & female) who took test prep courses as well as seeing if there is a correlation between test scores and the educational background of their parents. Each student is broken into groups based on their parents education level.
The groups are as follows:
GROUP A: Associate's degree
GROUP B: Bachelor's degree
GROUP C: Some college
GROUP D: High School
GROUP E: Master's Degree

I took some screenshots of the database, table and queries that I wrote to find answers to questions asked (keep in mind there are 1000 rows of data so I limited the return to 20 using a LIMIT clause so the viewer could get an idea of data in each row and the various columns) When I wrote the queries, it still extracts data from all 1000 rows even with a LIMIT clause. I want to see if there is a correlation between taking a test prep course vs. not, but also if the educational background of your parent plays a part in the test scores. I picked this dataset because I thought is relevant to the current state of our education system and could open a serious dialogue. The data also includes whether the student recieved a free/reduced rate lunch vs. a standard meal plan. I believe that could play a part in test scores too - poverty has an overwhelming affect on the quality of education. I found students who's parent's had at least a bachelors degree or higher scored higher than those whose parents had a high school diploma or lower. After examining the data this hit home because I grew up with friends who lived in poverty or weren't as fortunate as my family was. When you're a kid you don't look at the bigger picture of test scores and how poverty affects education rates. 

This is an ongoing project of mine. My next step is too import this into a Jupyter notebook file and use Pandas to create a visual and play around with some neat tools.

Some sample queries: 

1. Create a database called "students" 

![image](https://user-images.githubusercontent.com/75811937/110142546-47582680-7da4-11eb-85ee-3579d6d48013.png)

2. Created a table called "students_performance". Verified the table was created - here's the table schema. The Kaggle dataset was imported into MySQL I wanted to make sure to match the columns in the .csv file to prevent any errors in MySQL during the importing process.

![image](https://user-images.githubusercontent.com/75811937/110142398-1f68c300-7da4-11eb-88ae-78841d3b457c.png)

3. If we want an overall view of our data (columns & rows) - Writing a query to select all columns from the table limiting to 20 for purposes of space (there are 1000 rows total)
![image](https://user-images.githubusercontent.com/75811937/110142911-a9b12700-7da4-11eb-9a15-05cd01eb507a.png)

4. How many students are male & female? Writing a query to find out how many students are male & female - should equal 1000 since there are 1000 entries

![image](https://user-images.githubusercontent.com/75811937/110144329-37d9dd00-7da6-11eb-9e6e-a431edcc6e26.png)

5. Writing a query using the count() function to count the educational level of each parents
![image](https://user-images.githubusercontent.com/75811937/110146195-47f2bc00-7da8-11eb-8446-b8c5978e5bc4.png)

6. Finding the average test scores (all 3 subjects) for male students with all parental education backgrounds. Placed levels of education alphabetically
![image](https://user-images.githubusercontent.com/75811937/110148426-cb151180-7daa-11eb-8b8d-0602632f3f6a.png)

7. Same as #6 for females
![image](https://user-images.githubusercontent.com/75811937/110148713-29da8b00-7dab-11eb-9f3a-26baf0241799.png)

8. How many students have a free/reduced rate lunch and standard lunch?
![image](https://user-images.githubusercontent.com/75811937/110149856-88eccf80-7dac-11eb-8f5c-6b24497c340a.png)

9. How many students didn't complete a test preperation course?
![image](https://user-images.githubusercontent.com/75811937/110150797-a9695980-7dad-11eb-9ba1-c839cc4bc007.png)

10. How many students completed a test preperation course?
![image](https://user-images.githubusercontent.com/75811937/110150977-e3d2f680-7dad-11eb-8c54-313a86c7edff.png)

11. the average scores of those who took the test preperation course vs. those who didn't
![image](https://user-images.githubusercontent.com/75811937/110151844-f437a100-7dae-11eb-9c45-22a9ff5f2af4.png)

12. If we want to know the first 20 scores of each subject
![image](https://user-images.githubusercontent.com/75811937/110152412-b38c5780-7daf-11eb-8608-e2de394a90cf.png)

13. Writing a query to find all scores greater(>) than 70
![image](https://user-images.githubusercontent.com/75811937/110152887-4dec9b00-7db0-11eb-9df9-97ebbead0c08.png)

14. Writing a query to find the highest math score - using the Max() function

![image](https://user-images.githubusercontent.com/75811937/110153370-f6026400-7db0-11eb-8fed-c6526f3ed7b4.png)

15. Finding the lowest math score - using Min() function

![image](https://user-images.githubusercontent.com/75811937/110153470-1500f600-7db1-11eb-93f0-6ac745d33223.png)

16. How many students are male & female? Use the Count() function to figure this out! 

![image](https://user-images.githubusercontent.com/75811937/110153893-9c4e6980-7db1-11eb-842f-3fecf75138c6.png)
 
 17. Used a CASE Statement to see which scores are pass/fail. I learned of a CASE Statement recently and thought it was neat way to add some Boolean logic to a query and to add a bit of complexity to it. Created a conditional statement stating that if a score is equal to 70 or above, the status of "Pass" will appear. Anything lower than 70, will display a status of "Fail, must take again". When the query is run, it will go through each row based on the criteria I set and will determine what message to display based on the score. Used LIMIT to display the first 20 results just to get an idea of how this method works and for the purposes of space.

![image](https://user-images.githubusercontent.com/75811937/110509160-ccf31380-80cf-11eb-8e7b-08d56a1457f0.png)





