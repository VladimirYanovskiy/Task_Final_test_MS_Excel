# ЗАДАНИЕ
# Зачет. Анализ данных системы проката велосипедов

Описание проекта

Задание: с помощью инструментов Excel провести анализ данных (включая применения функций, обработку данных, фильтрацию и визуализацию данных) системы проката велосипедов и визуализировать его результаты.

Файл с данными: day_24.csv

Порядок выполнения: 
 1. Проанализировать кейс day_24.csv;
 2. Провести предобработку данных;
 3. Вывести описательную статистику;
 4. Сформулировать и проверить гипотезу;
 5. Сделать возможные выводы (отсутствие связи, наличие выбросов, несоответствие распределения закону и т.п. — это тоже вывод);
 6. Визуализировать свои рассуждения. Можно использовать приведенные ниже шаблоны презентаций;
 7. Подготовить отчет.

Требования к оформлению: 

Выполненное задание оформить в виде:
  -	файла презентации в формате *.pdf. Файл следует назвать "Презентация_, фамилия, инициалы". Например: "Презентация_Иванов АВ";
  -	файл с вычислениями в формате *.xlsx  Файл следует назвать "Аналитический отчет_, фамилия, инициалы". Например: "Аналитический отчет_Иванов АВ".

Информация о наборе данных для совместного использования велосипедов

Обзор

Системы проката велосипедов — это новое поколение традиционных прокатов велосипедов, в которых весь процесс от членства, аренды и возврата стал автоматическим. С помощью этих систем пользователь может арендовать велосипед в определенном месте и вернуться обратно в другом месте. Сегодня существует большой интерес к этим системам из-за их важной роли в вопросах дорожного движения, окружающей среды и здоровья.  В настоящее время в мире существует около 500 программ велопроката, в которых задействовано более 500 тысяч велосипедов. 

Помимо интересных реальных приложений систем проката велосипедов, характеристики данных, генерируемых этими системами, делают их привлекательными для исследований. В отличие от других транспортных услуг, таких как автобус или метро, ​​в этих системах четко записывается продолжительность поездки, место отправления и прибытия. Эта функция превращает систему проката велосипедов в виртуальную сенсорную сеть, которую можно использовать для определения мобильности жителей в городе. Следовательно, ожидается, что большинство важных тенденций в жизни города можно будет обнаружить с помощью мониторинга этих данных.

Информация об атрибутах

day_24.csv имеет следующие поля:

   instant: Индекс записи
    dteday: Дата;
    season: Сезон (1:весна, 2:лето, 3:осень, 4:зима);
    yr: Год (0: 2011, 1: 2012);
    mnth: Месяц (от 1 до 12);
    holiday: Праздничный день (день праздничный или нет);
    weekday: День недели (от 0 до 6);
    workingday: Рабочий день - если день не является ни выходным, ни праздничным днем, равен 1, иначе равен 0.

погода:

    1: Ясно, небольшая облачность, переменная облачность, переменная облачность;
    2: Туман + Облачно, Туман + Разорванные облака, Туман + Немного облаков, Туман;
    3: Слабый снег, Слабый дождь + Гроза + Рассеянные облака, Слабый дождь + Рассеянные облака;
    4: Сильный дождь + ледяные поддоны + гроза + туман, снег + туман;
    temp: Нормализованная температура в градусах Цельсия. Значения получены через (t-t_min)/(t_max-t_min), t_min=-8, t_max=+39;
    atemp: Нормализованная температура ощущения в градусах Цельсия. Значения получены через (t-t_min)/(t_max-t_min), t_min=-16, t_max=+50;
    hum: Нормализованная влажность. Значения делятся на 100 (макс.);
    windspeed: Нормализованная скорость ветра. Значения делятся на 67 (макс.);
    casual: Количество случайных пользователей;
    registered: Количество зарегистрированных пользователей;
    cnt: Общее количество арендованных велосипедов, включая обычные и зарегистрированные.
