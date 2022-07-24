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









