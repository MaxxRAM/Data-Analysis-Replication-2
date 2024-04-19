# --------------------------------------------------------------------------------------------------------------
# Title: Seasonal change in male reproductive investment of a fish
# 
# Principal investigators:
#  Shingo Fujimoto, Graduate School of Medicine, University of the Ryukyus, Okinawa 903-0125, Japan, fujimoto.s@outlook.com
#
# Date of Data collection:
#  Seasonal change in Gonad-soma index and fin length: 2004/3-2004/11
#  Replicate dataset of seasonal change in Anal-fin length and Dorsal-fin length:2013/4-2013/7
#  Mating experimnt: 2014/6/18-6/21
# 
# Geographic location of data collection: Aomori prefecture, Japan
# Keywords: Life-history adaptation, Seasonality, Oryzias latipes species complex, Sexual dimorphism, Indicator signal
#
# --------------------------------------------------------------------------------------------------------------
# Abstract
# --------------------------------------------------------------------------------------------------------------
Many animals are sexually dimorphic, whereby males may display brighter body coloration and
more distinctive ornamentation than females. Fishes in temperate regions markedly change their energy allocation
toward reproduction in response to the seasonal environment. Seasonal change in reproductive investment affects
the expression of sexually dimorphic traits in males through gonadal weight change.
Here, we report seasonal changes in body size, testis weight and sexual dimorphism of the fins
(anal fin length and dorsal fin length) in the northern medaka Oryzias sakaizumii. Fish were collected periodically
from a wild population (Aomori). Gonad weight increased from May to July in both males and females,
corresponding to the reproductive season. Moreover, during this period, the degree of sexual dimorphism in fin length
increased. To investigate the relationship between testis weight and individual differences in male fin length,
we analyzed relationships among morphological traits using structural equation modeling. In the reproductive season,
increased testis weight was associated with longer fin length in males, but the relationship disappeared
after the reproductive season. These observations suggest that the sexually dimorphic fin in this fish is a mating signal.
Results from a mating experiment also support this view. Males with larger size and/or longer fin attracted
more mates than those with smaller fins, suggesting that sexual selection operates through females choosing to mate
with males having longer fins.

# --------------------------------------------------------------------------------------------------------------
# Data and file overview
# --------------------------------------------------------------------------------------------------------------
Seasonal change in Gonad-soma index(GSI)
 |------- aomoriGSI_data2004.csv(2020/04/01): Wild individual's morphological data, standard length, anal fin length, body weight, and gonad weight
 |------- Fig2_seasonalChange_BW_GSI.R(2020/04/01): Boxplot of the seasonal change in GSI
 |------- Fig4_TableS2_SEM_BW_SL_TW_AFL.R(2020/04/01): The association among morphological traits using structural equation modeling.

Seasonal change in sexual dimorphism in fins, anal-fin length(AFL), and dorsal-fin length(DFL)
 |------- aomoriGSI_data2004.csv(2020/04/01): Wild individual's morphological data, standard length, anal fin length, body weight, and gonad weight
 |------- SLvsFin_Data2013.csv(2020/04/01): Wild individual's morphological data, standard length, body depth, anal fin length, and dorsal fin length.
 |------- Fig3_seasonalChange_AFLandDFLratio.R(2020/08/07): The ratio in AFL or DFL per standard length 

Mating experiment to test the effect of male morphology on reproductive success
 |------- mateNumberAndfertilizationRate.csv(2020/08/14): Egg number, fertilization rate, female size, and male morphological traits in the mating experiment
 |------- Table1_FigS3_mateNumber.R (2020/08/14): Wald test for the mate number and male morphological traits
 |------- Table1_FigS4_fertilizationRate.R(2020/08/14):  Wald test for the fertilization rate and male morphological traits

# --------------------------------------------------------------------------------------------------------------
# Sharing and access information
# --------------------------------------------------------------------------------------------------------------
Attribution License: ODC-By

Users are free to use the database and its content in new and different ways,
provided they provide attribution to the source of the data and/or the database.

# --------------------------------------------------------------------------------------------------------------
# Methodological information: (reference)
# --------------------------------------------------------------------------------------------------------------
Description of methods for data collection or generation: https://doi.org/10.1007/s10641-021-01059-x
The R scripts were written and performed using R version 3.6.1 for Windows (R Core Team, 2019, www.r-project.org/).

# --------------------------------------------------------------------------------------------------------------
# Data-specific information
# --------------------------------------------------------------------------------------------------------------
aomoriGSI_data2004.csv (2020/04/01)
                       |-- year: Year of fish collection
                       |-- month: Month of fish collection
                       |-- ordinal: Julian date of fish collection
                       |-- collectDate: The date of fich collection(YYYY/MM/DD)
                       |-- picID: picture ID for morphological measurement
                       |-- individualID: individual ID for morphological measurement
                       |-- sex: "f" is female, and "m" ins male
                       |-- SLmm: Standard length (mm)
                       |-- AFLmm: Anal fin length (mm)
                       |-- BW_fol: Formalin-fixed body weight (gram)
                       |-- gonadW: Gonad weight (gram)
                       |-- GSI: Gonad-soma index, 100 * Gonad weight per Formalin-fixed body weight

SLvsFin_Data2013.csv (2021/02/15)
                       |-- date: The date of fich collection(YYYY/MM/DD)
                       |-- year: Year of fish collection
                       |-- month: Month of fish collection
                       |-- ordinal: Julian date of fish collection
                       |-- population: collected site name
                       |-- sex: "f" is female, and "m" ins male
                       |-- SL: Standard length (mm)
                       |-- BD: Body depth (mm)
                       |-- AFL: Anal fin length (mm)
                       |-- DFL: Dorsal fin length (mm)
                       
mateNumberAndfertilizationRate.csv (2020/08/14)
                       |-- collectDate: The date of fich collection(YYYYMMDD)
                       |-- fID: Female individual ID for mating experiment
                       |-- sizeF: Female standard length (mm)
                       |-- reproduct: "1" is spawning egg in the mating experiment, and "0" is  not spawing.
                       |-- Fegg: number of fertilization egg
                       |-- NonFegg: number of non-fertilization egg
                       |-- mID: Male individual ID for mating experiment
                       |-- SL: Male standard length (mm)
                       |-- TL: Male total length (mm)
                       |-- BD: Male body depth (mm)
                       |-- CFL: Male caudal fin length (mm)
                       |-- AFL: Male anal fin length (mm)
                       |-- DFL: Male dorsal fin length (mm)
                       |-- AFLratio: Male anal fin length per standard length
                       |-- DFLratio: Male dorsal fin length per standard length
