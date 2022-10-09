Решение основано на использовании модели из семейства RNN:

- **RuMedDaNet** / **RuMedNLI** - используем двухслойную модель BiLSTM модель с 300-мерными вложениями слов;

- **RuMedTest** - Используем обученную модель из задачи RuMedNLI чтобы получить матрицу эмбеддингов вопросов и 4 матрицы для каждого из вариантов ответов. Ответ выбираем по максимальному значению косинусной близости между векторами вопроса и ответа.

### How to run

`./run.sh`