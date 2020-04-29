# analyez-csv-sample

## Overview
This repository is csv data sample.  
Purpose of sample is data processing through executing from command line.  

## Source of data
Sample data was taken from the following.  
https://people.sc.fsu.edu/~jburkardt/data/csv/csv.html

Sample data is biostats data, and file name is "biostats.csv".


## Sample command
```sh
$ curl -s https://raw.githubusercontent.com/tweeeety/analyez-csv-sample/master/sample.csv | awk -F"," '{print $1 ":" $2}'
```

