# Практическое задание №1

### Цель 
Реализовать модель для классификации фрагментов полнокадровых гистологических изображений (патчей) на 9 классов: [ADI, BACK, DEB, LYM, MUC, MUS, NORM, STR, TUM].
___

### Мотивация
В настоящее время методы глубокого обучения показывают высокие достижения в классификации, сегментации и анализе биомедицинских изображений, включая гистологические изображения. В данном исследовании основное внимание уделяется задаче классификации отдельных участков гистологических тканей.
___

### Обоснование выбора СNN
Когда речь идет о выборе между сверточными нейронными сетями (CNN) и классическими подходами машинного обучения для задач классификации участков гистологических тканей, существует несколько весомых причин в пользу CNN. Во-первых, CNN эффективно учитывают пространственную структуру данных, что особенно важно в случае обработки изображений. Этот аспект может быть недостаточно учтен классическими методами машинного обучения. Во-вторых, сверточные нейронные сети автоматически изучают иерархию признаков на разных уровнях, что обеспечивает извлечение сложных и абстрактных характеристик.

Кроме того, использование предварительного обучения на больших наборах данных является еще одним преимуществом CNN. Это позволяет модели выучивать общие признаки изображений до начала обучения на конкретной задаче, снижая необходимость в больших объемах размеченных данных. Наконец, сверточные нейронные сети эффективны при обработке больших объемов данных, таких как изображения высокого разрешения, что может быть ключевым фактором в задачах классификации гистологических участков.

В отношении ResNet, это тип глубоких нейронных сетей, который был предложен для преодоления проблемы затухающего градиента при обучении очень глубоких моделей. ResNet включает в себя блоки с "остаточными" соединениями, что упрощает передачу градиентов через сеть. В свою очередь, библиотека Keras обеспечивает удобные средства для реализации и обучения моделей, в том числе и ResNet.

___

### Метки
* LBL3 Автоматическое сохранение модели при обучении
* LBL4 Загрузка модели с какой-то конкретной итерации обучения
* LBL5 Вывод показателей loss и accuracy в процессе обучения
* LBL13 Предобучение на imageNet
___

### Доступ к Google Collab

[Доступ к Google collab документу](https://drive.google.com/file/d/1yjCy3EAeLNOZuq1eRl-fsPIb9QB-h3IL/view?usp=sharing) название документа: _solutionofproblemstarter1_, далее выйдет подсказка "использовать google collab" - нажмите на нее. Ссылка на файл: <https://drive.google.com/file/d/1yjCy3EAeLNOZuq1eRl-fsPIb9QB-h3IL/view?usp=sharing>
___

### Результаты

|  test_tiny  |  test_small |     test    |
|-------------|-------------|-------------|
|    0.755    |    0.795    |    0.7876   |
___

Если возникли вопросы напишете в telegram: **@BSnewlife**
