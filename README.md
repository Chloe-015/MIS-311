# MIS-311
MIS 311 coursework repository showcasing data analysis and portfolio work.

**Dataset**: Student Performance

**Student**: Thai Ngoc Mai Anh

**University**: Eastern International University

## 1. Data Overview
The Students Performance in Exams dataset contains academic performance records of students, focusing on achievement in mathematics, reading, and writing. Each record represents an individual student and includes demographic background information such as gender, race/ethnicity, and parental level of education, providing context for analysing differences in academic outcomes.

```
gender: Student gender
race_ethnicity (object): Student’s racial or ethnic group
parental_level_of_education (object): Educational background of the student’s family
math_score (int): Student performance in mathematics
reading_score (int): Student performance in reading
writing_score (int): Student performance in writing
total_score (int): Sum of math, reading, and writing scores
average_score (float): Average score across the three subjects
```

The dataset comprises 203 rows and 8 columns, containing both categorical variables (gender, race/ethnicity, parental level of education) and numerical variables (exam scores). This structure supports effective exploratory data analysis of student performance patterns.

<img width="789" height="144" alt="image" src="https://github.com/user-attachments/assets/482d080d-21f7-417a-a48c-24fd5766d87f" />
<img width="785" height="140" alt="image" src="https://github.com/user-attachments/assets/deb6cb02-1e7e-40ff-9c9a-8ea44cbff0fd" />

This dataset was chosen because it demonstrates how data analytics can be applied to understand academic performance trends and assess the influence of demographic factors on educational outcomes, supporting data-driven decision making in education and policy contexts.
## 2. Data Cleaning
- Mising value

I use Excel Power Query to indentify the missing value:

There are 2 null values of parental_level_of_education. As frequency analysis showed no single most frequent category, with _associate’s degree_ and _some college_ occurring with equal highest frequency, a unique mode could not be determined; therefore, the missing values were replaced with “Unknown” to ensure data completeness while maintaining data integrity.

<img width="269" height="85" alt="image" src="https://github.com/user-attachments/assets/4d7467b7-b5af-4289-a109-e72556e889a3" />

There are 4 null values of average_score. Missing values in the average_score variable were resolved using Excel Power Query by recalculating the column through a custom formula based on math, reading, and writing scores, with the results rounded to two decimal places to preserve numerical accuracy.

<img width="179" height="136" alt="image" src="https://github.com/user-attachments/assets/9faff2a9-c210-4544-8eab-4b45761b88c8" />

- Duplicate rows

The original dataset contained 3 duplicate rows, which were identified and removed using the Remove Duplicates function in Excel Power Query by applying it across all columns, ensuring that each remaining row represented a unique student record.

## 3. Descriptive Statistics 

<img width="511" height="244" alt="image" src="https://github.com/user-attachments/assets/705965f9-edc2-405c-b32c-4abfe8f32856" />

The descriptive statistics provide an overview of student performance in mathematics, reading, and writing. On average, students achieved the highest scores in reading (Mean = 67.63), followed by writing (Mean = 66.37) and mathematics (Mean = 64.22). The median scores are 65 for mathematics and 68 for both reading and writing, indicating that typical student performance is slightly higher in language-related subjects than in mathematics.

In terms of variability, writing scores show the greatest dispersion (Standard Deviation = 16.26), followed by mathematics (15.90) and reading (15.78), suggesting that student writing performance varies more widely than performance in the other subjects. All three subjects have wide score ranges, with minimum scores close to zero (Math = 0, Reading = 17, Writing = 10) and maximum scores reaching 100, highlighting substantial differences in individual achievement levels. Skewness values indicate slightly negative distributions across all subjects, suggesting a higher concentration of scores toward the upper end of the scale. Overall, these statistics reveal moderate average academic performance with noticeable variability, supporting further analysis of performance differences across student groups.

***Chart 1: Average Student Performance by Subject***

<img width="602" height="372" alt="image" src="https://github.com/user-attachments/assets/3b1f38bd-2b9c-40fd-9c35-72f96e5d7117" />

Students achieved the highest average score in reading (67.63), followed by writing (66.37) and mathematics (64.22). This indicates that students generally perform better in language-based subjects than in mathematics. The lower average in math suggests a potential need for additional academic support or targeted interventions to improve mathematical performance.

***Chart 2: Impact of Parental Education on Student Performance***

<img width="699" height="422" alt="image" src="https://github.com/user-attachments/assets/37e5c46d-2115-4ddc-9b91-ae3694bfe865" />


Students whose parents hold a bachelor’s degree (73.03) or master’s degree (72.27) achieve the highest average scores, while students from some high school and Unknown categories perform the lowest. This reveals a clear positive relationship between parental education level and student academic achievement. Higher parental education may provide stronger academic support and learning resources, contributing to improved student outcomes.
