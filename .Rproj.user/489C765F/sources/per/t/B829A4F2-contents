library(readr)
library(ggplot2)
library(dplyr)


# Read datasets/confirmed_cases_worldwide.csv into confirmed_cases_worldwide
confirmed_cases_worldwide <- read.csv("Data.csv", sep = ",")
confirmed_cases_worldwide <- confirmed_cases_worldwide[,1:2]
# See the result
confirmed_cases_worldwide

# Draw a line plot of cumulative cases vs. date
# Label the y-axis
ggplot(confirmed_cases_worldwide, aes (x=Days.after.Jan.21, y=Cases, group = 1)) +
  geom_line()

confirmed_cases_china_vs_world <- read.csv("Data.csv", sep=",")
confirmed_cases_china_vs_world <- confirmed_cases_china_vs_world[,4:7]

confirmed_cases_china_vs_world

# Draw a line plot of cumulative cases vs. date, grouped and colored by is_china
# Define aesthetics within the line geom
plt_cum_confirmed_cases_china_vs_world <- ggplot(confirmed_cases_china_vs_world) +
  geom_line(aes(x=Days.after.Jan.21.1, y=Cumulative.Cases, group=1,color=Is_china)) +
  ylab("Cumulative confirmed cases")

# See the plot
plt_cum_confirmed_cases_china_vs_world


