library(readr)
library(ggplot2)
library(dplyr)
library(tidyverse)

# Read datasets/confirmed_cases_worldwide.csv into confirmed_cases_worldwide
cases_worldwide <- read.csv("total_cases.csv", sep = ",")
cases_worldwide <- cases_worldwide[,]
head(cases_worldwide)

plt_cases_worldwide <- ggplot(cases_worldwide, aes (x=date, y=World, group=1))+
  geom_line()

plt_cases_worldwide

p1 <- ggplot(cases_worldwide, aes(x=date)) + 
  geom_line(aes(y=United.States, group=1, colour='United States'))+
  geom_line(aes(y=Italy, group = 1, colour='Italy'))+
  geom_line(aes(y=China,group=1, colour = 'China'))
p1

p1+scale_y_continuous(trans='log2')

p2 <- ggplot(cases_worldwide, aes(x=date)) + 
  geom_line(aes(y=United.States, group=1, colour='United States'))+
  geom_smooth(method="lm", se = FALSE, fullrange=TRUE)




  