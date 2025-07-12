# A clear blue sky isn't always good news for drivers in São Paulo State, Brazil
[Visit the website](https://phillctw.github.io/sp-car-crashes/)
---

## Objective

The project aimed to understand patterns in accidents on São Paulo State roads, in Brazil.

---
## Findings

The project analyzes all car accidents documented on São Paulo State roads so far in 2025. 

I found that weather conditions are not a good predictor of accidents in São Paulo, as the majority of the incidents happen in good weather and clear visibility. The data also shows that human recklessness is the main cause of car accidents in the state. 

Finally, I found that car crashes are clearly concentrated on Fridays, with high fatality rates on Fridays and over the weekend.

---

## Data collection and analysis
I used data from DER/SP (São Paulo Roads Department), which can be accessed [here](https://www.der.sp.gov.br/WebSite/Servicos/ConjuntoDados.aspx?tema=Seguranca_Viaria&conjunto=Acidentes).

The video at the top of the article was downloaded from YouTube using `yt-dlp`. It is part of the opening of a Brazilian comedy show called 'Choque de Cultura' (roughly Culture Crash), in which truck drivers discuss cinema.

For the analysis, I used `Pandas` to investigate the dataset, trying to answer the following questions:
1. What drives accidents on São Paulo highways?
2. Where do accidents happen the most?
3. Is there a weather component in car crashes in São Paulo? (My theory, which proved to be wrong, was that bad weather would account for a significant share of accidents.)
4. How are accidents distributed over the week? (I suspected that Mondays and weekends would have the most cases.)
5. Is there an hourly pattern for the accidents?

---

## New skills and growth

It was my first time using `pandas` in the wild, meaning there was no way to be completely sure I was getting the right answers to my questions. That itself was a great way to grow and develop my skill set.

Exactly because of that, I became more confortable and acquainted with the workflow for data analysis, which was one of my goals for that first project.

I also had to use `pd.to_datetime`, something we hadn't learned and that can be tricky. But I was lucky that the date data points were already in a friendly format.

---

## Things I tried or wanted to do

I really wanted to map the exact place of each accident. The data to do so is in the dataset, but, when I tried to pass that info to Datawrapper, the result wasn't understandable at all. Maybe breaking the data into smaller pieces would be my strategy if I were to continue developing the project.

I also tried to find hourly patterns for accidents, but I suspected the data for this wasn't clean enough (I thought this because there was a huge concentration of accidents at midnight, but almost none in the surrounding minutes and hours). With more time, I could have contacted the dataset custodian to confirm whether the data was correct or not.

I would also like to expand the period analyzed. I could have included data for 2024 -and, unfortanetly, that would be it, as the available data only starts then (at least using DER/SP as s source).
