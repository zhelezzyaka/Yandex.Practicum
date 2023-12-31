﻿## Шифрование персональных данных клиентов

---

### Цель

Закодировать данные для защиты персональной информации с сохранением качества моделей машинного обучения.

### Описание

- Необходимо разработать метод преобразования данных, чтобы по ним было сложно восстановить персональную информацию.
- Нужно защитить данные, чтобы при преобразовании качество моделей машинного обучения не ухудшилось.

### Используемые библиотеки
- **`Scikit-learn`**
- **`Pandas`**
- **`NumPy`**

### Результаты
Был разработан алгоритм шифрования данных. При проверке работы модели регресси на данных до и после шифрования различий в метрике R2 не оказалось, т.е. шифровка данных не повлияла на работы модели.
