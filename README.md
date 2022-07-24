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

        Inner workings of the pay column

## Data Analysis Carried out
Before I started the analysis I formatted my table to make things easier. This is actually one of the first steps before you start anything

After that, I carried out data analysis on the data set to gain insights to answer some questions which are
* Who is the highest paid employee?
* Who is the least paid employee?
* What is the total amount of money paid to employees?
* What is the average hourly wage?

### Who's the highest paid employee?
To find out who that was, I used to MAX function on the pay column to find the maximum value.

![image](https://user-images.githubusercontent.com/109159668/180645003-f1ebb273-7f6c-43e3-a8d3-3685151c22c1.png)

        MAX function

With that I could easily identify the employee with the highest pay. Turns out Lily Tiana is breaking the bank.

![image](https://user-images.githubusercontent.com/109159668/180645036-ee09ddf6-643f-4da8-b33d-0309bedb202a.png)

        The highest paid employee

Who's the least paid employee?
To find out who that is, I used the MIN function. It's the opposite of the MAX function.it returns the smallest numerical value.

![image](https://user-images.githubusercontent.com/109159668/180645053-b93ef9d7-279c-4eb9-8f1e-bd7043da1676.png)

        MIN function

With this function, I could easily identify the least paid employee as Ruby Beatrice. Maybe I'll have a talk with Ruby to ask whether she's ok with the amount she makes

![image](https://user-images.githubusercontent.com/109159668/180645077-e4988535-f4cd-4374-bab2-1819657d4ffe.png)

        The least paid employee

### Total of money paid to employees
To find the total amount of money paid to employees, I used the SUM function to sum the pay column

![image](https://user-images.githubusercontent.com/109159668/180645116-7d8ddf04-8bde-4e0b-abf2-710c79e4f365.png)

        SUM function

After that, I pressed enter and the total came up immediately. Take a look at the amount of money given out on a weekly basis, that's a lot of money.

![image](https://user-images.githubusercontent.com/109159668/180645133-9bbc69d9-e482-4fe9-a9f0-3d555e0e698f.png)

        Total amount paid per week

What is the average hourly pay?
I wanted to know the average hourly pay of the employees.to achieve this I used the AVERAGE function. This function carries out arithmetic mean on a given set of numbers.

![image](https://user-images.githubusercontent.com/109159668/180645160-9b48ebe2-674b-4c01-913c-cab0b8a79e46.png)

        AVERAGE function

After that, I press enter and the average shows up immediately. With this I now know that I pay an average of #73.13 per hour to my employees.

![image](https://user-images.githubusercontent.com/109159668/180645179-56918c29-7faf-4af3-925e-b9a4d547bb4f.png)

        Average amount of money paid for hourly wages

### Conclusion
In conclusion, I've been able to carry out some data analysis on dataset I formed by myself. This is my first article and I'll be building on this project over time. I'll really appreciate feedback and suggestions, thank you.


















