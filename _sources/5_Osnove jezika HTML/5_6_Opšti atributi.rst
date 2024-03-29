Општи атрибути
==============

Иако велики број HTML елемената има атрибуте који ближе одређују понашање тих атрибута, постоје неки атрибути који су применљиви на све HTML елементе. Ови атрибути су општег карактера, а неки од њих се најчешће примењују заједно са језиком CSS како би се прецизно дефинисала правила за стилизовање елемената или са језиком *JavaScript* како би се једноставније приступило из кода елементима којима се придружује одговарајуће динамичко понашање.

Неки од општих атрибута су:

- Атрибут `class` се користи за функционално груписање елемента у категорије (кажемо још и класе). Када се неко правило језика CSS или неко динамичко понашање придружи некој класи, онда се то правило (односно, то динамичко понашање) придружује свим елементима који имају постављену вредност овог атрибута на дату класу. Да би се ово понашање омогућило, једна класа се може доделити произвољном броју елемената. Такође, један елемент може имати више класа. Наредна табела илуструје додељивање класа елементима:

+-------------------------------------+----------------------------------------------------------+
| Пример кода                         | Објашњење                                                |
+=====================================+==========================================================+
| <element class=”obavestenje”>       | Елементу се додељује класа „obavestenje“.                |
+-------------------------------------+----------------------------------------------------------+
| <element class=”vazno obavestenje”> | Елементу се додељују две класе: „vazno“ и „obavestenje“. |
+-------------------------------------+----------------------------------------------------------+

- Атрибут `id` се користи за функционално препознавање елемента на основу идентификатора. За разлику од атрибута class, вредност овог атрибута се у оквиру једног документа може применити највише на једном елементу. Понављање идентификатора резултује недефинисаним понашањем и веома је важно избегавати ову ситуацију јер води ка непожељним резултатима.
- Атрибут `style` служи за постављање визуелних правила језика CSS која ће бити примењена искључиво над садржајем елемента (уместо на нивоу целог документа).
- Атрибут `title` служи за навођење додатних информација о елементу. Веб-прегледачи најчешће приказују ове информације и виду информационе поруке (*tooltip*) приликом постављања курсора миша на елемент.
- Већ поменути атрибут `lang` није применљив само на елемент `html`, већ се може користити за подешавање језика садржаја на нивоу било ког HTML елемента.

Правила за именовање класа и идентификатора су следећа:

- Име може садржати мала и велика слова енглеског алфабета (a-z, A-Z), цифре (0-9), цртице (-) и подвлаке (_).
- Име мора почињати карактером слова.

Иако ове атрибуте нећемо много користити у овом делу, важно је да разумеш њихове карактеристике зарад лакшег усвајања градива надаље.
