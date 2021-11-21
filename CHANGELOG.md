# Изменения в проекте
**История проекта ведется в соответствии со следующими принципами:**
+ Для каждой версии должен быть отдельный раздел.
+ Группировать изменения по категориям (Features, Bug fixes, Improvements и т.п).
+ Самые новые версии должны располагаться в начале документа.
+ Иметь возможность навигации по файлу.

## v0.0.1 (2021-09-27)
### Сделано
* Составление плана работы
* Составление концепции проекта
* Оформление репозитория

## v0.0.2 (2021-10-11)
### Сделано
* Встреча с заказчиком
* Согласование спринтов

## v0.0.3 (2021-10-25)
### Сделано
* Получение данных
* Предварительное знакомство с данными
* Изучение архитектуры нейросети UNet и ее особенностей применения в задачах медицины
* Построение сырой версии U-Net с использованием PyTorch по следующему туториалу на YouTube  
  [Implementing original U-Net from scratch using PyTorch](https://www.youtube.com/watch?v=u1loyDCoGbE&t=8s)

## v0.0.4 (2021-11-8)
### Сделано
* Обработаны данные и наложены маски на срезы сейсмических кубов напарником по проекту

  ![horizon mask](./images/Horizon_Mask.png?raw=true "horizon mask")
* Изучены статьи, посвященные работе с геологическими срезами:  
  1. [Seismic Horizon Detection with Neural Networks Part 1](https://medium.com/data-analysis-center/seismic-horizon-detection-with-neural-networks-part-1-5dec9ff7361a)
  2. [Seismic Horizon Detection with Neural Networks Part 2](https://medium.com/data-analysis-center/seismic-horizon-detection-with-neural-networks-part-2-2bd654d5aea7)
  3. [Making Seismic Interpretation Easy with SeismiQB](https://medium.com/data-analysis-center/making-seismic-interpretation-easy-with-seismiqb-ac62d01a477)
* Просмотрены 6 часов из 14 по курсу TensorFlow на YouTube  
  [Learn TensorFlow and Deep Learning fundamentals with Python (code-first introduction) Part 1/2](https://www.youtube.com/watch?v=tpCFfeUEGs8&t=22153s)

## v0.0.5 (2021-11-8)
### Сделано
* Разбиение исходных данных на квадраты с размерами 16, 64, 64 (y, x, z) и составление из них обучающей выборки
* Проведение экспериментов на архитектуре UNet3d и оценка метрики dice coefficient
* Реструктуризация модели под 2d архитектуру
* Эксперименты с новой архитектурой и получение первых практически применимых результатов
  
 ### Изменения
 * requirements.txt
