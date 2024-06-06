﻿# Поиск
            
Инструмент кодирования работает путем поиска по мере того, как пользователь продолжает вводить текст в поле поиска: 

![скриншот начала поиска в Инструменте кодирования](img/search-start-v4.png "Начало поиска в Инструменте кодирования")

Инструмент кодирования генерирует (и динамически обновляет) два различных результата по мере продолжения поиска:

![скриншот результатов поиска в Инструменте кодирования](img/search-result-columns-v4.png "Начало поиска в Инструменте кодирования")


1. ## Список слов
        
    В левой части интерфейса Инструмент кодирования показывает список слов.

    Если вы начали набирать слово в сроке поиска, система попытается угадать слово, которое вы набираете.
    
    ![скриншот Инструмент кодирования пытается угадать слово](img/wordlist-guessing.png "Инструмент кодирования пытается угадать слово")


    Если вы закончили набирать слово (это означает, что вы **нажали пробел** в конце слова или **выбрали слово** непосредственно из списка слов), система покажет вам связанные ключевые слова.     
    Связанность рассчитывается с помощью количества раз, когда слова встречаются вместе в МКБ, а также с помощью других подобных критериев.

    ![скриншот связанных слов в Инструменте кодирования](img/wordlist-related.png "Связанные слова в Инструменте кодирования")

    Этот список может быть отсортирован по связанности (по умолчанию) или по алфавиту

    ![скриншот вариантов сортировки списка слов в Инструменте кодирования](img/wordlist-sort.png "Варианты сортировки списка слов в Инструменте кодирования")

    Можно нажать на эти слова вместо того, чтобы продолжать набирать текст.

    <br/>

2. ## Целевые записи
    
    В средней части интерфейса Инструмент кодирования показывает совпавшие записи поиска.
 
    Эти результаты сортируются в соответствии с тем, насколько точно введенный текст совпадает с фразой в МКБ. Совпавшие слова в этом списке результатов выделены (например, слово "туберкулез" на скриншоте ниже).    
    Указатель мыши или клавиатуры (список записей можно прокручивать также клавишами вверх и вниз) отображается красной стрелкой слева от записи и светло-серым фоном.    

    ![скриншот результата поиска записей Инструмента кодирования](img/entities-list-v3.png "Результат поиска записей в Инструменте кодирования")

    В правой части результата поиска записей Инструмент кодирования также показывает небольшие значки, которые предоставляют конкретную информацию о записях, как показано на скриншоте ниже:  


    ![скриншот значка списка записей в Инструменте кодирования](img/entities-list-icons-v4.png "Значок списка записей в Инструменте кодирования")

    Каждый значок имеет свое значение:

    - Посткоординация доступна для этой записи: ![значок «Посткоординация доступна»](img/icon-pa-v4.png "значок «Посткоординация доступна»")
    - Посткоординация обязательна для этой записи: ![значок «Посткоординация обязательна»](img/icon-pr-v4.png "значок «Посткоординация обязательна»")
    - Для этой записи доступно примечание к кодированию: ![значок «Имеется примечание к кодированию»](img/icon-cn-v4.png "значок «Имеется примечание к кодированию»")    
    - Для этой записи существует (существуют) связанная (связанные) рубрика (рубрики) в классе о материнстве: ![значок «Связанные рубрики в классе о материнстве»](img/icon-ml-v4.png "«Связанные рубрики в классе о материнстве»")    
    - Для этой записи существует (существуют) связанная (связанные) рубрика (рубрики) в перинатальном классе: ![ значок «Связанные рубрики в перинатальном классе»](img/icon-pl-v4.png "«Связанные рубрики в перинатальном классе»")    
   
    Если результат поиска содержит "идеальное совпадение", совпавшая запись выделяется синим фоном (как на скриншоте ниже).

    ![скриншот результата полного совпадения в списке записей в Инструменте кодирования](img/entities-list-blu-match-v2.png "Полное совпадение в списке записей в Инструменте кодирования")

    Вы можете изменить порядок сортировки с помощью выпадающего окна в верхней части списка. У нас есть два варианта

      - Сортировка по количеству совпадений (по умолчанию)
      - Сортировка по расположению в классификации

    ![скриншот вариантов сортировки списка записей в Инструменте кодирования](img/entities-list-sort-v4.png "Варианты сортировки списка записей в Инструменте кодирования")

    В списке отображаются только коды и наименования основных терминов, за исключением случаев, когда наименование основного термина не является результатом поиска. Например, на скриншоте ниже выделенный термин является совпавшим термином:

    ![скриншот записи совпавшего термина в Инструменте кодирования](img/entity-matching-terms-v4.png "Запись совпавшего термина в Инструменте кодирования")


    ### Неполные результаты

    Если введенные в поле поиска слова недостаточно точны, и система находит больше результатов, чем может показать, она выдает следующие предупреждения:

    Если найдены результаты более чем в 100 записях, то будут показаны 100 лучших совпадений и предупреждение: *Показаны не все результаты*.

    ![скриншот Инструмента кодирования, когда показаны не все результаты](img/search-result-incomplete-v3.png "Инструмент кодирования, когда показаны не все результаты ") 

    ![скриншот Инструмента кодирования, когда результат поиска слов показан не полностью](img/wordlist-result-incomplete-v3.png "Инструмент кодирования, когда результат поиска слов показан не полностью")

    В этих случаях вам рекомендуется ввести больше информации в поле поиска.


    ### Гибкий поиск

    Функция гибкого поиска может быть использована в случаях, когда обычный поиск в Инструменте кодирования не дает никаких результатов.

    ![скриншот Инструмента кодирования, когда доступен гибкий поиск](img/flexisearch-v2.png "Инструмент кодирования, когда доступен гибкий поиск")

    Способ выполнения поиска в режиме гибкого поиска отличается в следующих аспектах:

    В режиме обычного поиска Инструмент кодирования выдает только результаты, содержащие *все* слова, которые вы использовали при поиске. Он допускает различные варианты или синонимы слов, но в основном он ищет результат, содержащий все компоненты вашего поиска. В то время как в режиме гибкого поиска результаты не обязательно должны содержать все введенные слова. Он все равно попытается найти наиболее подходящую фразу, но в результатах поиска могут быть слова, которые вообще не подходят.
    
    - Например, допустим, пользователь ищет * первичная стеаторея *, а в указателе МКБ-11 нет фразы, содержащей эти слова вместе. Обычный поиск в Инструменте кодирования не даст вам никаких результатов, в то время как гибкий поиск даст вам результаты, содержащие одно из этих слов. Наилучшим результатом в данном случае будет стеаторея, которая является термином в Алфавитном указателе в разделе "Другие уточненные симптомы, связанные с нижними отделами желудочно-кишечного тракта или брюшной полости".    

    <br/>

    ![скриншот результатов гибкого поиска в Инструменте кодирования](img/flexisearch-results-v3.png "Результаты гибкого поиска в Инструменте кодирования")

    Другая дополнительная возможность заключается в том, чтобы использовать также некоторые более широкие варианты слов. Например, если пользователь ищет _Аденосаркома легкого_, он получит _Злокачественные новообразования бронхов или легких, неуточненные_. Для этого вместо фразы "аденосаркома" используется фраза "злокачественное новообразование".


    ### Быстрое копирование

    Нажатие на код (или на наименование основного термина, которое соответствует коду) или нажатие клавиши Enter на клавиатуре копирует выделенный код в буфер обмена. Вы можете в любой момент проверить, какой код скопирован в буфер обмена, в правой верхней части страницы:

    ![скриншот кода записи в Инструменте кодирования, скопированного в буфер обмена](img/entity-clipboard-v3.png "Код записи в Инструменте кодирования, скопированный в буфер обмена")


    ### Дополнительные сведения о записи

    Нажатие на значок «Дополнительные сведения» (или на одну из маленьких иконок), расположенную справа от каждого результата, открывает дополнительные сведения о записи (см. скриншоты ниже):

    ![скриншот значка «Дополнительные сведения» о записи в Инструменте кодирования](img/entity-details-link-v4.png "Значок «Дополнительные сведения» о записи в Инструменте кодирования")

    ![скриншот значка «Дополнительные сведения» о записи в Инструменте кодирования](img/entity-details-open-v4.png "Дополнительные сведения о записи в Инструменте кодирования")

    В верхней части дополнительных сведений о записи, с помощью значка «Показать все», Инструмент кодирования показывает все совпадающие термины для текущей записи.

    ![ скриншот совпадающих терминов в дополнительных сведениях о записи в Инструменте кодирования](img/entity-details-matching-terms-v4.png "Совпадающие термины в дополнительных сведениях о записи в Инструменте кодирования")

    Нажав на значок "скрыть", вы скроете все совпадающие термины, кроме первых пяти.

    ![ скриншот окна со всеми совпадающими терминами в дополнительных сведениях о записи в Инструменте кодирования](img/entity-details-matching-terms-all-v4.png "Все совпадающие термины в дополнительных сведениях о записи в Инструменте кодирования")

3. ## Распределение по классам / фильтр

    С правой стороны интерфейса с помощью кнопки-переключателя Инструмент кодирования показывает распределение записей результатов поиска по классам и позволяет включить фильтр для поиска по классам.

    ![скриншот окна с отключенным фильтром распределения по классам в Инструменте кодирования](img/entities-list-filter-off-v3.png "Фильтр распределения по классам в Инструменте кодирования отключен")

    Распределение по классам показывает количество совпадений, найденных в каждом классе классификации.

    ![скриншот окна с включенным фильтром распределения по классам в Инструменте кодирования](img/entities-list-filter-on-v3.png " Фильтр распределения по классам в Инструменте кодирования включен")

    По умолчанию система осуществляет поиск во всех классах, кроме классов *Коды расширения* и *Традиционная медицина*.
    Фильтр можно изменить, нажав на флажки рядом с названиями классов. Если флажок не установлен, результаты из этого класса не отображаются.

    Нажав на название класса, вы увидите результаты только по этому классу.

    ![скриншот фильтра распределения по классам в Инструменте кодирования](img/chapters-filter.png "Фильтр распределения по классам в Инструменте кодирования")

    Нажав на *Показать результаты из списка по умолчанию*, вы сбросите установленные вами фильтры распределения по классам и получите результаты из всех классов, кроме классов *Коды расширения* и *Традиционная медицина*.

    ![скриншот списка классов по умолчанию в Инструменте кодирования](img/chapters-default.png "Список классов по умолчанию в Инструменте кодирования")

