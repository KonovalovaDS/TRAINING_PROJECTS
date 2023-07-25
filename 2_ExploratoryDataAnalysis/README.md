# <center> Exploratory Data Analysis </center>

## <center> Analysis of open positions on website headhunter.ru </center>

<center> <img src = https://play-lh.googleusercontent.com/s6JiMSUktkTX0ejwpJ-DgqVb03dE00O975GGOoMmrlVL1aI8A1yOy7xh3dOSaxpuFWJH></center>

## Content

[1. Project description](README.md#project-description)

[2. Dataset](README.md#dataset)

[3. Technologies](README.md#technologies)

[4. Contacts & Credits](README.md#contacts--credits)


## Project description
There is dataset downloaded from the job search website named "hh.ru". Problem is that some candidates do not stating their desired amount of monthly salary. This is an obsticle for recommendation system of the website, which selects a list of the most suitable vacancies for applicants, and a list of the most suitable specialists for employers. Therefore the company wants to create a model that would automatcally determine the approximate level of wages suitable for the user, based on the information that the user indicated about himself. But before creating the model, it is necessary to transform, explore and refine dataset. This is actually is the aim and the subject of this project, which is consist of the following parts:

1. basic data structure analysis;

2. data transformation;

3. intelligence analysis;

4. data cleaning.

[To the top](README.md#content)

## Dataset

Dataset can be downloaded from google drive using the following link: https://drive.google.com/file/d/1hFj2Itss8Higs1nmkwUIKfLZApQSPiUt/view?usp=drive_link

To read file please use the following code:
```python
url = 'https://drive.google.com/file/d/1hFj2Itss8Higs1nmkwUIKfLZApQSPiUt/view?usp=drive_link'

path = 'https://drive.google.com/uc?export=download&id='+url.split('/')[-2]

df = pd.read_csv(path)
```
Inital dataset contains 44744 rows and 12 columns

[To the top](README.md#content)

## Technologies  

The following tools and liabraries have been used:
- Plotly liabrary for visualization;

- Z-score method for outliers. More codes for outliers are located: https://gist.github.com/KonovalovaDS/fff66a0cea914aa53d054fb9832792dd.js

[To the top](README.md#content)

## Contacts & Credits

Credits to SkillFactory team of mentors and coordinators. Special appreciation to Sergey Dobdin.

Email: natalia_konovalova@icloud.com

Kaggle: https://www.kaggle.com/nataliamantyk 

LinkedIn: https://www.linkedin.com/in/natalia-ds-198612241

[To the top](README.md#content)
