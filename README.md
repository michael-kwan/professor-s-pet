# Professor's Pet: You *are* just a number
#### PYGHACK 2018

##### Introduction
Professor's Pet is a numerical model that will be able to rank classes within an academic department at UIUC, using [Prof. Fagen-Ulmschneider's dataset](https://github.com/wadefagen/datasets/tree/master/gpa) of grade point averages of offered classes.

Our algorithm is a adaption from the chess ELO rating, as we matched classes between each other as well as students against each other. We call our metric the competitiveness rating.

##### Our Algorithm

###### Input Data Models:

| class      | student    | studentclassentry |
|------------|------------|-------------------|
| `class_name` | `student_id` | `student_id`        |
| `elo`        | `elo`        | `class_name`        |
| `gpa`        |            | `gpa`               |

###### Purpose:
A general purpose algorithm that calculates the competitiveness index, a pseudo-elo based score that
objectively determines the difficulty of a class or professor or the ability of a student to perform in their respective major.

![yup](https://i.imgur.com/5eVFFHl.png)
![steps](https://i.imgur.com/gDF3w2f.png)


##### Results


Using the average GPA of 114 past and present ECE classes, we were able to come up with a competitiveness rating for each of them, and in the graph below show that there is a trend that classes with higher average GPAs tend to have higher ratings:

![](https://i.postimg.cc/jqhCSCqT/Competitiveness_Rating_vs_Average_GPA.png)

Among present classes, these are some of the hardest and easiest ECE classes, with higher ratings being easier, and lower ratings being harder. With a cursory glance, we can see that some notorious classes have a low rating due to low average GPA, and advanced graduate seminars are easier:

| Class Number and Name                            | Competitiveness Rating | Average GPA |
|--------------------------------------------------|--------------------|-------------|
| ECE 586: Game Theory                             | 1224.629613        | 3.738095238 |
| ECE 590: Grad Seminar in Special Topics          | 1213.443122        | 3.7111233   |
| ECE 544: Topics in Signal Processing             | 1201.389846        | 3.609375    |
| ...                                              |                    |             |
| ECE 391: Computer Systems Engineering            | 762.7012135        | 2.459546926 |
| ECE 313: Probability w/ Engineering Applications | 674.8997736        | 2.095202585 |
| ECE 210: Analog Signal Processing                | 652.7759941        | 2.088134569 |


We also took a look at the competitive rating by professor:
![](https://i.postimg.cc/KvbKFV61/Class_Competitiveness_Rating_by_Professor.png)
