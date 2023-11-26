# Практическое задание №1

### Цель 
&nbsp Реализовать модель для классификации фрагментов полнокадровых гистологических изображений (патчей) на 9 классов: [ADI, BACK, DEB, LYM, MUC, MUS, NORM, STR, TUM]. Каждый патч представляет собой цветное (8-bit) изображение 224×224 px

### Мотивация
&nbsp В настоящее время методы глубокого обучения показывают высокие достижения в классификации, сегментации и анализе биомедицинских изображений, включая гистологические изображения.
&nbspВ данном исследовании основное внимание уделяется задаче классификации отдельных участков гистологических тканей.

### Обоснование выбора СNN.
&nbsp Когда речь идет о выборе между сверточными нейронными сетями (CNN) и классическими подходами машинного обучения для задач классификации участков гистологических тканей, существует несколько весомых причин в пользу CNN. Во-первых, CNN эффективно учитывают пространственную структуру данных, что особенно важно в случае обработки изображений. Этот аспект может быть недостаточно учтен классическими методами машинного обучения. Во-вторых, сверточные нейронные сети автоматически изучают иерархию признаков на разных уровнях, что обеспечивает извлечение сложных и абстрактных характеристик.
&nbsp Кроме того, использование предварительного обучения на больших наборах данных является еще одним преимуществом CNN. Это позволяет модели выучивать общие признаки изображений до начала обучения на конкретной задаче, снижая необходимость в больших объемах размеченных данных. Наконец, сверточные нейронные сети эффективны при обработке больших объемов данных, таких как изображения высокого разрешения, что может быть ключевым фактором в задачах классификации гистологических участков.
&nbsp В отношении ResNet, это тип глубоких нейронных сетей, который был предложен для преодоления проблемы затухающего градиента при обучении очень глубоких моделей. ResNet включает в себя блоки с "остаточными" соединениями, что упрощает передачу градиентов через сеть. В свою очередь, библиотека Keras обеспечивает удобные средства для реализации и обучения моделей, в том числе и ResNet.
