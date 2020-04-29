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

