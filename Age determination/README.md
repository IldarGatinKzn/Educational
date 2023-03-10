# Определение возраста покупателей
[pdf](https://cloud.mail.ru/public/mc22/TysGnLASo) [Jupyter](https://github.com/IldarGatinKzn/Educational/blob/main/Age%20determination/age_determination.ipynb)

## Описание проекта

Целью работы является построение модели нейронной сети, которая по фотографии определит приблизительный возраст человека.

## Стек
* **python**,
* **pandas**,
* **numpy**,
* **PIL**,
* **tensorflow.keras**.

## Вывод

В результате данной работы построена модель свёрточной нейронной сети семейства ResNet50 библиотеки Keras, предобученная на датасете ImageNet. Модель решает задачу регрессии: по фотографии предсказывает возраст человека.
<br>Для увеличения количества входных данных применена аугментация.
<br>Для адаптации ResNet50 к решаемой задаче, последние 2 слоя исключены и сконструированы заново. В последнем полносвязном слое используется один нейрон с функцией активации ReLU.
<br>Обучалась модель с помощью алгоритма Adam c параметром "скорость обучения" равным 0.0001.
