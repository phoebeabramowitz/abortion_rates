##description: Made data into cleaner table
##create csvs for each individual table
##input: Pregnancy_rates_age_race_hispanic_origin.csv
##outputs: pregnancies-all.csv, births-all.csv,
##  abortions-all.csv, losses-all.csv
library(dplyr)

column_names <- c("year","total", "Under 15", "15-19", "15–17", "18–19", "20–24", "25–29",
                  "30–34", "35–39", "40–44")

rates_all <- read.csv("../data/all-races.csv", skip=1,
                         col.names = column_names)

#All Races

#Seperate by outcome and race, so we have age and year
pregnancies_all <-  slice(rates_all,1:20)
births_all <-  slice(rates_all,22:42)
abortions_all <- slice(rates_all,44:64)
losses_all <- slice(rates_all,66:86)

#put csv files in data folder
write.csv(pregnancies_all,"../data/pregnancies-all.csv")
write.csv(births_all,"../data/births-all.csv")
write.csv(abortions_all,"../data/abortions-all.csv")
write.csv(losses_all,"../data/losses-all.csv")


#Rates for White People
rates_white <- read.csv("../data/white.csv", 
                      col.names = column_names)
#Seperate by outcome and race, so we have age and year
pregnancies_white <-  slice(rates_white,1:20)
births_white <-  slice(rates_white,22:42)
abortions_white <- slice(rates_white,44:64)
losses_white <- slice(rates_white,66:86)

#put csv files in data folder
write.csv(pregnancies_white,"../data/pregnancies-white.csv")
write.csv(births_white,"../data/births-white.csv")
write.csv(abortions_white,"../data/abortions-white.csv")
write.csv(losses_white,"../data/losses-white.csv")

#Rates for Black People
rates_black <- read.csv("../data/black-non-hispanic.csv", 
                        col.names = column_names)
pregnancies_black <-  slice(rates_black,1:20)
births_black <-  slice(rates_black,22:42)
abortions_black <- slice(rates_black,44:64)
losses_black <- slice(rates_black,66:86)

#put csv files in data folder
write.csv(pregnancies_black,"../data/pregnancies-black.csv")
write.csv(births_black,"../data/births-black.csv")
write.csv(abortions_black,"../data/abortions-black.csv")
write.csv(losses_black,"../data/losses-black.csv")

#Rates for People of Hispanic Origin of all races
rates_hisp <- read.csv("../data/hispanic-all-races.csv", 
                        col.names = column_names)
pregnancies_hisp <-  slice(rates_hisp,1:20)
births_hisp <-  slice(rates_hisp,22:42)
abortions_hisp <- slice(rates_hisp,44:64)
losses_hisp <- slice(rates_hisp,66:86)

#put csv files in data folder
write.csv(pregnancies_hisp,"../data/pregnancies-hisp.csv")
write.csv(births_hisp,"../data/births-hisp.csv")
write.csv(abortions_hisp,"../data/abortions-hisp.csv")
write.csv(losses_hisp,"../data/losses-hisp.csv")

#when opening data in report, will need to
#coerce numeric columns as numeric becuase they'll be factors

#Generally, how do I call variables and functions
#from other scripts?



