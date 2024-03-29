## Используемые наборы данных
Для данной лабораторной работы я решил выбрать два табличных датасета на задачу бинарной классификации. Первый из них отражает отток клиентов, а другой -- задачу кредитного риска. Оба я нашел на Kaggle.
## Визуализация 
Для визуализации были использованы разные библиотеки: matplotlib, seaborn, plotly.\
Для датасета задачи кредитного риска были построены pairplot, так как в силу того что признаки анонимизированы, достаточно сложно понять их настоящую природу. Благодаря данной визуализации и экспертной оценки по распределениям признаков, может быть, станет возможным деанонимизировать некоторые из них. Самостоятельно, без наличия должного опыта, сделать это не представляется возможным.\
Со вторым датасетом ситуация обстоит куда лучше. Были построены графики, демонстрирующие распределения признаков относительно целевой переменной. Также мне было интересно посмотреть на распределения некоторых категориальных признаков.
##  Работа с данными
В ходе работы были разрешены проблемы пропуска в данных, проблема кодирования категориальных признаков, а также нормировка, необходимая для некоторых моделей, которые нам только предстоит применить.

В одном датасете пришлось разобраться с проблемой пропусков в данных. В каждой из задач релевантные категориальные признаки были преобразованы с помощью OneHotEncoding, а численные были нормализованы, так как это необходимая составляющая для линейной модели. От некоторых признаков, смысл которых не очень ясен, я решил и вовсе избавиться. Также были сгенирированы новые признаки для одной из задачи.