# analyez-csv-sample

## Overview
This repository is csv data sample.  
Purpose of sample is data processing through executing from command line.  

## Source of data
Sample data was taken from the following.  
https://people.sc.fsu.edu/~jburkardt/data/csv/csv.html

Sample data is biostats data, and file name is "biostats.csv".

>biostats.csv, 
>biometric statistics for a group of office workers. There are 18 records, recording Name, Sex, Age, Height, Weight There is an initial header line.

## Sample command

### only curl
```sh
$ curl -s https://raw.githubusercontent.com/tweeeety/analyez-csv-sample/master/sample.csv
Name,Sex,Age,Height (in),Weight (lbs)
Alex,M,41,74,170
Bert,M,42,68,166
Carl,M,32,70,155
Dave,M,39,72,167
Elly,F,30,66,124
Fran,F,33,66,115
Gwen,F,26,64,121
Hank,M,30,71,158
Ivan,M,53,72,175
Jake,M,32,69,143
Kate,F,47,69,139
Luke,M,34,72,163
Myra,F,23,62,98
Neil,M,36,75,160
Omar,M,38,70,145
Page,F,31,67,135
Quin,M,29,71,176
Ruth,F,28,65,131
```

### curl + awk

```sh
$ curl -s https://raw.githubusercontent.com/tweeeety/analyez-csv-sample/master/sample.csv | awk -F"," '{print $1 ":" $2}'
Name:Sex
Alex:M
Bert:M
Carl:M
Dave:M
Elly:F
Fran:F
Gwen:F
Hank:M
Ivan:M
Jake:M
Kate:F
Luke:M
Myra:F
Neil:M
Omar:M
Page:F
Quin:M
Ruth:F
```

