# Data_Wrangling_DA-ND

Countries compete for Olympic medals differently - some send many athletes, while others focus on specific sports they're good at. When we look at how many medals each country wins compared to their number of athletes, we see that smaller nations like Jamaica and Hungary can be surprisingly successful by concentrating on their strengths rather than competing in everything.

In this Udacity Data Analyst Nanodegree project, I performed data wrangling using Python’s libraries on a Jupyter notebook to clean, transform, and analyze Olympic data from the 2024 Paris Games. The goal was to determine which countries performed best in specific sports and whether their strengths in those sports influenced the distribution of gold, silver, and bronze medals they won. By merging datasets, handling missing values, and applying statistical methods, I identified patterns—such as whether top-performing nations in a sport tended to win more gold medals compared to others. The findings provided insights into how sporting excellence translates to medal outcomes, helping to predict future trends in international competitions.

## Dataset 1
Type: CSV File, called athletes.csv.

Method: This file is downloaded programatically using get function in the requests module from the Paris 2024 Olympic Summer Games by PETRO user in Kaggle, using the following url: "https://www.kaggle.com/api/v1/datasets/download/piterfm/paris-2024-olympic-summer-games/athletes.csv".

This file includes personal information about all athletes. In this project, not all variables will be used to answer the research question defined in the problem statement.

Dataset variables:

code: Athlete's code for the participation in olympics 2024.
name: Athlete's full name, capitalized surname + first name.
name_short: Athlete's short name, capitalized surname + first letter of the first name.
name_tv: Athlete's full name as shown on the tv, first name + capitalized surname.
gender: Athlete's gender, male or female.
country_code: Athlete's country abbreviation.
country: Country name that the athlete represents.
height: Athlete's height.
weight: Athlete's weight.
disciplines: A specific category within a group of sports.
events: A specific competition where athletes compete for medals. Each discipline can contain multiple events.
birth_date: Athlete's birth date.
This dataset includes more variables (such as function, birth_place, family, etc.), which will be dropped where they have no effect on this research.

## Dataset 2
Type: CSV File, called medallists.csv.

Method: This file is downloaded manually from the same source, which is Paris 2024 Olympic Summer Games by PETRO user in Kaggle, I used this data gathering method in order to meet the project's requirements in using two different data gathering methods. The file is downloaded from kaggle and then uploaded into the same folder "datasets" manually.

This file includes a brief information about all medalists. All athletes in the medalists dataset supposed to exist in the athletes dataset but not vice versa. In this project, not all variables will be used to answer the research question defined in the problem statement.

Dataset variables:

medal_type: The awarded medal type (Gold, Silver, Bronze).
medal_code: The code of the medal type (Gold: 1, Silver: 2, Bronze: 3).
name: The medalist name, and it's format is same as the name in athletes dataset.
gender: Medalist's gender, male or female.
country_code: Medalist's country abbreviation.
country: Country name which the athlete represents.
team: Name of the medallist's team if exist.
discipline: A specific category within a group of sports.
events: A specific competition where athletes compete for medals. Each discipline can contain multiple events.
code_athlete: Athlete's code for the participation in olympics 2024.
code_team: Code of the medallist's team if exist.
This dataset includes more variables, will be dropped where no effect for them on this research.
