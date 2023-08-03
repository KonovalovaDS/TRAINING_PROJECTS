# <p align="center"> Feature Engineering </p>
<p align="center"><img src = https://ml40sfg0bc2m.i.optimole.com/w:362/h:203/q:mauto/dpr:2.6/f:avif/https://lostontheroute.com/wp-content/uploads/2023/02/consigli-utili-per-risparmiare-prenotando-su-booking-com.webp></p>

### <p align="center"> ML-model: RandomForestRegressor </p>

### Content
[1. Project description](README.md#project-description)

[2. Dataset](README.md#dataset)

[3. Technologies](README.md#technologies)

[4. Credits and Contacts](README.md#credits-and-contacts)


## <p align="center"> Project description </p>

The company "Booking.com" is facing the problem - dishonest hotels that wind up their rating. One way to discover such hotels is to create a ML-model that predicts the rating of the specific hotel. If the prediction of the model is very different from the actual result, then the hotel might behave dishnestly and is worth to be checked.

The main target of the project is to see that thorough data cleaning, feature engineering, and exploratory data analysis can increase the accuracy of the ML-model significantly. 

To assess the quality of the ML-model, MAPE (mean absolute percentage error) has been calculated. The resut is 12%. Calculations and metrics were logged with Comet ML.

[To the top](README.md#content)

## <p align="center"> Dataset </p>

Dataset discription can be reviewed on Kaggle: https://www.kaggle.com/competitions/sf-booking/data

Please use the below code to read dataset:
``` python
url = 'https://drive.google.com/file/d/15SLYv8P7TgWghS3-dAnGf8RJgbewmrM5/view?usp=drive_link'

path = 'https://drive.google.com/uc?export=download&id='+url.split('/')[-2]

hotels = pd.read_csv(path, compression = 'zip')
```

[To the top](README.md#content)

## <p align="center"> Technologies </p>

The following special libraries and tools have ben used:

- Pycountry Convert
- NLTK
- Regular Expressions
- Category Encoders
- Anova test for numerical features

[To the top](README.md#content)

## <p align="center"> Credits and Contacts </p>

Credits to SkillFactory team of mentors and coordinators. Special appreciation to Sergey Dobdin.

Email: natalia_konovalova@icloud.com

Kaggle: https://www.kaggle.com/nataliamantyk 

LinkedIn: https://www.linkedin.com/in/natalia-ds-198612241

[To the top](README.md#content)



