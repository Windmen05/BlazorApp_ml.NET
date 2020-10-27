# BlazorApp_ml.NET
------------------
## Модель
=========
Модель была обучена на [датасете](https://www.kaggle.com/windmen/age-predict) с размеченным возрастом, где название каждой папки указывает на возраст человека помещенного в эту папку
В связи с тем, что платформа, предоставляющая GPU имеет лимит по времени, модель была обучена на 1й эпохе, с использованием готовой модели [resnet-18](https://neurohive.io/ru/vidy-nejrosetej/resnet-34-50-101/),
resnet-18 самая легкая сеть из сетей архитектуры resnet
После [первичного обучения](https://github.com/Windmen05/BlazorApp_ml.NET/blob/main/First%20training.ipynb), найденные моделью веса в течении обучения на 1й эпохи были загружены и [модель с загруженными весами была обучена заного](https://github.com/Windmen05/BlazorApp_ml.NET/blob/main/recursive-training.ipynb),
процесс можно повторять до получения необходимой точности
