# Предмет, цель и задачи теории прогнозирования. Основные методы статистического прогнозирования.

**Основными статистическими методами исследования временных рядов являются:** 

- метод выделения тренда (временного сглаживания)
- регрессионный
- автокорреляционный
- адаптивный (скользящих средних)
- метод гармонического анализа
- сингулярного спектрального анализа
- бутстрепа (численного размножения выборок)
- нейросетевой









# Эконометрическая модель, основные этапы построения эконометрической модели. 

**Основные этапы построения эконометрической модели:**

1. **Постановочный** – определение целей моделирования, отбор факторов и показателей. 
2. **Априорный** – предмодельный анализ экономической сущности изучаемого объекта или явления, формирование и формализация априорной информации и исходных допущений. 
3. **Параметризация** – выбор общего вида модели, состава и форм, входящих в нее связей между переменными (выбор вида функции 𝑓(𝑋1,𝑋2, … , 𝑋𝑘)) 
4. **Информационный** – сбор статистической информации (регистрация значений, участвующих в модели факторов и переменных). 
5. **Идентификация модели** – статистический анализ модели (статистическое оценивание параметров модели). 
6. **Верификация модели** – сопоставление реальных и модельных данных, проверка адекватности модели, оценка точности модельных данных. 

Этапы 1-3 – спецификация модели.









# Классификация исходных данных и переменных в эконометрических моделях. 

В любой эконометрической модели в зависимости от конечных при­кладных целей ее использования все участвующие в ней **переменные подразделяются на:**

- **экзогенные**, т. е. задаваемые как бы «извне», автономно, в опреде­ленной степени управляемые (планируемые);
- **эндогенные**, т.е. такие переменные, значения которых формиру­ются в процессе и внутри функционирования анализируемой социально-экономической системы в существенной мере под воздействием экзогенных переменных и, конечно, во взаимодействии друг с другом; в эконометри­ческой модели они являются предметом объяснения;
- **предопределенные**, т. е. выступающие в системе в роли *факторов-аргументов,* или *объясняющих* переменных.









# Понятия спецификации и идентифицируемости модели.

**Идентификация** — это соответствия между приведенной и структурной формами модели. 

**Приведенная форма модели** — каждое уравнение представляет собой решение системы уравнений модели, заданной в структурной форме.

**Структурная форма модели** — модель записана в виде системы уравнений.

- **Модель идентифицируема** – если все ее структурные коэффициенты определяются однозначно, единственным образом по коэффициентам приведенной формы модели, то есть если число параметров структурной формы модели равно числу параметров приведенной формы модели.
- **Модель неидентифицируема** – если число структурных коэффициентов больше числа приведенных коэффициентов и следовательно, структурные коэффициенты не могут быть оценены через коэффициенты приведенной формы модели.
- **Модель сверхидентифицируема**, если число приведённых коэффициентов больше числа структурных коэффициентов. В этом случае на основе коэффициентов приведённой формы можно получить два или более значений одного структурного коэффициента. В этой модели число структурных коэффициентов меньше числа коэффициентов приведённой формы.









# Основные задачи регрессионного анализа. Модель парной линейной регрессии.

**Регрессионный анализ** используется для решения следующих типов проблем: 

- Выявить, какая независимая переменная связана с зависимой. 
- Понять отношения между зависимой и независимыми переменными. 
- Предсказать неизвестные значения зависимой переменной.



![](https://i.imgur.com/PIcJkkb.png)

В матстатистике обычно используется следующий алгоритм для нахождения уравнения регрессии.

1. **Выбор модели (уравнения).** Часто модель задана заранее (найти **линейную регрессию**) или для подбора используют графический метод: строят диаграмму рассеяния и анализируют ее форму.
2. **Вычисление коэффициентов (параметров) уравнения регрессии.** Часто для этого используют [метод наименьших квадратов](https://www.matburo.ru/ex_ms.php?p1=msmnk).
3. **Проверка значимости коэффициента корреляции и параметров модели** (также для них можно построить доверительные интервалы), **оценка качества модели** по критерию Фишера.
4. **Анализ остатков**, **вычисление стандартной ошибки** регрессии, **прогноз** по модели (опционально).







# Функция регрессии, линия регрессии. Поле корреляции. Выборочная функция регрессии, ее параметры. 











# Метод наименьших квадратов (МНК), его графическая интерпретация. 

**Метод наименьших квадратов** основан на минимизации суммы квадратов отклонений функций от исходных переменных.

![https://books.econ.msu.ru/Introduction-to-Econometrics/chap02/2.2/](https://i.imgur.com/qqOjo9B.png)

![https://books.econ.msu.ru/Introduction-to-Econometrics/chap02/2.2/](https://i.imgur.com/TP4LrDh.png)





[МНК, формулы и примеры](https://teachmen.csu.ru/methods/phys_prac9.html)

[Дружелюбная эконометрия от МГУ](https://books.econ.msu.ru/Introduction-to-Econometrics/chap02/2.2/)





# МНК-оценки параметров парной линейной регрессии, их свойства. Интерпретация коэффициентов регрессионной модели. 

В общем случае коэффициент регрессии k показывает, как в среднем изменится результативный признак (Y), если факторный признак (Х) увеличится на единицу. 









# Стандартизированное уравнение регрессии, МНК-оценки параметров. 









# Коэффициент корреляции, его свойства. 

Свойства коэффициента корреляции:

1. Абсолютная величина выборочного коэффициента корреляции не превосходит единицы.
2. Если выборочный коэффициент корреляции равен нулю и выборочные линии регрессии – прямые, то *X* и *Y* не связаны линейной корреляционной зависимостью.
3. Если абсолютная величина выборочного коэффициента корреляции равна единице, то наблюдаемые значения признака связаны линейной функциональной зависимостью.
4. Если переменные *X* и *Y* умножить на одно и то же число, то коэффициент корреляции не изменится.



[Свойства коэффициента корреляции](https://studfile.net/preview/6864107/page:32/)







# Предпосылки МНК. Теорема Гаусса-Маркова. 

Основные предпосылки МНК ассоциируются с теоремой Гаусса-Маркова и представляют собой перечень условий для случайных отклонений эконометрической модели, выполнение которых обеспечивает эффективную статистическую проверку значимости параметров регрессии.

1. **Математическое ожидание случайного отклонения равно нулю для всех наблюдений.** Другими словами, случайное отклонение в среднем не оказывает влияния на зависимую переменную. Если уравнение регрессии включает коэффициент свободного члена (постоянную), то обычно это условие выполняется априори
2. **Дисперсия случайных отклонений постоянна для любых наблюдений.** В случае выполнения предпосылки, т.е. постоянства дисперсии отклонений, говорят о **гомоскедастичности**, в противном случае, т.е. когда предпосылка не выполняется и дисперсия отклонения непостоянная – о **гетероскедастичности**. Другими словами, несмотря на то, что при каждом конкретном наблюдении случайное отклонение может быть либо большим, либо меньшим, не должно быть некой априорной причины, вызывающей большее или меньшее отклонение, т.е. нельзя проследить закономерность в величинах отклонений. **Гетероскедастичность** случайных отклонений приводит к неэффективности оценок, полученных с помощью МНК, а также к смещенной и несостоятельной оценке дисперсионно-ковариационной матрицы МНК. Гомоскедастичность и гетероскедастичность: ![https://www.bsu.by/upload/page/558843.pdf](https://i.imgur.com/FT04crz.png)
3. **Случайные отклонения являются независимыми друг от друга.** В случае невыполнения предпосылки, говорят об автокорреляции случайных отклонений. Автокорреляция – «корреляция внутри себя», корреляционная связь между значениями одного и того же случайного процесса x(t) в моменты времени t1 и t2. Отсутствие автокорреляции и автокорреляция: ![https://www.bsu.by/upload/page/558843.pdf](https://i.imgur.com/tKE0OJV.png)
4. **Случайное отклонение должно быть независимо от объясняющих переменных.** Другими словами, случайное отклонение (или зависимая переменная) есть величина случайная, а объясняющая переменная - величина неслучайная. Модель является линейной относительно параметров. 
5. **Случайное отклонение должно быть распределено согласно нормальному закону распределения.** Должна отсутствовать высокая взаимная коррелированность экзогенных переменных. В случае невыполнения предпосылки, говорят о мультиколлинеарности. 



**Теорема Гаусса-Маркова:** если предыдущие предпосылки выполнены, то оценки, полученные по МНК, обладают следующими свойствами:

1. **Оценки являются несмещенными**. Те отсутствует систематическая ошибка в определении положения линии регрессии. 
2. **Оценки состоятельны**, так как дисперсия оценок параметров при возрастании числа n наблюдений стремится к нулю. Другими словами, при увеличении объема выборки надежность оценок увеличивается.
3. **Оценки эффективны**, то есть они имеют наименьшую дисперсию по сравнению с любыми оценками данных параметров, линейными относительно величин $y_i$.







# Оценка качества уравнения регрессии. Коэффициент детерминации. 

# Суммы квадратов отклонений, связь между ними. Дисперсионный анализ. 

# Проверка значимости уравнения (критерий Фишера). 

Критерий Фишера (F) для регрессионной модели отражает, насколько хорошо эта модель объясняет общую дисперсию зависимой переменной: 

$$F = \dfrac{R^2}{1 - R^2} \cdot \dfrac{f_2}{f_1}$$

$R$ — коэффициент корреляции, $f_1$, $f_2$ — число степеней свободы

Первая дробь в уравнении равна отношению объясненной дисперсии к необъясненной. Каждая из этих дисперсий делится на свою степень свободы. 

Число степеней свободы **объясненной дисперсии** $f_1$ равно количеству объясняющих переменных (например, для линейной модели вида $Y= AX + B$ получаем $f_1 = 1$. 

Число степеней свободы **необъясненной дисперсии** $f_2 = N - k - 1$ где $N$ — количество экспериментальных точек, $k$ — количество объясняющих переменных ($k = 1$ для модели $Y = AX + B$)









# Прогнозирование по регрессионной модели. Доверительные интервалы для функции и параметров регрессии.









[Доверительные интервалы для коэффициентов регрессии](https://mcimeer.narod.ru/data/t5/t5_2.html)

[Пример нахождения доверительных интервалов коэффициентов регрессии](https://math.semestr.ru/corel/prim1.php)











# Модель множественной линейной регрессии. МНК-оценки параметров множественной регрессии. Матричная запись МНК-оценок.

# Оценка качества уравнения множественной линейной регрессии. Коэффициент детерминации. Суммы квадратов отклонений, связь между ними. Дисперсионный анализ. 

# Проверка значимости уравнения множественной линейной регрессии (критерий Фишера). 

# Прогнозирование по модели множественной линейной регрессии. 

# Доверительные интервалы для функции и параметров регрессии. 

# Проверка статистической значимости коэффициентов регрессии.





[Пример нахождения статистической значимости коэффициентов регрессии](https://math.semestr.ru/corel/prim3.php)





# Некоторые вопросы практического применения регрессионных моделей. Мультиколлинеарность. 













# Методы устранения (уменьшения) мультиколлинеарности.

При построении прогноза на основе модели регрессии с мультиколлинеарными факторами важно учитывать величину ошибки прогноза. Если её величина является удовлетворительной, то модель можно использовать, несмотря на мультиколлинеарность. Если же величина ошибки прогноза большая, то устранение мультиколлинеарных факторов из модели регрессии является одним из методов повышения точности прогноза.









# Пошаговые процедуры отбора наиболее информативных переменных. 

В основе пошаговой процедуры отбора переменных лежит предположение, что признаки могут быть коррелированными.  Это приводит к тому, что включение в модель новых переменных может вызывать снижение значимости ранее включенных переменных. И если это снижение значимости сильнее некоторого критического, то ранее включенные переменные следует удалить из модели.

Иными словами, при пошаговом отборе чередуются шаги добавления и удаления переменных до тех пор, пока не будет достигнут стабильный набор переменных.

![](https://i.imgur.com/1rSEJgw.png)

![](https://i.imgur.com/Jri6VYw.png)

![](https://i.imgur.com/5MtLEXh.png)











[Шаговая регрессия](http://www.machinelearning.ru/wiki/index.php?title=%D0%A8%D0%B0%D0%B3%D0%BE%D0%B2%D0%B0%D1%8F_%D1%80%D0%B5%D0%B3%D1%80%D0%B5%D1%81%D1%81%D0%B8%D1%8F_%28%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%29)













# Введение фиктивных переменных в линейную модель регрессии. 

Иногда в процессе эконометрического моделирования у исследователя возникает потребность учитывать в качестве объясняющих факторов не только **количественные**, но и **качественные** характеристики. *Например, на цену квартиры могут влиять не только её жилая площадь (количественные переменные), но и материал, из которого изготовлен дом, или наличие в этой квартире балкона (качественные переменные).* Во всех этих случаях удобно использовать так называемые фиктивные переменные.

Фиктивные переменные — это такие переменные, которые принимают одно из двух значений — 0 или 1. Их также называют бинарными или дамми-переменными.

![https://books.econ.msu.ru/Introduction-to-Econometrics/chap04/4.2/](https://i.imgur.com/qAr9YaG.png)

![](https://i.imgur.com/rqcTpXg.png)

Отсюда видно, что при прочих равных условиях (при равном стаже работы) женщины получают на 3,5 доллара меньше, чем мужчины.

![](https://i.imgur.com/XPcEnC8.png)

![](https://i.imgur.com/RTRZV75.png)

![](https://i.imgur.com/b6XzrnV.png)









[Фиктивные переменные](https://books.econ.msu.ru/Introduction-to-Econometrics/chap04/4.2/)









# Оценка качества уравнения регрессии. Коэффициент эластичности.

**Коэффициент эластичности** показывает, на сколько процентов изменится величина результативной переменной *у*, если величина факторной переменной изменится на 1%.

![](https://i.imgur.com/kpOZUDO.png)

Коэффициенты эластичности могут быть рассчитаны как **средние** и **точечные** коэффициенты. 



Общая формула для расчёта коэффициента эластичности для среднего значения *x* факторной переменной *х*:

![](https://i.imgur.com/yjEcUxa.png)

![](https://i.imgur.com/8bszDvz.png)

![](https://i.imgur.com/m9eQOnZ.png)



**Точечный коэффициент эластичности** характеризует, на сколько процентов изменится результативная переменная *у* относительно своего значения в точке х1, если факторная переменная изменится на 1% относительно заданного уровня х1.

![](https://i.imgur.com/klhEl3d.png)

![](https://i.imgur.com/uVs8Uuj.png)

![](https://i.imgur.com/hswVTdO.png)







[Коэффициенты эластичности](https://be5.biz/ekonomika/e008/48.html)







# Некоторые виды нелинейных зависимостей, поддающиеся непосредственной линеаризации.









# Подбор линеаризирующего преобразования. 

![](https://i.imgur.com/vphRQxq.png)

![](https://i.imgur.com/CXvImLD.png)











# Тесты на гетероскедастичность (ранговой корреляции Спирмена, Голдфелда-Квандта, Уайта, Глейзера). 

# Устранение гетероскедастичности. 

Существует два подхода к решению проблемы гетероскедастичности:

1. преобразование данных
2. применение взвешенного и обобщенного метода наименьших квадратов (ОМНК)



**Преобразование данных** предполагает такое преобразование, чтобы модель уже обладала свойством гомоскедастичности. Чаще всего используется: **логарифмирование** и **переход к безразмерным величинам** путем деления на некоторые известные величины той же размерности, что и исходные данные. Возможна также **стандартизация исходных данных**.





[Подходы к решению проблемы гетероскедастичности](https://intuit.ru/studies/professional_skill_improvements/20842/courses/787/lecture/30345?page=2)







# Авторегрессия первого порядка. Тест Дарбина-Уотсона. 

![https://ru.wikipedia.org/wiki/%D0%9A%D1%80%D0%B8%D1%82%D0%B5%D1%80%D0%B8%D0%B9_%D0%94%D0%B0%D1%80%D0%B1%D0%B8%D0%BD%D0%B0_%E2%80%94_%D0%A3%D0%BE%D1%82%D1%81%D0%BE%D0%BD%D0%B0](https://i.imgur.com/IMCFeIU.png)







# Тест серий (Бреуша-Годфри). 

**Тест Бройша-Годфри** — процедура проверки автокорреляции произвольного порядка в случайных ошибках регрессионных моделей. Тест является асимптотическим, то есть для достоверности выводов требуется большой объём выборки.

![https://ru.wikipedia.org/wiki/%D0%A2%D0%B5%D1%81%D1%82_%D0%91%D1%80%D0%BE%D0%B9%D1%88%D0%B0_%E2%80%94_%D0%93%D0%BE%D0%B4%D1%84%D1%80%D0%B8](https://i.imgur.com/uarrO5g.png)







# Понятие о временных рядах. Основные составляющие временного ряда. Мультипликативная и аддитивная модели временных рядов, их связь. 

**Временной ряд** - это набор данных, который представляет эволюцию явления во времени. 

Ну или: **временной ряд** — последовательность регистрируемого сигнала. Он характеризуется:

- **тренд** (тенденция): общая эволюция серии
- **сезонность**: изменение значений за определенный период времени (неделя / месяц / год).
- **шум** (или остаток): события, которые невозможно предсказать.



Существует два основных типа моделей:

- **Аддитивная модель**, в которой мы суммируем три компонента.
- **Мультипликативная модель**, в которой мы умножаем три компонента.

Аддитивная модель выбирается, если линии, соединяющие максимумы и минимумы графика временного ряда, параллельны. Иначе выбирается мультипликативная модель. 

![](https://i.imgur.com/hQazi98.png)











# Задачи анализа временных рядов. Графическое представление временного ряда. Предмодельный анализ временного ряда. 

В анализе временных рядов выделяются две основные задачи: 

- задача идентификации
- задача прогноза

**Задача идентификации** при анализе наблюдаемых предполагает ответ на вопрос, каковы параметры системы, породившей данный временной ряд — размерность вложения, корреляционная размерность, энтропия и др. Размерность вложения — это минимальное число динамических переменных, однозначно описывающих наблюдаемый процесс. Корреляционная размерность является оценкой фрактальной размерности аттрактора системы и частным случаем обобщенной вероятностной размерности. Понятие энтропии связано с предсказуемостью значений ряда и всей системы

**Задача прогноза** имеет целью по данным наблюдений предсказать будущие значения измеряемых характеристик изучаемого объекта, т.е. составить прогноз на некоторый отрезок времени вперед. Сейчас разработано и обосновано несколько различных методов прогноза. Однако все они подразделяются на на два основных класса: локальные и глобальные. Такое деление проводится по области определения параметров аппроксимирующей функции, рекуррентно устанавливающей следующее значение временного ряда по нескольким предыдущим.











# Этапы выделения компонент мультипликативной и аддитивной модели временных рядов. 

Существует два основных типа моделей:

- Аддитивная модель, в которой мы суммируем три компонента.
- Мультипликативная модель, в которой мы умножаем три компонента.





# Методы сглаживания временных рядов (скользящего среднего, экспоненциального сглаживания, последовательных разностей). Прогнозирование на основе моделей временных рядов. Точечный и интервальный прогноз.

При работе с рядами наличие шума часто затрудняет анализ структуры ряда. Чтобы исключить его влияние и лучше увидеть структуру ряда, можно использовать методы сглаживания рядов.

Самый простой метод сглаживания рядов – **скользящее среднее**. Идея заключается в том, что для любого нечётного количества точек последовательности ряда заменять центральную точку на среднее арифметическое остальных точек:

![](https://i.imgur.com/9o7NSy5.png)

![](https://i.imgur.com/cTblq2O.png)

Метод скользящего среднего имеет определённые недостатки:

- Скользящее среднее неэффективно в вычислении. Для каждой точки среднее необходимо перевычислять по новой. Мы не можем переиспользовать результат, вычисленный для предыдущей точки.
- Скользящее среднее нельзя продлить на первые и последние точки ряда. Это может вызвать проблему, если нас интересуют именно эти точки.
- Скользящее среднее не определено за пределами ряда, и как следствие, не может использоваться для прогнозирования.



**Экспоненциальное сглаживание** (метод Хольта-Уинтерса)

Существует насколько вариантов данного метода:

- одинарное сглаживание для рядов, у которых нет тренда и сезонности;
- двойное сглаживание для рядов, у которых есть тренд, но нет сезонности;
- тройное сглаживание для рядов, у которых есть и тренд, и сезонность.

Метод экспоненциального сглаживания вычисляет значения сглаженного ряда путём обновления значений, рассчитанных на предыдущем шаге, используя информацию с текущего шага. Информация с предыдущего и текущего шагов берётся с разными весами, которыми можно управлять.

![](https://i.imgur.com/w51VXiM.png)

Параметр α определяет соотношение между несглаженным значением на текущем шаге и сглаженным значением с предыдущего шага. При α=1 мы будем брать только точки исходного ряда, т.е. никакого сглаживания не будет. При α=0 ряд мы будем брать только сглаженные значения с предыдущих шагов, т.е. ряд превратится в константу.

Чтобы понять, почему сглаживание называется экспоненциальным, нам нужно раскрыть соотношение рекурсивно:

![](https://i.imgur.com/QXdwbqN.png)

Из соотношения видно, что все предыдущие значения ряда вносят вклад в текущее сглаженное значение, однако их вклад угасает экспоненциально за счёт роста степени параметра α.

Однако, если в данных есть тренд, простое сглаживание будет «отставать» от него (либо придётся брать значения **α** близкими к 1, но тогда сглаживание будет недостаточным). Нужно использовать **двойное экспоненциальное сглаживание.** 

**Двойное сглаживание** использует уже два уравнения – одно уравнение оценивает тренд как разницу между текущим и предыдущим сглаженным значениями, потом сглаживает тренд простым сглаживанием. Второе уравнение выполняет сглаживание как в случае простого варианта, но во втором слагаемом используется сумма предыдущего сглаженного значения и тренда.

**Тройное сглаживание** включает ещё один компонент – сезонность, и использует ещё одно уравнение. При этом различаются два варианта сезонного компонента – аддитивный и мультипликативный. В первом случае амплитуда сезонного компонента постоянна и со временем не зависит от базовой амплитуды ряда. Во втором случае амплитуда меняется вместе с изменением базовой амплитуды ряда. Это как раз наш случай, как видно из графика. С ростом ряда амплитуда сезонных колебаний увеличивается.









[Методы анализа временных рядов: сглаживание](https://www.fsight.ru/blog/metody-analiza-vremennyh-rjadov-sglazhivanie/)













# Структурная и приведенная формы модели систем одновременных уравнений. 

Система совместных, одновременных уравнений (или структурная форма модели) обычно содержит эндогенные и экзогенные переменные.

**Эндогенные переменные** обозначены в приведенной ранее системе как *y*. Это зависимые переменные, число которых равно числу уравнений в системе.

**Экзогенные переменные** обычно обозначаются как *х*. Это предопределенные переменные, влияющие на эндогенные переменные, но не зависящие от них.

![](https://i.imgur.com/IaZruwx.png)

Классификация переменных на эндогенные и экзогенные зависит от теоретической концепции принятой модели.



![](https://i.imgur.com/BCetLhe.png)

По своему виду приведенная форма модели ничем не отличается от системы независимых уравнений, параметры которой оцениваются традиционным МНК. Применяя МНК, можно оценить, а затем оценить значения эндогенных переменных через экзогенные.







[Структурная и приведенная формы модели](https://vuzlit.com/2113360/strukturnaya_privedennaya_formy_modeli)

[Структурная и приведённая формы](https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D0%BE%D0%B4%D0%BD%D0%BE%D0%B2%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D1%8B%D1%85_%D1%83%D1%80%D0%B0%D0%B2%D0%BD%D0%B5%D0%BD%D0%B8%D0%B9)



# Рекурсивные системы одновременных уравнений. 

В таких системах в одном из уравнений содержится единственная зависимая переменная , которая в следующем уравнении присутствует в качестве факторной переменной. В третье уравнение эти эндогенные переменные из предыдущих уравнений могут быть включены как факторные и т.д.

![](https://i.imgur.com/2R5I11a.png)

В данной системе каждое последующее уравнение наряду с факторными переменными включает в качестве факторов все зависимые переменные предшествующих уравнений. Каждое уравнение этой системы может рассматриваться самостоятельно, и его параметры определяются методом наименьших квадратов (МНК).





[Система рекурсивных уравнений - vuzlit](https://vuzlit.com/729966/sistema_rekursivnyh_uravneniy)

[Системы рекурсивных уравнений](https://studme.org/179674/matematika_himiya_fizik/sistemy_rekursivnyh_uravneniy)





# Модель спроса – предложения как пример системы одновременных уравнений. 

![https://www.rea.ru/ru/org/cathedries/mathmek/Documents/Study%20material/%D0%AD%D0%BA%D0%BE%D0%BD%D0%BE%D0%BC%D0%B5%D1%82%D1%80%D0%B8%D0%BA%D0%B0.pdf](https://i.imgur.com/lAUsvVY.png)









# Основные структурные характеристики моделей СОУ. 











# Условия идентифицируемости уравнений системы.

**Достаточное условие идентифицируемости структурного уравнения:** ранг матрицы, составленной из коэффициентов (в других уравнениях) при переменных, отсутствующих в данном уравнении, не меньше общего числа эндогенных переменных системы минус единица.
