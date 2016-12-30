# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data


```r
activity <- read.csv('activity.csv')
```


## What is mean total number of steps taken per day?

1. Calculate the total number of steps taken per day

```r
step_date <- with(activity, tapply(steps, date, sum, na.rm=TRUE))
```

2. Plot a histogram of the total number of steps taken each day

```r
hist(step_date, main="Steps per day", xlab="Steps")
```

![](PA1_template_files/figure-html/unnamed-chunk-3-1.png)<!-- -->

## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
