# Diabetes prediction

## Описание

[Ссылка на презентацию](прогнозування_ризику_розвитку_діабету_у_людини.pdf)

Основная цель нашего проекта - определить наличие диабета с помощью восьми характеристик. Этот проект является анализом данных о диабете и причинах его возникновения и использует различные методы машинного обучения для прогноза вероятности развития диабета у человека. Наши модели натренированы на выборке из 100 000 человек, включающей медицинские и демографические данные пациентов, а также сведения о наличии или отсутствии диабета у них (положительный или отрицательный статус).

Мы использовали библиотеки Python, такие как Pandas, Scikit-learn, TensorFlow и Matplotlib для обработки данных, создания моделей и их оценки.
## Установка Библиотек

```
pip install -r requirements.txt
```

## Расположение

В файле [main_full.ipynb](main_full.ipynb) хранится реализация проекта и процессинг данных. В файле [main.ipynb](main.ipynb) хранится реализация модели которая включена в [main_full.ipynb](main_full.ipynb). Также 
хранится реализация основного пре процессинга данных.

## Работа Sequential-Нейросети 
Результаты предикта по внесенным от руки значениям.
```python
new_data = ["1", #Введите пол Female or Male \ 0 or 1
            "29", #Введите возраст 10.0
            "1", #'hypertension'0 or 1,
            "1", #'heart_disease'0 or 1,
            "1", #'smoking_history' 0 \ 0.1\ 0.5 \ 1 never, not current, current, ever
            "22.92", #'bmi'10.0,
            "6.5", #'HbA1c_level'10.0,
            "10.5" ] #'blood_glucose_level' mmol 6.2 or md\dl

1/1 [==============================] - 0s 54ms/step
Предсказанная вероятность: [[81.01]]
Человек вероятно заболеет диабетом, в течении года.
```

## Анализ данных
Приведенный в [main_full.ipynb](main_full.ipynb) и [main.ipynb](main.ipynb) анализ данных вполне хорош. Но дополнительно был 
проведен анализ с помощью tableau.  

[Ссылка на визуализацию данных по диабету](https://public.tableau.com/views/DiabetesSet/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)


## Авторы

- Павел Чистяков ИТШИ-21-4
- Ева Величко ИТШИ-21-4
- Егор Вилянский ИТШИ-21-5
- Отдельная благодарность Никите Хамбуру ПЗПИ-21 за предоставленные рекомендации в tableau.
