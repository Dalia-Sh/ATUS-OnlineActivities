# ATUS-OnlineActivities - Capstone Project 

## Overview

Since the emergence of the internet, individual's activities have changed, and more online activities have started to take place. Some activities, like reading the newspaper or watching movies, are now being done through the internet. Other activities, like surfing the web for personel interest or checking Twitter, Instagram or Facebook, are new activities that have emerged as a result of the introduction of internet in our day to day life. 


### Measuring the Value of the Internet

The internet's value cannot be measured monetarily, and hence, measuring its contribution to economic growth is challenging. Wallsten's research discusses a novel approach to measuring the value of online activities, by evaluating the opportunity cost of online leisure activity. 

Wallsten evaluates the opportunity cost of online leisure activity by measuring the time forgone on other activities. This is called the 'crowd-out effect'.

He uses a regression equation for each activity and report the computer leisure time coefficient as a measure of crowd out effect (correlation between that activity and online leisure activity).

![equation](https://github.com/Dalia-Sh/ATUS-OnlineActivities/blob/master/Other/equation.png)

### Goal
The goal is to estimate what activities are we forgoing when we are online. By the end of the study, we would be able to measure how one minute of the internet crowds out other activities. The activities are: 

- Leisure (excluding computer)
- Work activities
- Personal care (including sleep)
- Travel
- Household activities
- Education
- Sports
- Helping households members
- Eating and drinking
- Helping non-household members
- Religion
- Volunteer
- Professional care and services
- Household services
- Government and civic obligations
- consumer purchases
- Phone calls

## My Methodology

A summary of the methodology is provided in the table below.

![summary](https://github.com/Dalia-Sh/ATUS-OnlineActivities/blob/master/Other/summary.png)

### Data
We use the ATUS (American Time Use Survey) dataset. ATUS interviews respondents about how they spent their time on the previous day, where they were, and whom they were with. Individuals are randomly selected from a subset of households previousely interviewed in the Current Population Survey (CPS). 

### Subsetting Individuals With Internet Access
The ATUS dataset does not specify who has internet and who doesn't. Thus, the methodology for measuring crowd-out effect cannot rely on the whole dataset.
To subset individuals with internet access, Wallsten used a two-stage regression model similar to the one presented in the following paper: Goldfarb, Avi, and Jeff Prince. "Internet adoption and usage patterns are different: Implications for the
digital divide." Information Economics and Policy 20.1 (2008): 2-15.

I use a different approach, by introducing the CPS dataset (Current Population Survey). Years 2011, 2013 and 2015 of this dataset include information on internet access. I use this dataset to build a decision tree model classifier, and use the algorithm on the ATUS dataset to subset individuals with internet access.

#### Decision Tree Model
- Input: Demographics Variables
- Output: Internet or No Internet

### Measuring crowd-out effect
The last part is similar to Wallsten's approach. I use, however, ATUS years 2011 to 2015, to account for activities such as Facebook, Instagram, Twitter and other, as these have been reported in the ATUS questionaire starting 2011.

## Conclusion
I present (in both the extensive report and the presentation), the results of the study, as well as a comparison with Wallsten's results. 

## Acknowledgment

**I would like to thank Dr. Tamer Abdou for supervising this capstone project during the Spring 2017 term.** 
