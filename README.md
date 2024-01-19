## Project: MAINCLU

MAINCLU is a technology that recognizes non-standard speech and converts it into text or voice assistance. Our voice assistant aids individuals with speech disorders, such as dysarthria.

Choose from two options:
- Convert my speech to text
- Convert my speech to voice assistance

We simplify your life, caring for your well-being. 🚀

## Running the Project

Follow these simple steps to run the project:

1. *Clone the repository* to your local machine:

   ```shell
   git clone https://github.com/VorkhlikAS/MAINCLU.git

2. *Change to the project directory*:

   ```shell
   cd ./MAINCLU/app

3. *Build and run the project* using the provided Makefile:

   ```shell
   make

That's it! Your project should now be up and running.


## Дизайн ML системы - MAINCLU

MAINCLU — это голосовой помощник, созданный с использованием технологий машинного
обучения и разработанный для улучшения коммуникации и повышения качества жизни у людейс нарушением речи. Данное решение предназначено для облегчения коммуникации и помощи в повседневных задачах людям, страдающим от дизартрии и других нарушений речи

## 1. Цели и предпосылки

### 1.1. Зачем идем в разработку продукта?

- Бизнес-цель
    - Распознавание и интерпретация нарушенной речи: Основной задачей является разработка высокоэффективных алгоритмов и моделей машинного обучения для точного распознавания и интерпретации разнообразных форм нарушений речи, включая дизартрию. Это включает в себя учет индивидуальных особенностей пользователей.
    - Интуитивный пользовательский интерфейс: Не менее важным является создание пользовательского интерфейса, который будет максимально интуитивным и доступным для пользователей с нарушением речи, даже при наличии различных степеней ограниченности. Это позволит пользователям комфортно и эффективно взаимодействовать с системой.
    - Индивидуальная адаптация и обучение: Разработка механизмов для индивидуальной
    адаптации системы к каждому пользователю является неотъемлемой частью цели проекта. Это позволит системе постоянно улучшаться и настраиваться под изменяющиеся потребности пользователей.
    - Социальная инклюзия: Главным образом, целью НИОКР является создание продукта,
    способного значительно улучшить качество жизни и общение людей с нарушением речи. Посредством улучшения коммуникации и обеспечения возможности для более эффективного общения, мы стремимся способствовать социальной инклюзии и повышению самостоятельности данной аудитории.
    - Профессиональное и медицинское применение: Кроме того, нашей целью является создание инструмента, который будет полезен в медицинских учреждениях и для специалистов в области речевой терапии, помогая им лучше взаимодействовать и работать с пациентами, страдающими от нарушений речи.
    - Общей целью является разработка инновационной технологии MAINCLU, которая
    позволит значительно улучшить качество жизни и общение людей с нарушением речи, а также способствовать их социальной интеграции и самостоятельности в повседневной жизни и профессиональной деятельности.
- Почему необходимо использовать ML
    - Для каждого человека с нарушениями речи важна индивидуальная настройка инструмента распознавания его речи в виду того, что степени нарушения речи могут отличаться, как могут и отличаться и другие индивидульные особенности речи. Нейронная сеть может быть дообучена на речи конкретного человека, то есть настроена для того, чтобы этот человек мог ей пользоваться с максимальным уровнем комфорта.
    - Что будем считать успехом с точки зрения бизнеса
        
        Для измерения критерия успеха используем окупаемость 
        системы. Доходом является продажа системы другим бизнесам (часть B2B-сегмента, использующая голосовые ассистенты), прямые продажи подписки на функции приложения (B2C - сегмент), в перспективе - получение контрактов от государства для внедрения системы в государственные учреждения, например, МФЦ, медицинские учреждения.
        Затратами являются затраты на разработку и сопровождение. При 
        окупаемости за `N` месяцев считаем успешным внедрением.
        
        Для оценки будем использовать следующие ключевые показатели:
        
        1. Повышение точности распознавания речи
        2. Поддержание или увеличение клиентской базы за счет улучшения качества распознавания и соответствующего увеличения доверия.
- Стоимость
    - Затраты на расширение датасета: сбор данных требует вовлеченности большого количества людей с нарушениями речи, согласных принимать  участие в сборе данных в качестве спикеров (возможно, потребуется предоставить им особые условия по помощи им в прибытии на место звукозаписи), также требуется найти людей, которые бережно и аккуратно помогут спикерам принять участие в записи, а также корректно задокументировать полученные записи. Также понадобятся специальные технические средства для записи (микрофоны, помещения с шумоизоляцией)
    - Затраты на работу датасаентистов: Включает зарплаты и прочие
    расходы, связанные с наймом и содержанием команды датасаентистов,
    занимающихся разработкой и обслуживанием ML-моделей для Speech Recognition системы
    - Затраты на инфраструктуру ML-моделей: Это включает расходы, связанны с необходимой инфраструктурой для развертывания и работы ML-моделей .
    Это может включать в себя затраты на вычислительные ресурсы (например,
    серверы или облачные вычисления), хранение данных, сетевую
    инфраструктуру, обеспечение безопасности и т.д. Инфраструктура
    ML-моделей может быть дорогостоящей и требовать постоянной поддержки и
    обновлений, особенно при обработке больших объемов данных или в условиях высоких требований к производительности и доступности системы.
    - Затраты на зарплаты разработчиков приложений (мобильного и веб)
    - Затраты на хостинг приложений

### 1.2. Бизнес-требования и ограничения

- Краткое описание бизнес-требований. Проект направлен на создание инклюзивной среды для людей с нарушениями речи путем разработки системы на основе Speech Recognition. Бизнес-требования включают создание датасета, создание и интеграцию (в системы сегмента B2B, приложение) модели, которая может обрабатывать входные голосовые данные, разработку приложения, а также может быть дообучена под конкретного пользователя.
- Бизнес-ограничения. Включают ограниченный тайминг, в рамках которого следует распознавать устную речь. Кроме того, система должна приблизиться к максимальной точности распознавания текста, чтобы не ухудшать клиентский опыт и не приводить к потере клиентов.
- Описание бизнес-процесса пилота
    - После разработки и тестирования ML-модель будет интегрирована в
    разрабатываемое параллельно в созданный ранее Телеграм-бот, а также разрабатываемое параллельно мобильное приложение. Входные голосовые данные будут подаваться на вход модели, которая будет генерировать их голосовую или текстовую интерпретацию.
    - Во время пилотного проекта мы будем тщательно отслеживать точность распознавания речи.
    - Система будет содержать персональные данные (записи голоса, которые злоумышленники могут украсть и подделать с целью шантажа, мошенничества и т.п.), поэтому ее необходимо должным образом защитить.
- Что считаем успешным пилотом. Успешным пилотом можно считать
положительную экономическую оценку, основываясь на бизнес метрике (пункт 1.5):
- Возможные пути развития проекта:
    - расширение обучающего набора данных
    - интеграция во все сегменты рынка (B2B, B2C, B2G)
    - расширение клиентской базы

### 1.3. Что входит в скоуп проекта/итерации, что не входит

- Что не будет закрыто
    - Возможно, на данном этапе работать придется только с уже существующим датасетом записей голоса людей, а не записывать самостоятельно
    - На данном этапе не будет интеграции системы в сегменты B2B и B2G
- Описание результата с точки зрения качества кода и воспроизводимости решения
    - Результат проекта будет включать в себя четко описанный и
    документированный код, который можно легко внедрить в существующую
    систему. Модель должна быть обучена и протестирована, а ее
    производительность должна быть оценена с использованием отдельного
    тестового набора данных. Код будет структурирован таким образом, чтобы
    обеспечить воспроизводимость.
- Описание планируемого технического долга
    - Возможные аспекты технического долга могут включать оптимизацию
    алгоритмов для улучшения производительности, интерпретируемости и
    интеграции решения.
- Скоуп итерации:
1. Сбор и аннотация данных
2. Разработка моделей машинного обучения:
3. Интерфейс и дизайн:
Наша команда дизайнеров и разработчиков создаст интуитивно понятный пользовательский интерфейс, который будет удовлетворять потребности пользователей с нарушением речи и обеспечивать удобство использования.
4. Индивидуальная адаптация:
Разработаем механизмы для индивидуальной адаптации системы к конкретным пользователям, что позволит улучшить точность распознавания и комфортность использования.
5. Тестирование и оптимизация:
После создания прототипа системы мы проведем тщательное тестирование с участием целевой аудитории и внесем необходимые коррективы для оптимизации производительности и качества системы.
6. Внедрение и обучение:
Мы разработаем план внедрения MAINCLU в медицинские учреждения и среди специалистов в области речевой терапии, а также в обычную жизнь людей: рабочие процессы, повседневное общение и т.д. Обеспечим обучение пользователей и специалистов в использовании системы.

### 1.4. Предпосылки решения

- **Данные.** Наше решение будет базироваться на датасете записей русской речи людей с нарушениями голоса. Также предполагается расширять датасет записей.
- **Процесс.** Мы предполагаем, что модель будет интегрирована в разрабатываемое мобильное приложение, пользователь будет иметь возможность получить результат распознавание его речи в голосовом и текстовом виде

### 1.5. **Бизнес-метрики**

Определяем ключевые показатели, которые далее агрегируем в единую формулу в деньгах, понятную бизнесу. Показателями являются:

- Прирост количества постоянных пользователей приложения
- Количество обращений в поддержку: это позволяет измерить, насколько
успешно системы распознает речь.

## 2. Методология

### 2.1. Постановка задачи

Задача распознавания устной речи

### 2.2. Блок-схема решения

Нет

### 2.3. Этапы решения задачи

### 2.3.1 Выбор метрик

**Оффлайн-метрики** - это метрики, оценивающие производительность системы  на основе исторических данных и фактических результатов.

1. Точность распознавания речи (STT):
Точность перевода голосовых записей в текстовый формат. Значение должно находиться в диапазоне не менее 85%.
2. Полнота распознавания речи (STT):
Способность системы к распознаванию всего произнесенного пользователем текста. Полнота не менее 90%.
3. Точность синтеза речи (TTS):
Точность воспроизведения текста в стандартной речи. Значение не менее 90%

**Онлайн метрики** -  это метрики, которые мы можем получить во время работы системы.

Активность использования клиентами приложения (количество запросов, продолжительность записанных аудио)

**Технические метрики** - это метрики, связанные с производительностью и скоростью работы системы антифрод. Некоторые примеры таких метрик включают:

1. Максимальное количество одновременно работающих пользователей (серверная часть):
Количество пользователей, которые могут одновременно использовать серверную часть
приложения. Максимальное количество пользователей не менее 1000.
2. Скорость обработки голосовых записей:
Среднее время, требуемое для обработки голосовой записи и предоставления результата
пользователю. Скорость обработки не более 5 секунд на голосовую запись продолжительностью 1 минута.
3. Пропускная способность сервера:
Пропускная способность серверной инфраструктуры, которая обеспечивает плавную работу приложения с указанным максимальным количеством одновременных пользователей. Пропускная способность должна быть не менее 100 запросов в секунду на сервер.

### 2.3.2 Определение объекта и таргета

- Объект - запись голоса человека
- Целевая переменная: результат распознавания записи голоса - текст или аудиозапись

### 2.3.3 Сбор данных

### 2.3.4 Подготовка данных

Этап 0: Валидация и корректировка существующего датасета

Этап 1: Запись голосов дикторов с помощью подготовленных текстов

**Результат:** Чистый и корректный набор данных для задачи

### 2.3.5 Подготовка тренировочного и тестового наборов данных

### 2.3.6 Валидация

В качестве метрики валидации используется Word Recognition Rate (WRR) и WER (Word error rate)

### 2.3.7 Выбор архитектуры модели для решения задачи

**Этап 1 (MVP)**. Доучивание (сначала для русского языка, потом для русского языка с нарушениями речи) и тестирование избранных моделей — Whisper, PaddleSpeech, Athena, Vosk и т.д. 

**Этап 2**. Тестирование оптимизаций для лучших моделей.

Данный этап включает в себя варьирование гиперпараметров —
математических и эвристических показателей модели, для её улучшения, а 
так же подбор подходящих признаков

**Этап 4**. Сопоставление качества проверенных моделей по целевой метрике. Выбор конечной архитектуры/структуры модели.

**Результат:** Выбраны приоритетная модель и ее гиперпараметры для дальнейшей оптимизации

### 2.3.8 Анализ ошибок

Анализ наличия и природы ошибок в MVP. Проверка модели при
 помощи методов интерпретации, оценка корректности гиперпараметров. При 
необходимости возвращение к пунктам 2.3.4—2.3.8.

**Результат:** Модель, достигающая качества на тестовом наборе данных, соответствующего бизнес требованиям.

**Необходимая проверка бизнеса:** Согласованность качества модели с требованиями бизнеса;

## 3. Подготовка пилота

Для монетизации нашего продукта мы выбираем бизнес-модель “Freemium”. Реализация
бизнес-модели Freemium позволяет нам привлечь большую аудиторию пользователей через
бесплатную версию, а затем предоставить дополнительные возможности через платные
премиум-функции. Это способствует увеличению пользовательской базы, монетизации продукта и обеспечению устойчивого развития бизнеса.
Реализация бизнес-модели для нашего голосового помощника может иметь следующие шаги:

1. Разработка и оптимизация продукта. Продукт – мобильное приложение. Продукт должен быть готов к выводу в магазины приложений, соответствовать требованиям и протоколам, установленным операционными системами iOS и Android.
2. Разработка маркетинговой стратегии. Создание уникального ценностного предложения
продукта для каждой целевой группы. Стратегия будет включать создание лэндинга,
презентаций, демонстрацию продукта, вебинары и семинары с экспертами, рекламные
кампании в социальных сетях и на специализированных платформах.
3. Подача заявки на размещение приложения в магазинах. Подача заявки для включения нашего голосового помощника в магазины приложений, такие как App Store от Apple и Google Play Store, и проходим процесс проверки соблюдения требований платформы по содержанию, политике конфиденциальности и безопасности данных.
4. Размещение приложения в магазинах. Приложение предполагает базовую бесплатную версию с бесплатным периодом пользования и ограниченным функционалом приложения. Далее по истечении бесплатного периода пользователю предлагается приобрести один из вариантов подписки, что обеспечивает монетизацию продукта.
5. Поддержание функционирования приложения, с помощью постоянных обновлений версий приложения и удержание пользователей с помощью сбора обратной связи

### 3.1. Способ оценки пилота

Для оценки пилота используются метрики из пункта 2.3.1, определяется время, на протяжение которого тестируется приложениями.

### 3.2. Что считаем успешным пилотом

По завершению теста принимаем решение.

Успешным проведение пилота считается при удовлетворенности полученными метриками.

В случае успеха пилота переходим к следующей итерации (внедрение системы в сектор B2B и B2G). В случае неуспеха определяем и исправляем ошибки или улучшаем модель и систему, 
либо переходим к другим типам решения или отказываемся от решения.

При любом исходе пилота мы собираем аналитику, новые идеи и гипотезы. А так же сохраняем все результаты.

Для измерения критерия успеха используем окупаемость 
системы. Доходом является покупка платных функций приложения. Затратами являются затраты на разработку и сопровождение. При окупаемости за N месяцев считаем успешным внедрением.

1. Поддержание или увеличение клиентской базы за счет улучшения качества распознавания речи
2. Снижение обращений в техническую поддержку с жалобами на качество предсказания

## 4. Внедрение

### 4.1. Архитектура решения

Архитектура решения.


![image](https://github.com/VorkhlikAS/mainclu/tree/main/docs/design.png)

Флоучарт мобильного приложения

![image](https://github.com/VorkhlikAS/mainclu/tree/main/docs/schema.jpeg)

### 4.2. Описание инфраструктуры и масштабируемости

- Для высокой производительности возможно создание отдельных образов модулей приложения и запуск в кластере kubernetes с регулируемым количеством контейнеров.
- Для хранения пользовательской информации возможно использовать кластерную систему хранения в БД, с подключением новых датанод по мере необходимости

### 4.3. Мониторинг

Мониторинг приложения производится средствами Prometheus+Grafana и осуществляется для отслеживания состояния нагрузки на систему разработчиками. Производится сбор следующих характеристик:

- Загрузка ядер процессора
- Загрузка диска
- Загрузка оперативной памяти
- I/O операции
- Память

### 4.4. Требования к работе системы

- Пропускная способность и задержка обеспечивается структурой и возможностью масштабирования

### 4.5. Безопасность системы

Обеспечивается отсутствием внешних связей и внутренней сетью

### 4.6. Безопасность данных

Безопасность данных обеспечивается 100% хранением на внутренних серверах

### 4.7. Издержки

- Расчетные издержки на работу системы в месяц
- Зарплаты 2 МЛ специалистов на период от 2 - 4 месяцев для создания MVP
- Зарплаты 1 разработчику на период от 2 - 4 месяцев на реализацию MVP
- Затраты на инфраструктуру

### 4.8. Риски

- Риск неверного распознавания специфичного голоса
- Сбой работы модели в результате хакерских атак
- Технический сбой в модели
- Риск незаинтересованности рынка в продукте
