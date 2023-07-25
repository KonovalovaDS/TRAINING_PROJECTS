# <center> A / B Testing Results Analysis</center>
# <center> & </center>
# <center> Logging Experiment in Comet ML 

<center><img src = https://www.invespcro.com/blog/images/blog-images/ab-testing-1.jpg></center>

## Content

[1. Project description](README.md#project-description)

[2. Technologies](README.md#technologies)

[3. Contacts](README.md#contacts)

## Project description
### - Analysis of A / B testing Results 
A tourist company plans to launch a new prmotion to sell as many tours as possible. The team developed two versions of company's official website and conducted A/B testing. The task is to analyze the effectivness of both variants of website by two criteria: purchase conversion and average check, make the conclusion which of the website design is preferable. 
The company offers the tours to the following destinations with corresponding price tag:

- Thailand - 100.000 RUR
- Turkiye - 60.000 RUR
- Maldives - 200.000 RUR
- St.Petersburg - 10.000 RUR
- Kamchatka - 150.000 RUR

### - Logging Experiment
The target of the project is to learn how to run and logging the experiment & corresponding metrics via Comet ML web-service. It is necessary tool while developing ML-model using various parameters in order to keep track of updated and improved model metrics. 
To use dataset, please use the below code:
```python
url = 'https://drive.google.com/file/d/11sgquDFg1cSfm-j3i1XtyCl2eNO5dcYb/view?usp=sharing'

path = 'https://drive.google.com/uc?export=download&id='+url.split('/')[-2]

data = pd.read_csv(path, compression = 'zip')
```

[To the top](README.md#content)

## Technologies
1. Z-test
2. Conversions intervals and their difference
3. Shapiro Test
4. T-test

[To the top](README.md#content)

## Contacts

Email: natalia_konovalova@icloud.com

Kaggle: https://www.kaggle.com/nataliamantyk 

LinkedIn: https://www.linkedin.com/in/natalia-ds-198612241

[To the top](README.md#content)