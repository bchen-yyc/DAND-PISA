# PISA 2012 Data Analysis
## by Liangbin Chen

## Project Information

This is the final project of Udacity Data Analyst Nanodegree.

## Dataset

Programme for International Student Assessment (PISA)is a survey of students' skills and knowledge as they approach the end of compulsory education. It is not a conventional school test. Rather than examining how well students have learned the school curriculum, it looks at how well prepared they are for life beyond school. 
Around 510,000 students in 65 economies took part in the PISA 2012 assessment of reading, mathematics and science representing about 28 million 15-year-olds globally. Of those economies, 44 took part in an assessment of creative problem solving and 18 in an assessment of financial literacy.

The raw data set is not uploaded to github due to its size, it can be downloaded 
from the link below and you should place it in the `raw-data` folder.
https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip

The purpose of this project is to find out the features that contribute most to the students' academic success.

## How to run

Libraries needed: numpy, pandas, seaborn, matplotlib  
Running environment: Jupyter Notebook  
Executable files: PISA2012.ipynb, slide_deck_PISA2012.ipynb. This first file documented the whole process while the second file was used to generate the slide deck.  
Slide format file: output_toggle.tpl
Convert ipynb file to slides: jupyter nbconvert slide_deck_PISA2012.ipynb --to slides --post serve --template output_toggle
Slide deck file: slide_deck_PISA2012.slides.html

## Summary of Findings

To avoid making this presentation too long, I only explorated the relationship between math score and other features. The approaches for english and science score are the same.
From my exploration I found it is obvious that students in OECD countries have higher math scores than those in non-OECD countries. Male students are better in math than female students worldwide. Math score is also positively related with grade of the students, education level of their parents and their family wealth.   
After further analysis I concluded that the OECD feature is not a independent feature. The fact that OECD students are better in math is highly related to their parents' education level and their family wealth. 
I also noticed that there was a weak positive relationship between math scores and math study minutes. There was no obvious relationship between math and after-school study hours.
Since gender is a indenpendent feature, I seperated the data set to male and female dataset and focused only on male students. The approach for female students are exactly the same. 
I also seperated the top ten countries with highest students math scores. After furthing digging into the data I found that math score has a strong positive relation with math study minutes for some of those asian countries including: Japan, Korea, China-Shanghai, Singapore, Chinese Taipei. I also found math score has a moderate positive relationship with after-school study hours. My guess is that in those countries the competitions are so fierce that every minutes they spend on the subject matters.

## Key Insights for Presentation

For this presentation I only explore the relationship between math score and other main features. To avoid those features from affecting each other during analysis, I isolated them from each other. I seperated the data set to male and female subsets. I explore the relationship between math score and other features for each grade and parents education level. At the end of the presentation, I dig into data from some asian countries and draw some slightly different conclusion from global data. 


