Использование Geoscan Planner
==============================

Предварительная настройка
-----------------------------------

1) Подключите радиомодем к USB-порту ноутбука.
2) Включите бортовое питание БВС.
3) Запустите программу **MdmDisp**.

В правом нижнем углу появится пиктограмма антенны и количество подключенных бортов.

.. figure:: _static/_images/planner1.png
   :align: center
   :width: 100

   Индикатор работы программы MdmDisp

3.1 При первом подключении необходимо настроить соединение с БВС, запустив программу **NetTopology**:

* Нажмите на значок **Поиск новых устройств**.

.. figure:: _static/_images/planner29.png
   :align: center
   :width: 200

   Значок поиска новых устройств

Программа отобразит список обнаруженных модемов.

.. note:: Эфир сканируется до тех пор, пока кнопка **Поиск новых устройств** не будет нажата повторно.

* Выберите появившийся Борт №xxx и нажать на значок **Добавить устройство**.

.. figure:: _static/_images/planner30.png
   :align: center
   :width: 300

   Значок добавления устройства

Программа сохраняет список добавленных устройств.

При проведении последующих полетов достаточно запустить **MdmDisp** и убедиться, что подключение выполнено успешно.

Если БВС не обнаружено, необходимо переподключить наземный модем, нажав на значок **MdmDisp** правой кнопкой мыши и выбрав **Переподключить**.

.. figure:: _static/_images/planner2.png
   :align: center
   :width: 150

   Контекстное меню MdmDisp

4) Запустите программу **Geoscan Planner**.
5) В окне ввода логина и пароля введите свой логин и пароль пользователя продукта.
6) Во вкладке **Полет** выберите **Подключить БВС - Поиск...**

.. figure:: _static/_images/planner3.png
   :align: center
   :width: 500

   Подключение БВС

7) Выберите тип подключения **MdmDisp**. Задайте **IP-адрес** *localhost*. В списке **Борт** установите для **БВС Порт 6**.

.. figure:: _static/_images/pl4.png
   :align: center
   :width: 500

   Окно подключения БВС

.. note:: Параметры достаточно установить один раз. При последующих подключениях БВС воспользуйтесь кнопкой **Подключить БВС** панели инструментов. Приемник автоматически определит координаты и отобразит местоположение БВС на карте. В окне программы появятся панель телеметрии (слева) и панель приборов (справа).

.. figure:: _static/_images/pl5.png
   :align: center
   :width: 500

   Подключение БВС


Проектирование полетного задания
----------------------------------------

1) Создайте **Новый проект**.

.. figure:: _static/_images/planner5.png
   :align: center
   :width: 400

   Создание нового проекта

Укажите имя проекта, параметры съемки, модель БВС и фотоаппарата.

.. figure:: _static/_images/planner6.png
   :align: center
   :width: 500

   Создание нового проекта полетного задания


Площадная аэрофотосъемка
-------------------------------------------
Площадная аэрофотосъемка – съемка полигонов. Полигон – это оБВСсть, ограниченная многоугольником. Оператор задает вершины многоугольника, а программа автоматически рассчитывает маршрут обхода.

1) Нажмите на значок **Создать площадную аэрофотосъемку** на панели инструментов.

.. figure:: _static/_images/planner8.png
   :align: center
   :width: 500

   Создание площадной аэрофотосъемки

2) Задайте на карте угловые точки исследуемого участка местности. Программа автоматически рассчитает маршрут обхода полигона. При построении маршрута отображаются набор высоты и снижение БВС в виде цилиндров, если разница высот соседних точек превышает 30 метров. Если БВС набирает высоту, то цилиндр залит оранжевым цветом, иначе – синим.

.. figure:: _static/_images/planner9.png
   :align: center
   :width: 500

   Цилиндры набора высоты и снижения

Добавление и удаление вершин полигона
__________________________________________
В готовый полигон можно добавлять вершины. 

С зажатой левой кнопкой мыши переместите среднюю точку стороны полигона. 

.. figure:: _static/_images/planner10.png
   :align: center
   :width: 500

   Добавление вершины

Вершина будет создана автоматически. 
В плавающем окне рядом с вершиной отобразятся ее координаты.

.. figure:: _static/_images/planner34.png
   :align: center
   :width: 500

   Результат добавления вершины


Для удаления вершины:

1) нажмите на вершину правой кнопкой мыши;
2) в контекстном меню выберите **Удалить вершину**.

.. figure:: _static/_images/planner33.png
   :align: center
   :width: 500

   Удаление вершины


Изменение направления линий облета
--------------------------------------
Необходимость оптимизировать полигон «по направлению» возникает, например, если на месте проведения работ сила и направление ветра неБВСгоприятны (сильный ветер вдоль линий облета полигона).
Для изменения типа оптимизации щелкните правой кнопкой мыши на полигоне и выберите в контекстном меню вариант **Оптимизация «направление»**.

.. figure:: _static/_images/planner11.png
   :align: center
   :width: 500

   Оптимизация по направлению

Одна из вершин полигона будет подсвечена, на ней появится поводок для задания направления.

.. figure:: _static/_images/planner12.png
   :align: center
   :width: 500

   Корректировка направления облета

Результатом будет новый маршрут облета полигона по заданному направлению.

.. figure:: _static/_images/planner13.png
   :align: center
   :width: 500

   Новый маршрут облета

Изменение точки входа
--------------------------
Если необходимо сменить точку входа в полигон, то выполните следующие действия:

1) Выделите полигон.

.. figure:: _static/_images/planner14.png
   :align: center
   :width: 500

   Выделенный полигон

2) Правой кнопкой мыши выделите точку, в которой нужно осуществить вход. 
3) В появившемся контекстном меню выберите **Начать здесь**.

.. figure:: _static/_images/planner15.png
   :align: center
   :width: 500

   Изменение точки входа в полигон

.. |flag| image:: _static/_images/flag.png
    :width: 50

У выбранной точки входа появится флажок |flag|



Линейная аэрофотосъемка
---------------------------
Линейная аэрофотосъемка служит для облета линейных протяженных объектов, таких как реки, дороги, линии электропередачи, газо- и нефтепроводы.

1) Нажмите на значок **Создать линейную аэрофотосъемку** на панели инструментов.

.. figure:: _static/_images/planner16.png
   :align: center
   :width: 500

   Создание оБВСсти линейной аэрофотосъемки

2) Однократными щелчками задайте маршрут обхода протяженного объекта по точкам разворотов. Программа автоматически построит линии облета.

.. figure:: _static/_images/planner17.png
   :align: center
   :width: 500

   Пример линейной аэрофотосъемки

Изменение параметров БВС в точках разворота
_______________________________________________
По умолчанию поведение БВС в точках разворота выбирается автоматически с учетом угла между соседними линиями (развороты на углы до заданного угла автопролета осуществляются пролетом).
Для изменения параметров прохождения конкретной вершины щелкните по ней правой кнопкой мыши и выберите нужный параметр разворота.

.. figure:: _static/_images/planner18.png
   :align: center
   :width: 500

   Настройка параметров прохождения вершины

* **Разворот с выходом на ЛЗП** *(линия заданного пути)* означает, что БВС полностью пролетит галс, а затем зайдет на следующий галс с дополнительным маневром («петлей»). Этот вариант гарантирует съемку территории под маршрутом в полном объеме, и он предпочтителен в случае резких разворотов.
* **Разворот пролетом** может с успехом применяться при съемке рек и других естественных объектов, не имеющих выраженных точек разворота. Это более быстрый способ разворота, но он плохо подходит для резких разворотов (крайние части территории под линиями маршрута могут оказаться вне зоны съемки).

Перелет
----------------
Добавление перелетов в полетное задание необходимо, если в зоне полета могут оказаться точечные высотные объекты (опоры ЛЭП, трубы и т.п.). 

1) Нажмите на значок **Создать перелет** на панели инструментов.

.. figure:: _static/_images/planner19.png
   :align: center
   :width: 500

   Создание перелета

2) Однократными щелчками задайте маршрут  перелета. Для построения перелёта на разных высотах, выберите в окне «Свойства» **Режим высоты точек – Нефиксированный**.

.. figure:: _static/_images/planner20.png
   :align: center
   :width: 500

   Свойства перелета

* Функция «Выполнять фотографирование» активирует работу фотоаппарата.

Шаг фотографирования в метрах указывается в соответствующее поле.
Значения в столбце **Превышение** – это разность абсолютной высоты точки ПЗ и рельефа под ней. Таким образом, высота рельефа обязательно учитывается. Абсолютные высоты точек также доступны для редактирования через столбец **Высота**. Кроме этого, высоту можно изменять визуальным редактированием (потянуть мышкой с нажатой клавишей *Shift*).

Маршрут перелёта между двумя полётными элементами строится по следующим правилам:

1) Если у полётных элементов одинаковая высота, то перелёт будет на этой
же высоте.
2) Если у полётных элементов разные высоты, то перелёт будет на наибольшей
из двух высот.

.. attention:: Если условия не позволяют достичь высоты второй точки по прямой (например, небольшое расстояние между точками, но большая разница высот), самолет полетит с максимально допустимым тангажом по прямой до достижения заданной точки по координатам, после чего наберет/сбросит высоту по спирали.

Точка ожидания
------------------------
Команда **Создать точку ожидания** служит для того, чтобы БВС  удерживало точку на высоте в течение отрезка времени. Позволяет измерять направление и силу ветра на высоте.

1) Нажмите на значок **Создать точку ожидания** на панели инструментов.

.. figure:: _static/_images/planner22.png
   :align: center
   :width: 500

   Создание точки ожидания

2) Щелчком мыши на карте задайте точку, в которой должно осуществляться ожидание.

В экспертном режиме можно изменить свойства: задать высоту точки ожидания, длительность ожидания, направление движения и активировать функции измерения ветра и бесконечного ожидания.

.. figure:: _static/_images/planner23.png
   :align: center
   :width: 500

   Свойства точки ожидания

Планер будет на заданной высоте «удерживать» точку в течение указанного времени (по умолчанию 300 секунд), после чего отправится по запланированному маршруту.

При активации варианта «Измерение ветра» длительность автоматически выставляется в значение 0. При этом точка ожидания окрасится в желтый цвет. Самолет выполняет полный оборот с постоянным измерением ветра.

.. figure:: _static/_images/planner24.png
   :align: center
   :width: 500

   Точка измерения ветра

Функция бесконечного ожидания служит для постоянного удержания точки (пока не сработает отказ по низкому заряду АКБ, приводящий к автоматическому возврату). При этом цвет точки ожидания сменяется на темно-синий.

.. figure:: _static/_images/planner25.png
   :align: center
   :width: 500

   Точка бесконечного ожидания

.. attention:: Рекомендуется устанавливать точку ожидания с измерением ветра перед каждым полетным элементом на высоте полётного элемента. Автопилот, учитывая измеренные данные о ветре, будет плавнее идти по маршруту.
.. attention:: Комплексы Геоскан не являются сертифицированными приборами измерения ветра, поэтому не могут быть использованы в качестве надежных источников данных о состоянии окружающей среды.

Маршрут посадки
--------------------------------
Команда **Создать посадку** служит для построения маршрута посадки.

Это обязательное действие при построении полетного задания.

На месте проведения полета определите направление ветра, скорректируйте при необходимости зону полета и выберите место посадки.
Для посадки следует выбирать открытое сухое пространство без деревьев и прочих препятствий.
Площадка для посадки должна быть ровной, желательно с травяным покровом.

1) Нажмите на значок **Создать посадку** на панели инструментов.

.. figure:: _static/_images/planner31.png
   :align: center
   :width: 500

   Создание посадки

2) Щелчком клавиши мыши выберите сначала точку посадки, затем точку захода на посадку.

Программа автоматически создаст маршрут посадки из трех точек (промежуточная точка создается автоматически).

.. figure:: _static/_images/planner32.png
   :align: center
   :width: 500

   Пример посадки

.. attention:: Важно, чтобы посадка осуществлялась против ветра в оБВСсти посадки. В противном случае возможна жесткая посадка, приводящая к повреждениям самолета.


Предстартовая подготовка
----------------------------

1) Запустите **Мастер предстартовой подготовки**.

.. figure:: _static/_images/planner26.png
   :align: center
   :width: 300

   Запуск мастера предстартовой подготовки

Следуйте указаниям мастера предстартовой подготовки (большинство проверок выполняются автоматически).
Задайте радиус автоматического отцепа парашюта и время автономного полёта (время, в течение которого осуществляется полёт независимо от наличия связи между НСУ и БВС).
После прохождения предстартовой подготовки установите БВС на пусковую установку.

Полет
----------------------------

1) Нажмите на значок **Старт**.

.. figure:: _static/_images/planner27.png
   :align: center
   :width: 300

   Перевод БВС в стартовый режим

БВС перейдет в стартовый режим. 
На панели телеметрии отобразится режим **КАТАПУЛЬТА**.


.. figure:: _static/_images/planner28.png
   :align: center
   :width: 400

   Режим КАТАПУЛЬТА

.. attention:: Переводить БВС в стартовый режим необходимо после установки на пусковую установку. После перехода в стартовый режим запрещается брать в руки и переносить БВС.

.. attention:: Чтобы отменить переход в режим Катапульта, нажмите кнопку **Возврат**. БВС перейдет в режим Подготовка. Мастер предстартовой подготовки необходимо будет пройти заново.

2) Снимите предохранитель и активируйте пусковую установку, потянув за спусковой шнур. 

БВС осуществит взлёт.

.. note:: Подробнее о предстартовой последовательности - в разделе `запуск`_.

.. _`запуск`: launch.html


Действия при отказах
----------------------

При возникновении отказа на панели телеметрии в графе Отказы отобразится сообщение о типе ошибки. Ниже представлена таблица возможных сообщений панели и действия по устранению проблем.


.. csv-table:: 
   :header: "Отказ", "Описание", "Действия"
   :widths: 7, 15, 20

    "АВАРИЯ", "Критическая температура платы регулятора или мотора", "Осуществите немедленную посадку. Свяжитесь со службой поддержки"
    "ЗАПУСКИ ПОТРАЧЕНЫ", "Количество предусмотренных лицензией запусков истекло", "Обновите лицензию. Свяжитесь со службой поддержки "
    "ЗОНЫ ИСТЕКЛИ", "Срок действия полетных зон истек ", "Подключитесь к интернету для обновления файла зон. Свяжитесь со службой поддержки "
    "ЗОНЫ НЕ ВЕРИФИЦИРОВАНЫ ", "Проверка полетных зон завершилась неудачей", "Подключитесь к интернету для обновления файла зон. Свяжитесь со службой поддержки "
    "К ВЗЛЕТУ НЕ ГОТОВ ", "После прохождения предстартовой подготовки автопилота не готов осуществить взлет", "Перепройдите предстартовую подготовку. Свяжитесь со службой поддержки "
    "ЛИЦЕНЗИЯ ИСТЕКЛА ", "Закончился срок использования лицензии", "Обновите лицензию. Свяжитесь со службой поддержки "
    "НАРУШЕНИЕ ЗОНЫ ", "Текущие координаты БВС не попадают в разрешенную полетную зону", "Происходит отключение фотокамеры, БВС выполняет полет к месту посадки "
    "НЕ ГОТОВ ", "БВС не готов к переходу в другое состояние", "Дождитесь инициализации автопилота "
    "НЕВЕРНАЯ ЛИЦЕНЗИЯ ", "Лицензия была дистанционно отключена", "Свяжитесь со службой поддержки "
    "НЕВЕРНЫЕ ЗОНЫ ", "Несовпадение номера группы зон лицензии с фактическим номером группы зон", "Подключитесь к интернету для обновления файла зон. Свяжитесь со службой поддержки "
    "НЕТ ЗОН ", "Отсутствие загруженных полетных зон", "Подключитесь к интернету для обновления файла зон. Свяжитесь со службой поддержки "
    "НЕТ ДВИГ ", "Отсутствует связь с двигателем", "Свяжитесь со службой поддержки "
    "НЕТ СИНХР ВРЕМЕНИ ", "Отсутствует синхронизация внутреннего времени автопилота со временем от спутникового приемника", "Дождитесь синхронизации "
    "ОШИБКА АКСЕЛ ", "Ошибка системы ориентации БВС, не приходят данные с акселерометра", "Свяжитесь со службой поддержки "
    "ОШИБКА БАРО ", "Ошибка датчика измерения высоты, не приходят данные с барометра", "Свяжитесь со службой поддержки "
    "ОШИБКА ГНСС ", "Ошибка приемника спутниковой навигации", "Перевключите БВС "
    "ОШИБКА ГИРОСКОПА ", "Ошибка системы ориентации БВС, не приходят данные с гироскопа", "Свяжитесь со службой поддержки "
    "ОШИБКА EEPROM ", "Ошибка чтения или записи энергонезависимой памяти", "Свяжитесь со службой поддержки "
    "ОШИБКА КАРТЫ ", "Ошибка внешнего постоянного хранилища данных: не удалось инициализировать внешнюю карту памяти", "Проверьте карту памяти "
    "ОШИБКА КОМПАСА ", "Ошибка датчика определения направления, не приходят данные с магнитометра", "Осуществите немедленную посадку "
    "ОШИБКА КРЛ ", "Ошибка канала связи: автопилот в течение длительного времени не получал сообщений от наземной станции управления", "Проверьте бортовой модем после возвращения борта "
    "ОШИБКА ЛИЦЕНЗИИ ", "Ошибка проверки лицензии на полет", "Попробуйте перезагрузить файл лицензии. Свяжитесь со службой поддержки "
    "ОШИБКА ЛОГГЕРА ", "Ошибка записи полетного лога", "Проверьте карту памяти автопилота "
    "ОШИБКА НАСТРОЙКИ ", "Ошибка в параметрах автопилота", "Свяжитесь со службой поддержки " 
    "ОШИБКА ПЗ ", "Ошибка выполнения загруженного полетного задания", "Попробуйте обновить полетное задание. Свяжитесь со службой поддержки "
    "ОШИБКА ПИТАНИЯ ", "Ошибка питания автопилота", "Перевключите БВС "
    "ОШИБКА ФОТО ", "Произошла ошибка фотографирования", "Перевключите фотокамеру/проверьте флеш-карту фотокамеры "
    "ПЕРЕЗАГРУЗКА ", "Произошла внеплановая перезагрузка автопилота", "Свяжитесь со службой поддержки "
    "ФОТО: НЕТ КАРТЫ ", "Отсутствует карта памяти", "Вставьте карту в фотокамеру "
    "ФОТО: ОШИБКА КАРТЫ ", "Ошибка чтения/записи карты памяти", "Снимите защиту карты от записи "
    "ФОТО: ОШИБКА ПИТ ", "Напряжение питания фотоаппарата слишком высокое", "Перевключите БВС "
    "ФОТО: НИЗКОЕ НАПРЯЖЕНИЕ ", "Напряжение питания фотоаппарата слишком низкое", "Перевключите БВС "
    "ФОТО: ОШИБКА СИНХ ", "Потеря сигнала синхронизации времени", "Перевключите БВС "
    "ФОТО: ТЕМПЕРАТУРА ", "Фотокамера перегрета или переохлаждена", "Поместите фотокамеру в условия комнатной температуры "



Если предложенный вариант действий при отказе не помогает исправить ситуацию, незамедлительно свяжитесь со службой поддержки.

