### 1. Классификация видов моделирования: аналитическое, имитационное, комбинированное. Типовые математические схемы (D,F,P,Q,A).
<b>Аналитическое моделирование</b> – математическая формализация, изменение свойств объекта во времени.

Для аналитического моделирования характерно то, что процессы функционирования элементов системы записываются в виде некоторых функциональных соотношений (алгебраические, интегро-дифференцированные, конечно разностные) и логических условий.

Аналитическая модель может быть исследована 3-мя способами:

 - аналитическим способом – стремятся получить в общем виде зависимость от исходных характеристик;

 - численным способом – когда нельзя решить в общем виде, то получаем результаты для конкретных начальных данных;

 - качественный способ – не имея решения управления в общем виде, мы можем найти некоторые свойства решения;

Имитационное моделирование хуже аналитического. Комбинированное – самое лучшее.

При <b>имитационном моделировании</b> реализующий модель алгоритм воспроизводит процесс функционирования системы во времени, причем имитируются элементарные явления, составляющие процесс с сохранением их логической структуры и последовательности протекании во времени, что позволяет по исходным данным получить сведения о состоянии процесса в определенные моменты времени, дающие возможность оценить характеристики системы.

Основным преимуществом имитационного моделирования по сравнению с аналитическим, является возможность решения более сложных задач. Имитационные модели позволяют достаточно просто учитывать такие факторы, как наличие дискретных и непрерывных элементов, нелинейные характеристики системы и её элементов, многочисленные случайные воздействия.

Когда результаты, получаются при воспроизведении на имитационной модели процесса функционирования системы, являются реализациями случайных величин и функций, тогда для нахождения характеристик процесса, требуется его многократное воспроизведение с последующей статической обработкой.

<b>Комбинированное моделирование</b> при анализе системы позволяет определить достоинства его компонентов. Обычно проводят декомпозицию процесса функционирования объекта на составляющие подпроцессы.

#### Типовые математические схемы (D,F,P,Q,A) + N

<b>D-схемы (Непрерывно-детерминированные модели)</b>

D-схемы (англ. dynamic) – отражают динамику изучаемой системы, и в качестве независимой переменной, от которой зависят неизвестные искомые функции, обычно служит время t.

Частным случаем динамических систем, описываемых D-схемами, являются системы автоматического управления. Использование D-схем позволяет формализовать процесс функционирования непрерывно детерминированных систем S и оценить их основные характеристики, применяя аналитический или имитационный подход, реализованный в виде соответствующего языка для моделирования непрерывных систем или использующий аналоговые и гибридные средства вычислительной техники.

<b>F-схемы (Дискретно-детерминированные модели)</b>

F-схема (англ. finite automata) – это абстрактно-конечный автомат, характеризующейся шестью элементами.

Конечным автоматом называется автомат, у которого множества внутренних состояний, входных и выходных сигналов являются конечными множествами. Существуют несколько способов задания работы F-автоматов, но наиболее часто используются табличный, графический и матричный.

<b>Р-схемы (Дискретно-стохастические модели)</b>
<i>По идее, они же - Марковские цепи.</i>

Р-схема (англ. probabilistic automata) – это вероятностный автомат схем при дискретно-стохастическом подходе на вероятностных (стохастических) автоматах. В общем, виде Р-схемы можно определить как дискретный потактный преобразователь информации с памятью, функционирование которого в каждом такте зависит только от состояния памяти в нем, и может быть описано статистически.

<b>Q-схемы (Непрерывно-стохастические модели)</b>

Q-схема (англ. queueing system) – система массового обслуживания.

В качестве процесса обслуживания могут быть представлены различные по своей физической природе процессы функционирования экономических, производственных, технических и других систем, например: потоки поставок продукции некоторому предприятию, потоки деталей и комплектующих изделий на сборочном конвейере цеха, заявки на обработку информации ЭВМ от удаленных терминалов и т.д. При этом характерным для работы таких объектов является случайное появление заявок (требований) на обслуживание и завершение обслуживания в случайные моменты времени, т.е. стохастический характер процесса их функционирования.

На работу с Q-схемами при машинной реализации моделей ориентированы многие языки имитационного моделирования, например SIMULA, SIMSCRIPT, GPSS и др.

<b>N-схемы (Сетевые модели)</b>

N-схема – сети Петри (англ. Petri Nets), используемые для формального описания структуры и взаимодействия параллельных систем и процессов, а также анализа причинно-следственных связей в сложных системах.

<b>А-схемы (Комбинированные модели)</b>

А-схема – агрегативная система (англ. aggregate system), используемая для описания поведения непрерывных и дискретных, детерминированных и стохастических систем.

При агрегативном описании сложный объект (система) расчленяется на конечное число частей (подсистем), сохраняя при этом связи, обеспечивающие взаимодействие частей. Если некоторые из полученных подсистем оказываются в свою очередь еще достаточно сложными, то процесс их разбиения продолжается до тех пор, пока не образуются подсистемы, которые в условиях рассматриваемой задачи моделирования могут считаться удобными для математического описания. В результате такой декомпозиции сложная система представляется в виде многоуровневой конструкции из взаимосвязанных элементов, объединенных в подсистемы различных уровней.

### 2. Формализация и алгоритмизация процесса функционирования сложных систем.

Сущность компьютерного моделирования сложной системы состоит в проведении на компьютере эксперимента с моделью, которая в нашем случае представляет собой некоторый программный комплекс, описывающий формально или алгоритмически поведения элементов системы в процессе её функционирования, т.е. в их взаимодействии друг с другом и внешней средой.

Основные требования, предъявляемые к модели:

- Полнота модели – должна предоставлять пользователю возможность получения необходимого набора характеристик, оценок системы, с требуемой точностью и достоверностью.
- Гибкость модели – должна давать возможность воспроизведения различных ситуаций при варьировании структуры, алгоритмов и параметров системы. Причем структура должна быть блочной, т.е. допускать возможность замены, добавления, исключение некоторой части без переделки всей модели.
- Компьютерная реализация моделидолжна соответствовать имеющимся техническим ресурсам.

Основные этапы моделирования больших систем:
- Построение концептуальной (описательной) модели системы и её формализация;
- Алгоритмизация модели и её машинная реализация;
- Получение и интерпретация результатов моделирования;

На <b>этапе формализации</b> формулируется модель и строится её формальная схема, т.е. основным назначением данного этапа является переход от содержательного описания объекта к его математической модели.

Последовательность действий:

- Проведение границы между системой и внешней средой.
- Исследование моделируемого объекта с точки зрения выделения основных составляющих функционирования системы (по отношению к поставленной цели)
- Переход от содержательного описания модели к формализованному описанию свойств функционирования модели, т.е. к её концептуальной модели. Это сводится к исключению из рассмотрения некоторых второстепенных элементов. Полагают, что они не указывают существенного явления на ход процесса исследуемой модели.

Оставшиеся элементы модели группируются в блоки:

- Блоки I-ой группы представляют собой имитатор событий внешних воздействий.

- Блоки II-ой группы являются собственно моделью процесса функционирования.

- Блоки III-ой группы являются вспомогательными и служат для реализации блоков I и II группы. Так же эти блоки обеспечивают корректность ввода данных, приемлимость результатов и т.д.

Процесс функционирования системы, так разбивается на подпроцессы, чтобы построение модели подпроцесса было элементарно и не вызывало особых трудностей

На <b>этапе алгоритимизации</b> и компьютерной реализации математическая модель, сформированная на первом этапе, воплощается в конекретную программную модель.

Исходный материал – блочная логическая схема.

Последовательность действий:
- Разработка схемы моделирующего алгоритма.
- Разработка схемы программы.
- Выбор технических средств для реализации программной модели.
- Процесс программирования и отладки.
- Проверка достоверности программы на тестовых примерах.
- Составление технической документации.

На этапе получения и интерпретации результатов компьютер изспользуются для проведения рабочих расчетов по готовой программе. Результаты этих расчетов позволяют проанализировать и сделать выводы о характеристиках процессов функционрирования исследуемой схемы.

### 3. Моделирование на системном уровне.

<i>(Т.е. моделирование вычислительных систем - судя по лекциям из бауманки)</i>

При моделировании новых и модернизации существующих вычислительных систем и сетей необходимо предварительно оценивать эффективность их функционирования с учетом различных вариантов структурной организации. Эти варианты могут отличаться составом и характеристиками устройств. Структурой межмодульных связей, режимами работы и алгоритмами управления. Для оценок таких структур используют модели вычислительных систем. Под вычислительной системой будем понимать комплект аппаратных (процессор, память, ву) и программных средств ( ОС ), которые в совокупности выполняют определенные рабочие функции.

Коллектив пользователей – это сообщество таких людей, которые используют вычислительную систему для удовлетворения своих нужд по обработке информации.

Входные сигналы (программы, команды, данные), которые создаются коллективом пользователей, называются рабочей нагрузкой.

Схема вычислительной установки:

![схема](https://www.dropbox.com/s/k68jxx6ku67m1d1/Screenshot%202022-06-28%20140244.jpg)

<b>Концептуальная модель</b> включает в себя сведения о выходных и конструктивных параметрах системы, её структуре, особенности работы каждого ресурса (элемента системы), характере взаимодействия между ресурсами. Как правило, включается постановка прикладной задачи, определяющей цели моделирования исходной системы, а так же исходные данные для исследования системы.

<b>Формализованная схема</b> представляет собой, как правило, некоторую сложную систему массового обслуживания.

Основные задачи, которые необходимо решить:
- Определение принципов организации вычислительной системы;
- Выбор архитектуры, уточнение функции и их разделение на подфункции, реализуемое аппаратным или программным способом;
- Разработка структурной схемы, т.е. определение состава устройств и способов их взаимодействия;
- Определение требований к выходным параметров устройств и формирование технического задания для разработки отдельных устройств.

### 4. Исследование сложных дискретных структур с очередями. Уравнение Колмогорова.
Исследование сложных дискретных структур с очередями - это тема научной работы какого-то бауманского мудака-Корягина
https://math.semestr.ru/cmo/kolmogorov.php

### 5. Моделирование систем и языки моделирования, классификация языков имитационного моделирования

Алгоритмические языки при моделировании систем служат вспомогательным аппаратом в разработке машинной реализации и анализа характеристик моделей. Основная задача– это выбор языка.

Каждый язык имеет свою систему абстракций, лежащую в основе формализации функционирования сложных систем.

Для программирования модели могут использоваться следующие языки:
1. Универсальные алгоритмические языки высокого уровня.
2. Специализированные языки моделирования: языки, реализующие событийный подход, подход сканирования активностей, языки, реализующие процессно-ориентированный подход.
3. Проблемно-ориентированные языки и системы моделирования.

Качество языков моделирования характеризуется:
- Удобство описания процесса функционирования;
- Удобство ввода исходных данных, варьирования структуры, алгоритмов работы и параметров модели;
- Эффективностью анализа и вывода результатов моделирования;
- Простотой отладки и контроля работы моделирующей программы;
- Доступностью восприятия и использования языка.

В большинстве своем языки моделирования определяют поведение систем во времени с помощью модифицированного событийного алгоритма. Как правило, он включает в себя список текущих и будущих событий.

#### Классификация языков имитационного моделирования.

![схема](https://studfile.net/html/764/338/html_hQRGVZIBMF.yJus/img-budrau.png)

Непрерывное представление систем сводится к представлению дифференциальных уравнений, с помощью которых устанавливают связь между входной и выходной функциям. Если выходные переменные модели принимают дискретные значения, то уравнения являются разностными.

GASP– комбинированный, в основе лежит язык FORTRAN. Предполагается, что в системе могут наступать события двух типов:

1. события, зависящие от состояния
2. события, зависящие от времени.

Состояние системы описывается набором переменных, причем некоторые из них меняются непрерывно. При таком подходе пользователь должен составлять процедуры, описывающие условия наступления событий. Законы изменения непрерывных переменных, правила перехода от одного состояния к другому, т.е. реализуется классический принцип ДУ.

Группы языков моделирования, ориентированные на дискретное время, используется при построении именно имитационных моделей, но при этом используются разные способы описания динамического поведения исследуемого объекта.

### 7. Методология вычислительного эксперимента в науке и технике. Понятие корректности постановки задач моделирования. Методы построения математических моделей 
#### Методология вычислительного эксперимента в науке и технике

Вычислительным экспериментом называется методология и технология исследований, основанные на применении прикладной математики и ЭВМ как технической базы при использовании ММ (математического моделирования). Вычислительный эксперимент основывается на создании ММ изучаемых объектов, которые формируются с помощью некоторой особой математической структуры, способной отражать свойства объекта, проявляемые им в различных экспериментальных условиях.

Процесс построения любой математической модели можно представить последовательностью этапов:

1. Обследование объекта моделирования и формулировка технического задания на разработку модели (содержательная постановка задачи);
2. Концептуальная и математическая постановка задачи;
3. Качественный анализ и проверка корректности модели;
4. Выбор и обоснование выбора методов решения задачи;
5. Поиск решения;
6. Разработка алгоритма решения и исследование его свойств, реализация алгоритма в виде программ;
7. Проверка адекватности модели;
8. Практическое использование построенной модели.

<i>Подробнее про все пункты: http://systems-analysis.ru/mathmodeling_process.html</i>

#### Понятие корректности постановки задач моделирования

Понятие корректности задачи имеет большое значение в при­кладной математике. Например, численные методы решения оправ­дано применять лишь к корректно поставленным задачам. При этом далеко не все задачи, возникающие на практике, можно считать корректными (например, так называемые обратные задачи). Дока­зательство корректности конкретной математической задачи - до­статочно сложная проблема, она решена только для некоторого класса математически поставленных задач. Проверка математичес­кой замкнутости является менее сложной по сравнению с провер­кой корректности математической постановки. В настоящее время активно исследуются свойства некорректных задач, разрабатывают­ся методы их решения. Аналогично понятию «корректно поставлен­ная задача» можно ввести понятие «корректная математическая модель».

Математическая модель является корректной,если для нее осу­ществлен и получен положительный результат всех контрольных проверок: размерности, порядков, характера зависимостей, экстре­мальных ситуаций, граничных условий, физического смысла и ма­тематической замкнутости.

#### Методы построения математических моделей
1. Экспериментальный
2. Аналитический
3. Экспериментально-аналитический
   
#### Экспериментальный
При построении методов управления требуются знания статики, динамики объекта в узком диапазоне вокруг рабочей точки.

Допускаются предположения:
- линейность объекта;
- сосредоточенность параметров;
- стационарность.

Эти допущения позволяют использовать линейные статические модели: и линейные дифференциальные уравнения и определять их экспериментальными методами на каждом объекте управления.

Достоинства и недостатки

- Достоинства: простота управления, малая трудоемкость.
- Недостатки метода: нельзя использовать модели при переходе на другую рабочую точку, нельзя использовать модель на другом объекте.

#### Аналитический
При составлении моделей аналитическим путем используются уравнения материального, энергетического баланса и другие.

Используется для построения моделей при оптимизации процессов. При этом учитываются физико-химические процессы, характеристики сырья, режимы параметров, параметры оборудования.

Достоинства и недостатки

- Достоинства: строится более общая модель, не требуется экспериментов на объекте, можно применять на других объектах управления.
- Недостатки: невысокая точность, сложность процесса построения моделей, необходимость лабораторных исследований. При определении коэффициентов кинетики химических процессов, гидродинамики, тепло процессов и т. д.

По многим параметрам и режимам делаются допущения о механизме процесса. (например, при идеальном перемешивании продукта в химическом реакторе имеются ошибки в описании и точность не высока).

#### Экспериментально-аналитический
Для повышения точности моделей, полученных аналитическим методом, на объекте управления проводят серию экспериментов и уточняют модель. Такой метод – экспериментально-аналитический. Метод позволяет использовать и экспериментальный, и аналитический методы. Точность моделей, по полученному вектору коэффициентов В можно использовать только на объекте, где производятся эксперименты.

### 8. Современные системы научно-технических расчетов и моделирования (MatLab, Mathcad). Общая характеристика и особенности применения в вычислительных экспериментах.

Matlab, Mathcad, а также - бонус - Maple и Mathematica - это системы, относящиеся к разделу CAE (Computer Aided Engeneering) инженерного проектирования.
Системы MathСad и MATLAB - системы автоматизации математических расчетов, построенные на расширенном представлении и применении матричных операций. Применение матриц, как основных объектов системы, способствует уменьшению числа циклов, которые очень распространены при выполнении матричных вычислений на обычных языках программирования высокого уровня, и облегчению реализации параллельных вычислений.

Спектр задач, решаемых этими системами, очень широк:

- проведение математических исследований, требующих вычислений и аналитических выкладок;
- разработка и анализ алгоритмов;
- математическое моделирование и компьютерный эксперимент;
- анализ и обработка данных;
- визуализация, научная и инженерная графика;
- разработка графических и расчетных приложений.

Поскольку CAE-системы содержат операторы для базовых вычислений, то почти все алгоритмы, отсутствующие в стандартных функциях, можно реализовать посредством написания собственной программы. 

В данных математических пакетах применяется принцип конструирования модели, а не традиционное «искусство программирования». То есть пользователь лишь ставит задачу, а методы и алгоритмы решения система находит сама. Более того, такие рутинные операции, как раскрывание скобок, преобразование выражений, нахождение корней уравнений, производных и неопределенных интегралов компьютер самостоятельно осуществляет в символьном виде, причем практически без вмешательства пользователя.

<i>Не знаю, как подробно нужно давать ответы на вопросы по этой теме, подробнее об отличиях Matlab и Mathcad здесь (наверное, стоит один раз прочитать, всего 4 страницы):</i> https://cyberleninka.ru/article/n/programmnaya-realizatsiya-statisticheskoy-obrabotki-dannyh-sistemy-mathcad-i-matlab/viewer

### 9. Основные задачи линейной алгебры, решаемые при математическом моделировании. Плохо обусловленные системы. Нелинейные уравнения и системы нелинейных уравнений.

#### Плохо обусловленные системы

<b>Плохо обусловленная система</b> — это система, у которой определитель А не равен нулю, но число обусловленности |А-1| |А| очень велико. Несмотря на то, что плохо обусловленные системы имеют единственное решение, на практике искать это решение чаще всего не имеет смысла. Рассмотрим свойства плохо обусловленных СЛАУ на двух конкретных примерах:

![пример](https://radiomaster.ru/cad/mc12/glava_08/24.gif)

Пример содержит решение двух очень близких плохо обусловленных СЛАУ (с одинаковой правой частью ь и мало отличающимися матрицами А). Несмотря на близость, точные решения этих систем оказываются очень далекими друг от друга. Надо заметить, что для системы двух уравнений точное решение получить легко, однако при решении СЛАУ большой размерности незначительные ошибки округления, неминуемо накапливаемые при расчетах (в том числе и "точным" алгоритмом Гаусса), приводят к огромным погрешностям результата. Возникает вопрос: имеет ли смысл искать численное решение, если заранее известно, что, в силу неустойчивости самой задачи, оно может оказаться совершенно неправильным?

Чтобы лучше понять причину некорректности, полезно сравнить графическую интерпретацию хорошо и плохо обусловленной системы двух уравнений. Решение системы визуализируется точкой пересечения двух прямых линий, изображающих каждое из уравнений.

Хорошо обусловленная:

![пример](https://radiomaster.ru/cad/mc12/glava_08/25.gif)

Плохо обусловленная

![пример](https://radiomaster.ru/cad/mc12/glava_08/26.gif)

Плохая обусловленность матрицы типична и при реконструкции экспериментальных данных, задаваемых переопределенными (несовместными) СЛАУ (например, в задачах томографии).

Для решения некорректных задач, в частности, вырожденных и плохо обусловленных СЛАУ, используется регуляризация. В ее основе лежит учет дополнительной априорной информации о структуре решения (векторе априорной оценки хо), которая очень часто присутствует в практических случаях. Задачу решения СЛАУ Аx=b можно заменить задачей отыскания минимума функционала Тихонова:

Ω(х,λ) = |Ах-b|^2+λ|х-х0|^2

Здесь λ, — малый положительный параметр регуляризации, который необходимо подобрать некоторым оптимальным способом. Можно показать, что задачу минимизации функционала Тихонова можно, в свою очередь, свести к решению другой СЛАУ:

(АTА+λI)-х=АTВ+λх0, <i>(AT = A транспонированная)</i>

которая при λ->0 переходит в исходную плохо обусловленную систему, а при больших x, будучи хорошо обусловленной, имеет решение х0. Очевидно, оптимальным будет некоторое промежуточное значение А, устанавливающее определенный компромисс между приемлемой обусловленностью и близостью к исходной задаче.

#### Нелинейные уравнения и системы нелинейных уравнений.

[РЕШЕНИЕ НЕЛИНЕЙНЫХ УРАВНЕНИЙ И СИСТЕМ НЕЛИНЕЙНЫХ УРАВНЕНИЙ](https://mainfodotru.files.wordpress.com/2017/09/numeric-methods-part2.pdf)

[Методы решения систем нелинейных уравнений](http://mathhelpplanet.com/static.php?p=metody-resheniya-sistem-nelineynykh-uravneniy)

### 10. Аппроксимация функций в задачах моделирования. Многомерная интерполяция. Наилучшее линейное и нелинейное среднеквадратичное приближения.

#### Аппроксимация функций в задачах моделирования.

<b>Аппроксимация</b> – это замена одних математических объектов другими, которые в определённом смысле близки к исходным и более просты и удобны. Исходными данными для аппроксимации в задачах моделирования могут являться эмпирические данные или результаты предварительного моделирования отдельных наиболее сложных элементов модели. Кроме того, часто практикуется замена точных сложных моделей на приближенные, но значительно более простые соотношения с целью сокращения времени моделирования.

Наиболее часто исходными данными для аппроксимации является множество табличных данных, которые называют узловыми точками

<b>Аппроксимацией (приближением) функции</b> f(x) называется нахождение такой функции (аппроксимирующей функции) g(x), которая была бы близка заданной. Критерии близости функций могут быть различные.

В случае если аппроксимация проводится на непрерывном множестве точек (отрезке), аппроксимация называется непрерывной или интегральной. Примером такой аппроксимации может служить разложение функции в ряд Тейлора, то есть замена некоторой функции степенным многочленом.

Наиболее часто встречающим видом точечной аппроксимации является интерполяция – нахождение промежуточных значений величины по имеющемуся дискретному набору известных значений.

Пусть задан дискретный набор точек, называемых узлами интерполяции, а также значения функции в этих точках. Требуется построить функцию g(x), проходящую наиболее близко ко всем заданным узлам. Таким образом, критерием близости функции является g(xi)=yi.

В качестве функции g(x) обычно выбирается полином, который называют интерполяционным полиномом.

В случае если полином един для всей области интерполяции, говорят, что интерполяция глобальная.

В случае если между различными узлами полиномы различны, говорят о кусочной или локальной интерполяции.

Найдя интерполяционный полином, мы можем вычислить значения функции между узлами, а также определить значение функции даже за пределами заданного интервала (провести экстраполяцию).

<b>Аппроксимация линейной функцией</b>

Любая линейная функция может быть записана уравнением ![уравнение](https://prog-cpp.ru/wp-content/uploads/2016-12-28_17-55-55.png). Аппроксимация заключается в отыскании коэффициентов a и b уравнения таких, чтобы все экспериментальные точки лежали наиболее близко к аппроксимирующей прямой.

С этой целью чаще всего используется метод наименьших квадратов (МНК), суть которого заключается в следующем: сумма квадратов отклонений значения точки от аппроксимирующей точки принимает минимальное значение: 

![МНК](https://prog-cpp.ru/wp-content/uploads/2016-12-28_17-56-25.png)

<b>Теорема Цыбенко, Универсальная теорема аппроксимации</b> — теорема, доказанная Джорджем Цыбенко в 1989 году, которая утверждает, что искусственная нейронная сеть прямой связи (англ. feed-forward; в которых связи не образуют циклов) с одним скрытым слоем может аппроксимировать любую непрерывную функцию многих переменных с любой точностью. Условиями являются: достаточное количество нейронов скрытого слоя, удачный подбор ${\displaystyle \mathbf {w} _{1},\mathbf {w} _{2},\dots ,\mathbf {w} _{N},\mathbf {\alpha } ,}$ и ${\displaystyle \mathbf {\theta } }$, где

${\displaystyle \mathbf {w} _{i}}$ — веса между входными нейронами и нейронами скрытого слоя,

${\displaystyle \mathbf {\alpha } }$ — веса между связями от нейронов скрытого слоя и выходным нейроном,

${\displaystyle \mathbf {\theta } }$ — смещения для нейронов входного слоя.

#### Многомерная интерполяция

### 11. Алгоритмы численного интегрирования функций одной переменной. Формулы Рунге. Сходимость квадратурных формул. Нелинейные формулы. Вычисление многомерных интегралов.

Сначала стоит прочитать [это](http://solidstate.petrsu.ru/p/tutorial/meth_calc/files/04.shtml), потом [это](http://solidstate.petrsu.ru/p/tutorial/meth_calc/files/05.shtml)

#### Алгоритмы численного интегрирования функций одной переменной
Квадратурные формулы - формулы для численных методов интегрирования

<b>Методы прямоугольников</b>

Метод численного интегрирования функции одной переменной, заключающийся в замене подынтегральной функции на многочлен нулевой степени, то есть константу, на каждом элементарном отрезке. Если рассмотреть график подынтегральной функции, то метод будет заключаться в приближённом вычислении площади под графиком суммированием площадей конечного числа прямоугольников, ширина которых будет определяться расстоянием между соответствующими соседними узлами интегрирования, а высота — значением подынтегральной функции в этих узлах. Алгебраический порядок точности равен 0. (Для формулы средних прямоугольников равен 1).

<i>Алгебраический порядок точности численного метода (порядок точности численного метода, степень точности численного метода, порядок точности, степень точности) — наибольшая степень полинома, для которой численный метод даёт точное решение задачи.

Другое определение: говорят, что численный метод имеет порядок точности ${\displaystyle d}$, если его остаток ${\displaystyle R_{n}}$ равен нулю для любого полинома степени ${\displaystyle d}$, но не равен нулю для полинома степени ${\displaystyle d+1}$</i>



- Метод левых прямоугольников
  
  ![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/724605531ba4757a6675c9e3002d70946d27839a)

- Правых
  
  ![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/3e0e39e50a25cb1a9233e54971eb2bcddba2ae6b)
- Средних 

  ![s](https://wikimedia.org/api/rest_v1/media/math/render/svg/7869e8ec9ac3217822dc8519816c54b41bc02af1)

![s](https://studfile.net/html/2706/297/html_OxZSXTVw5n.niFf/img-HfuG21.png)
  
<b>Метод трапеций</b>

![s](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image064.png)

![s](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/glava2_clip_image012.png)

Метод трапеций имеет второй порядок алгебраической точности

<b>Метод Симпсона</b>

В этом методе подынтегральная функция на частичном отрезке ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image051.png) аппроксимируется параболой, проходящей через три точки ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image066.png), ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image067.png), ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image068.png), то есть интерполяционным многочленом Лагранжа второй степени.

На отрезке  формула Симпсона примет вид:

![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image071.png)

Если разбить отрезок интегрирования ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image072.png) на четное количество 2N равных частей с шагом ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image073.png), то можно построить параболу на каждом сдвоенном частичном отрезке ![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image073.png) и переписать выражение выше без дробных индексов. Тогда формула Симпсона примет вид:

![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/image074.png)

![i](http://aco.ifmo.ru/el_books/numerical_methods/lectures/images/glava2_clip_image025.png)

Метод Симпсона имеет порядок погрешности 4 и алгебраический порядок точности 3.

<b>Оценка погрешности</b>

Для оценки погрешности численных методов используется <b>правило Рунге</b>. Основная идея состоит в вычислении приближения выбранным методом с шагом h, а затем с шагом h/2, и дальнейшем рассмотрении разностей погрешностей для этих двух вычислений.

<b>Метод Гаусса</b>

![i](https://cf.ppt-online.org/files/slide/f/fiud0OWsqY8HVyxz2wUtl6ZKj1bS3BIMRDELcJ/slide-9.jpg)

Квадратура Гаусса относится к квадратурам открытого типа. Это означает, что ни один и узлов не совпадает ни с одним из концов отрезка интегрирования a или b.

Веса квадратур Гаусса всегда положительны, и при увеличении числа узлов точность приближения почти всегда возрастает.

Недостаток метода Гаусса состоит в том, что он не имеет лёгкого (с вычислительной точки зрения) пути оценки погрешности полученного значения интеграла. Использование правила Рунге при дроблении отрезка интегрирования требует вычисления подынтегральной функции примерно в таком же числе точек, не давая при этом практически никакого выигрыша в точности, в отличие от простых методов, где точность увеличивается в несколько раз при каждом новом разбиении. Кронродом был предложен следующий метод оценки значения интеграла

${\displaystyle I\approx \sum _{i=1}^{n}a_{i}\,f(x_{i})+\sum _{i=1}^{n+1}b_{i}\,f(y_{i})}$,

где ${\displaystyle x_{i}}$ — узлы метода Гаусса по ${\displaystyle n}$ точкам, а ${\displaystyle 3n+2}$ параметров ${\displaystyle a_{i}}$, ${\displaystyle b_{i}}$, ${\displaystyle y_{i}}$ подобраны таким образом, чтобы порядок точности метода был равен ${\displaystyle 3n+1}$. Тогда для оценки погрешности можно использовать эмпирическую формулу:

${\displaystyle \Delta =\left(200|I-I_{G}|\right)^{1.5}}$,

где ${\displaystyle I_{G}}$ — приближённое значение интеграла, полученное методом Гаусса по ${\displaystyle n}$ точкам. 

#### Сходимость квадратурных формул и нелинейные формулы

Простых ответов не будет

![i](https://scask.ru/htm/stu.sernam/book_dig_m/1/86.gif)

![i](https://scask.ru/htm/stu.sernam/book_dig_m/1/87.gif)

![i](https://scask.ru/htm/stu.sernam/book_dig_m/1/88.gif)

![i](https://scask.ru/htm/stu.sernam/book_dig_m/1/89.gif)

![i](https://scask.ru/htm/stu.sernam/book_dig_m/1/90.gif)

![i](https://scask.ru/htm/stu.sernam/book_dig_m/1/91.gif)

#### Вычисление многомерных интегралов.

С помощью метода Монте-Карло. Все. (Как у Серова искали площадь какого-то многоугольника)

### 12. Математические модели на основе обыкновенных дифференциальных уравнений. Постановки задач. Неявные схемы. Интегрирование жестких систем уравнений.

<i>Начиная с этого раздела, темы касаются разностных схем. Вообще это все трэш</i>

#### Математические модели на основе обыкновенных дифференциальных уравнений

Значительная часть проблем, с которыми имеет дело вычислительная математика, представляет собой различные задачи для обыкновенных дифференциальных уравнений и уравнений с частными производными. Так, например, <b>обыкновенными дифференциальными уравнениями можно описать задачи химической кинетики, электрических цепей, движение систем взаимодействующих материальных точек и другие задачи физики, химии, техники. </b> К дифференциальным уравнениям в частных производных приводятся задачи математической физики, гидродинамики, акустики и других областей знаний. Все методы решения дифференциальных уравнений можно условно разбить на две группы: аналитические и численные. В свою очередь аналитические методы подразделяются на точные и приближенные. Точные методы позволяют выразить решение дифференциальных уравнений через элементарные функции (в аналитическом виде). 

<i>Следующий абзац важен для понимания сути разностных схем</i>

Приближенными называются методы, в которых решение получается как предел некоторой последовательности, члены которой выражаются через элементарные функции. <b>Численные методы не позволяют найти точное решение дифференциальных уравнений в аналитической форме. С их помощью получается таблица приближенных (иногда точных) значений искомого решения в некоторых точках рассматриваемой области решения, именуемых сеткой. В силу этого численные методы называют иначе разностными методами или методами сеток. </b> Численные методы применимы к широким классам дифференциальных уравнений и всем типам краевых задач для них.

Понятия сетки и сеточной функции возникают в теории разностных схем в связи с изучением численных методов решения краевых задач математической физики. Для построения численного метода необходимо написать разностную схему, приближенно описывающую дифференциальное уравнение (или систему). Этот этап связан с заменой области непрерывного изменения аргумента областью дискретного его изменения и с заменой дифференциального оператора некоторым его разностным аналогом, кроме того, записывается разностная аппроксимация для начальных и граничных условий. Результатом этой процедуры является алгебраическая система уравнений или система разностных уравнений. Численное решение краевой задачи для исходного линейного дифференциального уравнения сводится к решению полученной алгебраической системы.

#### Неявные схемы

<b>Явные схемы</b>

Явные схемы вычисляют значение сеточной функции через данные соседних точек. Пример явной схемы для дифференцирования: ${\displaystyle f'(x)={\frac {f(x+h)-f(x-h)}{2h}}}$ (2-й порядок аппроксимации). Явные схемы часто оказываются неустойчивыми.

<b>Неявные схемы</b>

Неявные схемы используют уравнения, которые выражают данные через несколько соседних точек результата. Для нахождения результата решается система линейных уравнений. Пример неявной схемы для уравнения струны: ${\displaystyle f(x,t+h)-2f(x,t)+f(x,t-h)=f(x+h,t+h)-2f(x,t+h)+f(x-h,t+h)}$. Неявные схемы обычно являются устойчивыми.

#### Интегрирование жестких систем уравнений

Жёсткой системой обыкновенных дифференциальных уравнений (ОДУ) называется (нестрого говоря) такая система ОДУ, численное решение которой явными методами (например, методами Рунге — Кутты или Адамса) является неудовлетворительным из-за резкого увеличения числа вычислений (при малом шаге интегрирования) или из-за резкого возрастания погрешности (так называемого, взрыва погрешности) при недостаточно малом шаге. <b>Для жёстких систем характерно то, что для них неявные методы дают лучший результат, обычно несравненно более хороший, чем явные методы.</b>

Численные методы решения ОДУ делятся на одношаговые и многошаговые, которые в свою очередь можно разделить на явные и неявные. 

<b>Явные одношаговые методы можно записать в виде:</b>

$y_{k+1} = y_{k} + hФ(x_{k}, y_{k})$,

где для простоты полагаем $h_{k}=h$, через ук будем обозначать приближенное решение в точке $x_{k}$, а у(х) – точное решение, в частности, у($x_{k}$) – точное решение в точке $x_{k}$. Для продвижения на один шаг одношаговые методы используют значения решения лишь в одной предыдущей точке.

<b>Явные многошаговые методы используют решение в нескольких предыдущих точках:</b>

$y_{k+1} = y_{k} + hФ(x_{k}, y_{k}, y_{k-1}, ... , y_{k-m})$

<b>Неявные одношаговые методы записываются в виде:</b>

$y_{k+1} = y_{k} + hФ(x_{k+1}, y_{k+1})$,

<b>Неявные многошаговые:</b>

$y_{k+1} = y_{k} + hФ(x_{k+1}, y_{k+1}, y_{k}, ... , y_{k-(m-1)})$

В неявных методах для нахождения $y_{k+1}$ требуется решить, вообще говоря, нелинейное уравнение или в общем случае систему уравнений.

### 13. Математические модели на основе обыкновенных дифференциальных уравнений. Краевые задачи. Уравнения с разрывными коэффициентами.

#### Краевые задачи
Краевая задача (граничная задача) — задача о нахождении решения заданного дифференциального уравнения (системы дифференциальных уравнений), удовлетворяющего краевым (граничным) условиям в концах интервала или на границе области. Краевые задачи для гиперболических и параболических уравнений часто называют начально-краевыми или смешанными, потому что в них задаются не только граничные, но и начальные условия.

x′′ + A(t)x + B(t)x′ = c(t),   t ∈ [0, T],	(LE)
x(0) = a,   x(T) = b,

<b>Решение краевых задач</b>

Большинство используемых численных методов решения краевых задач может быть отнесено к одному из трех больших классов. Разумеется, границы между этими методами размыты, некоторые методы нельзя отнести ни к одному из этих классов, другие же могут быть отнесены одновременно к двум классам и т. д. 

а) Методы стрельбы. 

б) Конечно-разностные методы, основывающиеся на построении разностных схем, аппроксимирующих решение исходной задачи.

в) Проекционные, или вариационные, методы, суть которых состоит в проектировании исходной задачи на конечномерное пространство функций.