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
## 2. Data Overview
- Mising value

I use Excel Power Query to indentify the missing value:

There are 2 null values of parental_level_of_education. As frequency analysis showed no single most frequent category, with _associate’s degree_ and _some college_ occurring with equal highest frequency, a unique mode could not be determined; therefore, the missing values were replaced with “Unknown” to ensure data completeness while maintaining data integrity.

<img width="269" height="85" alt="image" src="https://github.com/user-attachments/assets/4d7467b7-b5af-4289-a109-e72556e889a3" />

There are 4 null values of average_score. Missing values in the average_score variable were resolved using Excel Power Query by recalculating the column through a custom formula based on math, reading, and writing scores, with the results rounded to two decimal places to preserve numerical accuracy.

<img width="179" height="136" alt="image" src="https://github.com/user-attachments/assets/9faff2a9-c210-4544-8eab-4b45761b88c8" />

- Duplicate rows
## 3. Descriptive Statistics 
