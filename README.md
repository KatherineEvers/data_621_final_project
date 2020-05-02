# data_621_final_project

Hi guys, I complied five sets of data from the cdc: https://wwwn.cdc.gov/Nchs/Nhanes/Search/DataPage.aspx?Component=Questionnaire&CycleBeginYear=2017

Below are the five sets of data, and you can look up the code book for each via the url

Mental Health - Depression Screener (DPQ_J)
<https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/DPQ_J.htm>

Occupation (OCQ_J)
<https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/OCQ_J.htm>

Sleep Disorders (SLQ_J)
<https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/SLQ_J.htm>

Current Health Status (HSQ_J)
<https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/HSQ_J.htm>

Smoking - Cigarette Use (SMQ_J)
<https://wwwn.cdc.gov/Nchs/Nhanes/2017-2018/SMQ_J.htm>

I combined them all (using the "get_data.R" script) into one data set (joining by common key and removing variables that have significant number of missing values). You can find it ("df.csv") in the data folder.

For the sake of simplicity of this final project, we can do 1) multiple linear regression on depression and 2) classification on current health status. For instance, we need to combine the scores (0, 1, 2 or 3) from "DPQ010" to "DPQ090" in this data set to get an overall depression score (range from 0 to 27) for each individual, i.e. 0 not depressed at all to 27 clinical depressed. We can fit a regression model to predict depression using data such as current health status, sleep hours, smoke habit, etc. In addition, we can build classification model to classify current health status "HSD010" (1 - Excellent, 2 - Very good, etc.). Finally, since we still have a lot of missing values in the data set, I can do 3) odds ratio to come up with features that significantly associates with current health status.

It should be fairly easy to look up on the literature and write about it. Let's cross the finish line together!

We can do literature reivews separately on health, psychology, sociology or so forth, and then combine our work together in one paper. 
