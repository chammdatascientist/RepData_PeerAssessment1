# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data

data <- read.csv(file = "activity.csv", header = TRUE,
                 +                   colClasses = c("numeric","Date","numeric"))

## What is mean total number of steps taken per day?

mean_steps <- aggregate(data$steps,list(day=data$date),mean)

## What is the average daily activity pattern?

hist(mean_steps$x)

## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
