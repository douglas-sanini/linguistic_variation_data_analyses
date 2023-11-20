# Linguistic Variation Data Analysis
> This repository contains all data engineering and analysis from a graduate research on social linguistic variations.

## ABOUT THE RESEARCH
"This research aims to analyze the linguistic and identity properties of undergraduate students at the State University of Londrina, employing the theoretical and methodological principles of Variationist Sociolinguistics. Additionally, it seeks to describe the linguistic variety of these students, considering phonetic and phonological aspects, as well as the implications of these phenomena in interaction within a geographically diverse environment where different linguistic variants are present. To achieve the proposed objectives, data were collected from students in their first and final years of undergraduate programs. These data were stratified to analyze the linguistic patterns of academic discourse. Understanding these patterns could offer insights into the social dynamics within academic communities, shedding light on how language functions as a tool for identity construction and social interaction." - Ana Paula Silva

## PHENOMENON

"The four most productive were selected for this analysis: palatalization of /t/ and /d/; rhotic variants; /s/ as a plural marker; and deletion of /d/ in the gerund.

For the palatalization of /t/ (tia ~ tʃia) and /d/ (dia ~ dʒia), the analysis focused on the context following alveolar stops, considering whether they were followed by /i/. It was hypothesized that when the speaker chooses to pronounce /i/, they would also use [dʒ], and with the vowel /e/, they would prefer [d]. Additionally, the position in the word—beginning, middle, or end—was also examined. 

Regarding the deletion of /d/ in the gerund (cantando ~ cantan∅o), the goal was to verify the consistent presence of this process in the academic discourse, analyzing it based on social variables.

To investigate /s/ as a plural marker (vamos ~ vamo∅), two linguistic analysis criteria were established. Following Scherre (1978; 1988), the elimination of plural markers generally occurs only in determiners or elements in the first position. Therefore, the position of the word in the phrase was chosen as the first criterion. For the second criterion, the following context was examined to test the hypothesis that /s/ initiating the next word would favor the presence of /s/ as a plural marker for the previous word (a[s] saias).

Rhotic variants, on the other hand, were required to be in the coda position (partir), medial, or final. It's important to note that final syllable coda contexts with resyllabification and the occurrence of the tap variant as a result of /r/ ceasing to be a coda and becoming an onset, as in "mar aberto," were excluded from the analysis. The occurrence of deletion (comer ~ come∅) was also examined to test the hypothesis of a gradation in rhotic deletion. The analysis categorized words based on their size and the position of /r/ in the word: beginning, middle, or end. Furthermore, words were divided into two categories: verb and noun." - Ana Paula Silva

## DATA ENGINEERING
Within the `data` folder can be found all the .docx files with the fonetic transcriptions of the interviews used for this research. Within the `data_structure` folder, each fonetic phenomenom data sets were organized and created in seperate jupyter files. What happens there is the extraction of the .docx files into text files where the re library, also known as the python's regular expressions library, comes in great use to create specific expressions that can identify words with each phenomenon. Combining this with pandas library it was possible to meticulously create organized dataframes that in the future comes handy for the data analysis. The end results for each phenomenon can be found below. One important note observe is that each word for each table shown below have data regarding the subject that was interviewed which are subject number, undergrad major, year of college (either first or last) and sex. 

### PALATALIZATION 

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/4d8e2dc2-2b9b-44ad-893a-0c285652291c)

###  DELETION OF /d/ IN GERUNDS

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/d1d3b4af-d66a-4452-89d5-688459f0d60e)

### /s/ AS A PLURAL MARKER

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/9dcc9afa-87cc-4cc4-90ed-ab1bb7eb13ff)

### RHOTICS VARIANTS

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/552857af-b70b-42c9-aecc-161973f17aec)

## DATA ANALYSIS

Within the same jupyter files the analysis of each of the data sets shown above was preformed. Here are the interesting results found for each phenomenom


### PALATALIZATION 

Below are the counts of the combination of each patalization and the acompanied target vowel with their percentages.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/cdef7e41-6c35-400a-b2e9-630d39a718fa)

Next up are the counts of the combination of patalizations with the acompanied target vowel and the positions (alone, beginning, middle or ending) where the patalization is found within the word. Included are also the percentages of these ocurrences.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/09ca7358-7819-4e9d-a69f-6c87206f2cd1)


###  DELETION OF /d/ IN GERUNDS

The below table shows the counts of words that did and didn't have the deletion of the /d/ in gerunds with their respective percentages.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/48123071-30ce-4d14-b811-ab8efb8bd1fd)

Next up is the same case but now it will be divided by undergrad major, year of college and sex. Each case of division will be in seperate tables.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/0298bf75-272e-440d-b804-6b3855b4a8cd)

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/5ec8c62e-1638-4bda-a45c-b80f8f998bb9)

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/12b3962a-e875-4adb-a7df-40646ac1262f)


### /s/ AS A PLURAL MARKER

The table belows shows the count of words where the /s/ in plural words were included or deleted and the percentages.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/78654d3e-98b0-444c-bef6-cbfa359f2b92)

Next up is the same but seperating by undergrad major, year of college and sex.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/4de078a6-8e99-496d-b71c-6bd10cc319c8)

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/27dd921c-1df7-4596-ad89-a9f966a85e19)

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/3467d26d-57cc-4c3e-b929-b6bfb1687241)


### RHOTIC VARIANTS

The table belows shows the count of words with rhotic variants and their percentages.

![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/64ad38c5-b096-4c4d-87a7-f5ddc5d519ce)

Next up are respectively the counts and percentage tables of the cases where the /r/ was deleted and if these cases were for nouns or verbs.
Count:
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/86c35e6d-6364-4c9c-b22a-2cccebbf6348)
Percentage:
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/1b744c7d-0c53-457e-b117-6180a0b5186f)


Next up are the counts and percentage tables of the cases where the /r/ was deleted and if these cases were big (more than 8 characters), medium (Between 5 and 7 characters) or small (less than 5 characters).
Count:
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/2dc676fa-69c8-49e8-b8cc-f9c0b2ea6f57)
Percentage:
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/ac318614-fcd0-4282-a8f9-30faf48610e0)


Finally below are tables are the cases where the /r/ is deleted but now divided by undergrad major, year of college, sex and also the postition in  were the deletion ocorres within the word in which it was found.
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/7bf23130-b226-44c7-a7d1-7f0021667fcb)
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/80f15408-c43c-433e-aee6-5e07cfe6666b)
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/1cc10a05-01d1-4e9d-a108-70c78ef7239e)
![image](https://github.com/douglas-sanini/linguistic_variation_data_analyses/assets/102381949/485a1e28-e8a4-4488-8a71-d30f0d11f6d0)


## CONTACT
> DATA ENGINEER AND ANALYSIS - [Douglas Sanini](https://www.linkedin.com/in/douglas-sanini/)

> RESEARCH, DATA COLLECTION, ANALYSIS - [Ana Paula Silva](https://www.linkedin.com/in/ana-paula-silva-2b5906182/)
