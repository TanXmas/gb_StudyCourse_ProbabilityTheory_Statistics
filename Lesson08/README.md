***
# Урок 8. Корреляционный анализ

## Лекция

### Ковариация

### Коэффициент корреляции
#### – Коэффициент корреляции Пирсона
#### – Коэффициент корреляции Спирмена
#### – Условия применимости коэффициентов корреляции
#### – Интерпретация коэффициента корреляции

### Слабые стороны корреляционного анализа

***
## Семинар

## Задание 1.
Проведено 5 экспериментов. Для каждого построить график и посчитать коэффициенты корреляции Пирсона.

X = np.array([10, 8, 13, 9, 11, 14, 6, 4, 12, 7, 5]) \
Y = np.array([8.04, 6.95, 7.58, 8.81, 8.33, 9.96, 7.24, 4.26, 10.84, 4.82, 5.68])

X = np.array([10, 8, 13, 9, 11, 14, 6, 4, 12, 7, 5]) \
Y = np.array([9.14, 8.14, 8.74, 8.77, 9.26, 8.10, 6.13, 3.10, 9.13, 7.26, 4.74])

X = np.array([10, 8, 13, 9, 11, 14, 6, 4, 12, 7, 5]) \
Y = np.array([7.46, 6.77, 12.74, 7.11, 7.81, 8.84, 6.08, 5.39, 8.15, 6.42, 5.73])

X = np.array([8, 8, 8, 8, 8, 8, 8, 19, 8, 8, 8]) \
Y = np.array([6.58, 5.76, 7.71, 8.84, 8.47, 7.04, 5.25, 12.5, 5.56, 7.91, 6.89])

X = np.array([10, 8, 13, 9, 11, 14, 6, 4, 12, 7,5, 15, 16, 18 ])
Y = np.array([9.14, 8.14, 8.74,8.77, 9.26, 8.10, 6.13, 3.10, 9.13, 7.26, 4.74, 6.5, 5, 2.9])

### Задание 2.
2.1 Провести двусторонний тест и ответить на вопрос, есть ли статистически значимые различия между средними 2х нормально распределенных генеральных совокупностей,представленных следующими независимыми выборками. Уровень статистической значимости принять за 5%. \
1. Используйте функцию в Python.
2. Имея p-value из функции рассчитать наблюдаемое значение критерия

2.2 Используя функцию stats.ttest_ind, проведите односторонний тест. Проверить ,что $M(X) > M(Y)$.

2.3 Используя функцию stats.ttest_ind, проведите односторонний тест. Проверить ,что $M(X) < M(Y)$.

X = np.array([12, 10, 11, 19, 13, 11, 17, 15, 19, 14, 21, 18, 21, 11, 17, 14, 15, 17, 20, 19]) \
Y = np.array([11, 13, 18, 15, 17, 18, 10, 21, 26, 15, 11, 12, 15, 17, 10, 18, 18, 12, 21, 20])

***
## Практическое задание

### Задание 1.
Даны значения величины заработной платы заемщиков банка (zp) и значения их поведенческого кредитного скоринга (ks).

X = np.array([35, 45, 190, 200, 40, 70, 54, 150, 120, 110]) \
Y = np.array([401, 574, 874, 919, 459, 739, 653, 902, 746, 832])

1. Найдите ковариацию этих двух величин с помощью элементарных действий.
2. Найдите ковариацию этих двух величин с помощью функции cov из numpy.
3. Найдите коэффициент корреляции Пирсона с помощью ковариации и среднеквадратичных отклонений двух признаков.
4. Найдите коэффициент корреляции Пирсона с использованием функций из библиотек numpy и pandas.

### Задание 2.
Измерены значения IQ выборки студентов, обучающихся в местных технических вузах: 131, 125, 115, 122, 131, 115, 107, 99, 125, 111. Известно, что в генеральной совокупности IQ распределен нормально. Найдите доверительный интервал для математического ожидания с надежностью 0.95.

### Задание 3.
Известно, что рост футболистов в сборной распределен нормально с дисперсией генеральной совокупности, равной 25 кв.см. Объем выборки равен 27, среднее выборочное составляет 174.2. Найдите доверительный интервал для математического ожидания с надежностью 0.95.