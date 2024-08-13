# CRASH-DATA-PROJECT


# Project Title
A brief description of the project- Crash Data

## Problem Statement

This dashboard was made to give the  report of accident in September 2021 .It shows the number of accident occurence in each day, each gender that got involved, the speed limit, and the type of road users daily accident case.

## Questions

1. Total number of accident in each day
2. Average Speed for Each Road User
3. Total Number Of Accident for Each Road User
4. Total Number of Accident for Each Gender
5. Total Number of Accident for Each Dayweek


## Library Used
Numpy

Pandas

Matplotlib


## Steps Followed

STEP 1:
The crash data file was imported from csv file into matplotlib

STEP 2:
The column contents were properly checked

STEP 3:
The Speed Limit column was adjusted. Using replace method,the cells that contains"Unspecified" were changed to 0 and the ones that contains "<40" were changed to 40 and the column type was changed to intrger

STEP 4:
The daily accident occurence was calculated using grouping method.

![Screenshot (2)](https://github.com/user-attachments/assets/8c8d639c-b6fe-4e8a-bbfe-c8c9b9299d53)


STEP 5:
By grouping method,calculation of the average speed limit of each road user was also made


![Screenshot (3)](https://github.com/user-attachments/assets/a62dac2b-a0e5-4000-afa0-71d04bfeaf59)


STEP 6:
I calculated the total accident by each road user

![Screenshot (4)](https://github.com/user-attachments/assets/6ac64d72-4488-4cd3-9830-8ba3d18ab493)


STEP 7:
Estimation of number of total accident by each gender was also made using grouping method

![Screenshot (5)](https://github.com/user-attachments/assets/38d4fa24-bfbc-41c4-83b1-a626d8c77215)



STEP 8:

The average age of each road user was calculated 

![![Screenshot (6)](https://github.com/user-attachments/assets/4d5b30c7-0285-4cec-a186-78dce16dcf12)


STEP 9:
I calculated the total accident occurence in dayweek

![Screenshot (7)](https://github.com/user-attachments/assets/8aee8b2e-7da8-47fd-bcb5-08c05351115f)


STEP 10:
Using matplotlib, a single report page was made to demonstrate "The Crash Accident Report"

STEP 11:
A bar chart illustration was created to reveal the daily accident Estimation

STEP 12:A line chart was made to represent the average speed by each road user

STEP 13:
A horizontal bar was designed to show the accident case by each road user

STEP 14:
A bar chart was made to show the average age of each accident occurnce and the road user

STEP 15:
A pie chart design was created to showcase the percentage of accident in dayweeks to weekends

STEP 16

fig,CR=plt.subplots(nrows=3,ncols=2,figsize=(10,5))
fig.suptitle('CRASH ACCIDENT REPORT',fontsize=16,fontweight='bold',c='r')
plt.tight_layout()
CR[0,0].set(title='ACCIDENT PER EACHDAY')
CR[0,0].bar(a,b)
CR[0,1].set(title='AVERAGE SPEED')
CR[0,1].plot(roadu,spl)
CR[1,0].set(title='ACCIDENT BY ROAD USER')
CR[1,0].barh(accu,accr)
CR[1,1].set(title='ACCIDENT BY GENDER')
CR[1,1].bar(e,f)
CR[2,0].set(title='AVERAGE AGE')
CR[2,0].bar(avgr,avga)
CR[2,1].set(title='ACCIDENT PER DAYWEEK')
CR[2,1].pie(j,labels=i,autopct="%1.0f%%",shadow=True)
plt.tight_layout()
plt.savefig('CRASH DATA REPORT.png')
plt.show()


![Screenshot (8)](https://github.com/user-attachments/assets/21d65abd-7dc0-4f62-8f62-0aeaadfaa151)






