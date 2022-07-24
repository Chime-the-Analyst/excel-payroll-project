# Project Name: Excel Payroll Project

I did a project using Microsoft Excel. It's a beginner project and this is its documentation.

## Project Background
The project is a payroll spreadsheet of a hypothetical company. I'm the manager of that company and I oversee the payment of the employees.

## Steps taken to get dataset ready
The dataset is fictional and I made up the values. I got the names used in the dataset online. I google baby names and copied and pasted them in a word document.

![image](https://user-images.githubusercontent.com/109159668/180644722-07623049-e4f3-44c3-9a22-dd634e5650c3.png)

    Baby names in word document

I then copied and pasted the names into my spreadsheet but there was a problem. It copied with numbers, full stop and space.

![image](https://user-images.githubusercontent.com/109159668/180644757-7530039d-747c-488d-a76e-8a4b5ab2a4de.png)

    Names when copied to spreadsheet

To resolve this, I used the MID function to take the part of the text string that I needed. I specified the text that I wanted to use, my starting point and how many letters I need. I used 9 for the number of letters because I felt most names are less than 9 letters and also because my name is 9 letters and it's a really long name.


    The MID function in action

After I dragged the formula down the column, I noticed another issue. I noticed that as the formula gets to 2 digit numbers, it started returning the space in front of the text and 3 digit numbers like 100 started to return wrong outputs too. Since I said the formula should start from the fourth character, it returned the full stop and empty space with the numbers.

![image](https://user-images.githubusercontent.com/109159668/180644811-60b86455-3157-4bc1-a94a-2a4bd763c9a9.png)

        MID function used with double digits

![image](https://user-images.githubusercontent.com/109159668/180644819-2ecec143-fd30-48ac-a5ff-e8bae87d737b.png)

        MID function used with 3 digits

There are many ways to solve this problem, I chose to concentrate on the ones with full stop. So I used the MID function again to remove the full stop. Then I went ahead to use the TRIM function from the top to remove any leading or trailing spaces.

![image](https://user-images.githubusercontent.com/109159668/180644836-5c38ac30-6944-4289-ba2f-018746b4b400.png)

        TRIM function being used

So with that taken care of, I went ahead to create another column for last names with the same process. Then I added a phone number column to make the dataset realistic. I used the RAND BETWEEN function to create a list of numbers from a certain range.

![image](https://user-images.githubusercontent.com/109159668/180644852-b36e1ef2-7b38-4554-bbf5-2b1c0142588a.png)

        RAND BETWEEN function

Then I added the hourly wage column which is the amount of money the employees are paid per hour. I used 8 different rates to give the dataset some form of variety.

![image](https://user-images.githubusercontent.com/109159668/180644871-c5cd8510-fe6e-4e1a-840e-ceb8cb1f7f1f.png)

        Creating the hourly wage column

Then I added an hour worked column to show the amount of hours worked by employees for the week. The maximum amount of hours an employee can work in a week is 40 hours but some employees did overtime which means they worked extra hours.

![image](https://user-images.githubusercontent.com/109159668/180644887-14221dea-9cc9-487c-88b9-ddd397ffe650.png)

        RAND BETWEEN function in hours worked column

Then finally, I added the pay column, which is a calculated column. The pay is the hours worked multiplied by the hourly wage.

![image](https://user-images.githubusercontent.com/109159668/180644909-abead806-51a6-482b-b736-9a6bfaf632b5.png)


































