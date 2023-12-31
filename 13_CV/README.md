## Определение возраста покупателей
---

### Цель
Построить модель, которая по фотографии определит приблизительный возраст человека. 

### Описание
Имеется датасет с фотографиями людей [ChaLearn Looking at People](http://chalearnlap.cvc.uab.es/dataset/26/description/), содержащий 7591 фотографию. В нашем распоряжении уже предобработанные фотографии лиц - задачу детекции выполнять не нужно.
, содержащий 7591 фотографию. В нашем распоряжении уже предобработанные фотографии лиц - задачу детекции выполнять не нужно.

Код обучения выполнялся на GPU на отдельном сервере. Прямого доступа к ядру сервера нет - он импортирует и выполняет функции в заданном формате:

- `load_train(path)` - загрузка тренировочного датасета,
- `load_test(path)` - загрузка тестового датасета,
- `create_model(input_shape)` - создание архитектуры сети, компиляция модели,
- `train_model(model, train_data, test_data, batch_size, epochs, steps_per_epoch, validation_steps)` - обучение модели

Значения **`MAE`** на тестовой выборке должно быть **не больше 8**.

### Используемые библиотеки
- **`Keras`**

- **`NumPy`**

- **`PIL`**

- **`Matplotlib`**

## Результаты
- За основу модели была взята архитектура **ResNet50**.\
Использовалась предобученная модель.
- За 10 эпох обучения сети удалось достичь значения **`MAE = 5.9063`**.

