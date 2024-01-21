# 4.3.4 LAB: A Leap Year

* In a Gregorian calendar, a normal year consists of 365 days, because the time required for the earth to revolve once about the sun is actually 365.2425 days. A "leap year" of 366 days is used once every 4 year and any year that is evenly divisible by 4
  is a leap year, for example 1988, 1992, and 1996 are leap years.
* However, there still a small error that must be accounted for. To eliminate error, the Gregorian calendar stipulates that year that is evenly divisible by 100 is a "leap year" only if it is also evenly divisible by 400.
* For this reason, the following years are not leap years:
  1700, 1800, 1900, 2100, 2200, 2300, 2500, 2600
  This because they are evenly divisible by 100 but not 400. The following years are leap years: 1600,2000,2400. This is because they are evenly divisible by both 100 and 400.

## How To Determine Whether a Year is a Leap Year
### Let's examine the codes what really happen behind the scenes:

```python
def is_year_leap(year):
  if year % 4 != 0:
    return False
  elif year % 100 !=:
    return True
  elif year % 400 != 0:
    return False
  elif:
    return True

test_data = [1900,2000,2016,1987]
test_result = [False, True, True, False]
for i in range(len(test_data)):
  yr = test_data[i]
  print(yr,"->",end="")
  result = is_year_leap(yr)
  if result == test_results[i]:
    print("OK")
  else:
    print("Failed")

```
### Let's broken down the code into pieces so we have a better understandings.
* Using if statements to check whether the year is division by 4, 100, and 400.
* The code also using for loop to test each data inside the list.
* Inside the function where the divison happens.
* Lastly, the if statement to compare the results.

#### Let's work with the function structure first
```python
def is_year_(year):    #The name of the function and its parameter needed whish is the year
if year % 4 !=0        #If the year divide by 4 the answer not 0, it will return False.
  reutn False
elif year % 100 !=0:   #If the year divide by 100 the answer not 0, it will return True.
  return True
elif year % 400 !=0:   #If the year divide by 400 the answer not 0, it will return False
  return False
elif:                  #If all the if statement go opposite answer, it will return True.
  return True
```
  
#### In this lab, it have 2 class variables, to store the data we want to test which is the years and the result to compare between the result we get from the functions.
```python
test_data = [1900,2000,2016,1987]
test_result = [False, True, True, False]
```

#### Inside the for loop, where all the mixing taking place from variable, to for loop and function, lastly, if statement for the result comparing.
```python
for i in range(len(test_data)):
  yr = test_data[i]
  print(yr,"->",end="")
  result=is_year_leap(yr)
  if result == test_results[i]:
    print("OK")
```
#### Let


