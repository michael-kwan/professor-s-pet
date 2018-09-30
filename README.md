# Professor's Pet
#### PYGHACK 2018

##### Introduction
Professor's Pet is a numerical model that will be able to rank classes within an academic department at UIUC, using [Prof. Fagen-Ulmschneider's dataset](https://github.com/wadefagen/datasets/tree/master/gpa) of grade point averages of offered classes.

Our algorithm is a adaption from the chess ELO rating, as we matched classes between each other as well as students against each other. We call our metric the competitiveness rating.

##### Our Algorithm


##### Results


Using the average GPA of 114 past and present ECE classes, we were able to come up with a competitiveness rating for each of them, and in the graph below show that there is a trend that classes with higher average GPAs tend to have higher ratings:

![](https://i.postimg.cc/tTbLMqxR/Class_Competitiveness_vs_Average_GPA-1.png)

Among present classes, these are some of the hardest and easiest ECE classes, with higher ratings being easier, and lower ratings being :

| Class Number and Name                        | Competitiveness Rating |
|----------------------------------------------|--------------------|
| ECE 343: Electronic Circuits Laboratory      | 2067.996954        |
| ECE 199: Undergraduate Open Seminar          | 1993.911498        |
| ECE 486: Control Systems                     | 1522.132066        |
| ...                                          |                    |
| ECE 330: Power Circuits and Electromechanics | 337.4888692        |
| ECE 459: Communications                      | 283.2651991        |
| ECE 380: Biomedical Imaging                  | 273.143938         |



![](https://i.postimg.cc/52qGFcrZ/Student_Competitiveness-1.png)
