# R_code
#H1N1_DATA_ANALYSIS
library(trackViewer)
## enter the mutation of 2018 isolates

mutation_2018<-GRanges("HA", IRanges(start = c(91,156,181,200,312,320,420,513,524),width = 1, names = c("91/S-R", "156/A-S","181/S-T","200/S-P","312/I-V","320/K-T", "420/I-M", "513/N-S","524/E-D")))

## add genomic features 

features_all<-GRanges("HA",ranges=IRanges(start = c(1,324,330,78,128,156,187,169,206,238,140,224,98,153,183,190,194,195), end=c(323,329,566,83,129,167,198,173,208,240,145,225,98,153,183,190,194,195), names = c("HA1","CS","HA2","Cb","Sa","Sa","Sb","Ca1","Ca1","Ca1","Ca2","Ca2","RBD","RBD","RBD","RBD","RBD","RBD"), fill=c("#AFEEEE","#FF4500","#5F9EA0","#FF69B4","#FFA07A","#FFA07A","#EEE685","#C0FF3E","#C0FF3E","#C0FF3E","#EE7AE9","#EE7AE9","#000000","#000000","#000000","#000000","#000000","#000000"), height=c(0.06,0.06,0.06,0.09,0.09,0.09,0.09,0.09,0.09,0.09,0.09,0.09,0.03,0.03,0.03,0.03,0.03,0.03)))

## create lollipot for 2018

lolliplot(mutation_2018, features_all, ranges=GRanges("HA:1-566"))

mutation_2019<-GRanges("HA",IRanges(start = c(55,91,146,181,200,202,277,312,537),width = 1, names = c("55/N-D","91/S-R","146/N-D","181/S-T","200/S-P","202/T-I","277/N-D","312/I-V","537/V-A")))
features_all

lolliplot(mutation_2018, features_all,ranges = GRanges("HA:1-566"))

#Enter the mutation of 2020 isolates compare to Brisbrane/02/2018

mutation_2020<-GRanges("HA", IRanges(start = c(8,62,146,147,173,178,200,240,267,277,299,315,523),width = 1, names = c("8/L-M","62/G-R","146/N-D","147/K-N","173/N-K","178/L-I","200/T-I","240/R-Q","267/V-A","277/N-D","299/A-P","315/V-I","523/E-D")))

##lolliplot for 2020 isolates
lolliplot(mutation_2020,features_all,ranges = GRanges("HA:1-566"))

## Enter the mutation of 2021 isolates compare to A_Victoria_2570_2019
mutation_2021<-GRanges("HA", IRanges(start = c(71,203,206,240,241,276,325,387),width = 1, names = c("71/K-Q","203/A-T","206/Q-E","240/R-G","241/E-A","276/R-K","325/K-R","387/N-S")))

## Loliplot for 2021 isolates

lolliplot(mutation_2018,features_all,ranges=GRanges("HA:1-566"))

