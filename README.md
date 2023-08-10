# J124 Final Project: A Data Analysis and Visualization of Long COVID in the United States
## By Piper Melnick
### Data Analysis Process
*  Start by downloading the 9link9 post-COVID conditions dataset from the CDC and then uploading to google drive and opening in google sheets<br>

_These are 5 analysis questions on the dataset and a step-by-step guide on how to recreate them_ <br>
<br>
**Question 1: Which state had the highest percentage of adults affected by long COVID?** <br>
**_Step-by-step Answer:_** <br>
<br>
1. Filter the main sheet so it only contains data pertaining to states, and filter the indicator to only contain "Ever experienced long COVID, as a percentage of all adults" <br>
<img width="1075" alt="q1step1" src="https://github.com/pmelnick13/finalproject/assets/140004443/eb295a0f-8ccc-4ec7-88e6-d06832705107"> <br>
2. Then paste the filtered data into a new sheet in the workbook to edit<br>
<img width="473" alt="Screenshot 2023-08-09 at 12 25 13 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/611aff4b-80f0-4590-9ee7-54197a518969"> <br>
3. Use the formula depicted below to find the average percentage of adults affected from each phase, and then copy and paste the formula to find the average for each state <br>
<img width="1162" alt="Screenshot 2023-08-09 at 12 25 51 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/00b7eeb6-beb3-4550-b398-6b64cefe0ace"> <br>
4. Create a new column of these averages by copy and pasting "value only" (this way the functions won't be affected during sorting). I then moved the decimal point to the tenth for easier viewing, and then filtered the sheet by the average percentage to exclude any blanks. <br>
<img width="256" alt="Screenshot 2023-08-09 at 12 26 07 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/07ce752d-592e-47d4-b20a-438601e14d14"> <br>
<img width="1669" alt="Screenshot 2023-08-09 at 12 36 09 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/6cc69056-bb3a-4418-8310-473e4f17e6d6"> <br>
5. Finally, sort the sheet by the non-function average column from Z-A. <br>
<img width="930" alt="Screenshot 2023-08-10 at 10 11 10 AM" src="https://github.com/pmelnick13/finalproject/assets/140004443/02fa5016-eb07-4dec-8f12-945ad9da4fde"><br>
**The state with the highest percentage of adults affected by long COVID is West Virginia**<br>
<br>
**Question 2: Which phase in the last year (7/27/22-7/10/23) had the highest average percentage of adults who experienced long COVID??** <br>
**_Step-by-step Answer:_** <br>
<br>
1. Filter the main sheet so it only contains phases with the aforementioned dates (phase 3.5-3.9) and filter the indicator to only contain "Ever experienced long COVID, as a percentage of all adults" <br>
<img width="694" alt="Screenshot 2023-08-09 at 1 03 16 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/539e1592-26d9-42e5-a3a5-60bd51002858"> <br>
2. Create a new sheet with this data and then insert a pivot table. Place "value" in the values, summarized by average, and then place "phase" in the rows, ordered by ascending and sorted by the average value <br>
<img width="234" alt="Screenshot 2023-08-09 at 1 06 00 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/b007a58a-f984-4b4a-9f9c-1db51f6dbe42"> <br>
<img width="232" alt="Screenshot 2023-08-09 at 1 05 55 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/7807844a-6071-4bc0-8f1e-e1f271f9fed8"> <br>
**The phase in the last year with the highest percentage of adults who experienced long covid was the most recent phase, 3.9**<br>
<br>
**Question 3: What race/ethnicity had the highest average percentage of adults most affected by long covid across all phases?** <br>
**_Step-by-step Answer:_** <br>
<br>
1. Filter the main sheet so the "group" is by race/ethnicity and filter the indicator to only contain "Ever experienced long COVID, as a percentage of all adults". Then copy this data into a new sheet to work on. <br>
<img width="1314" alt="Screenshot 2023-08-09 at 1 09 45 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/39dc41aa-7748-4847-bb29-c06b31582c62">
2. Insert a pivot table into this new sheet. Place "value" in the values, summarized by average, and then place "subgroup" in the rows, ordered by descending and sorted by the average value. I also added "phase" into the rows, because I was interested in what phase had the highest percentage of those affected within each average, but this is not necessary <br>
<img width="228" alt="Screenshot 2023-08-09 at 1 12 17 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/3b3403a6-6eeb-446a-8415-23f4fcca8a8b"> <br>
<img width="436" alt="Screenshot 2023-08-09 at 1 12 27 PM" src="https://github.com/pmelnick13/finalproject/assets/140004443/9f677e76-7526-4ac7-a123-ef21464da03a"> <br>
**The race/ethnicity in the last year with the highest percentage of adults who experienced long covid was those who are non-Hispanic and other races/multiple races**<br>
<br>
**Question 4: What was the difference in average percentage of adults affected by long covid across all phases between adults who had disabilities vs. adults who didn’t?** <br>
**_Step-by-step Answer:_** <br>
<br>
1. Filter the main sheet so the "group" is by disability status and filter the indicator to only contain "Ever experienced long COVID, as a percentage of all adults". Then copy this data into a new sheet to work on. 
<img width="949" alt="Screenshot 2023-08-10 at 7 47 35 AM" src="https://github.com/pmelnick13/finalproject/assets/140004443/9ceb73c9-407c-435f-8463-367e9056fef0"> <br>
<img width="693" alt="Screenshot 2023-08-10 at 7 49 38 AM" src="https://github.com/pmelnick13/finalproject/assets/140004443/660adbc6-9c04-481d-a4fb-4a0e78d9db70">
2. Insert a pivot table into this new sheet. Place "value" in the values, summarized by average, and then place "subgroup" in the rows, ordered by descending and sorted by the average value. To find the difference, I then added a cell with the function (b2-b3)
<img width="431" alt="Screenshot 2023-08-10 at 7 51 13 AM" src="https://github.com/pmelnick13/finalproject/assets/140004443/5b4bcdff-f8b3-4b55-b8f1-c024076c548f"> <br>
**The difference in the average percentage of adults affected by long covid across all phases between adults who had disabilities vs. adults who didn’t was 9.1%** <br>
<br>





