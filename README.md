# AutoGraph
Пэт-проект, библитоека заметок с автоматической иерархической сортировкой.
# План реализации
## Сбор датасета
Инструмент ориентирован на работу с заметками-инсайтами о математике и машинном обучении.
Для обучения моделей из пайплайна будут использованы научные тексты из этих тематик, обязательно хорошо размеченные тегами и/или главами, если речь о книгах.
## Текстовые эмбеддинги
Первым шагом будет получение эмбеддингов тренировочных текстов на основе модели-энкодера.
Также нужно настроить NRT инференс для текстов, которые будут приходить в инструмент.
## Создание якорей
На основе эмбеддингов будет обуена модель квантизатор, либо другоя технология, разбивающая представление на осмысленные токены/эмбеддинги.
Выделенные из обучающего датасета темы будут выступать в качестве узлов-якорей.
## Иерархическое Вложение
Для привязки новых заметок к узлам графа знаний будут применеы иерархические представления, полученные на основе текста новой заметки.
Далее через близость в соответсвии с уровнем гранулярности топика заметки будут привязываться к нодам из графа.
# Demo
Для записи новых заметок предполагается использовать телеграм бота; интерфейс отображения графа пока что не выбран.
