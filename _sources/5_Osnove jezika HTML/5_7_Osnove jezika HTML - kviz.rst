Основе језика HTML - квиз
=========================

.. quizq::

    .. mchoice:: osnove_jezika_html_kviz_1
        :answer_a: боја насловног текста
        :answer_b: позиција елемента на страници
        :answer_c: табела са подацима
        :answer_d: размак између елемената
        :answer_e: галерија слика
        :correct: c, e

        Одабери елементе који описују логичку структуру веб-странице.

.. quizq::

    .. mchoice:: osnove_jezika_html_kviz_2
        :answer_a: ширина ивице табеле
        :answer_b: боја позадине
        :answer_c: везе у навигацији највишег нивоа
        :answer_d: дугме за сакривање садржаја
        :answer_e: величина слова у тексту
        :correct:  a, b, e

        Одабери елементе који описују визуелну презентацију веб-странице.

.. quizq::

    .. fillintheblank:: osnove_jezika_html_kviz_3

        Допиши затварајућу етикету HTML елемента *p* тако да се добије исправан HTML код.

        Одговор: <p> |blank| 

        - :^</p\s*>$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: osnove_jezika_html_kviz_4

        Напиши самозатварајућу етикету за HTML елемент *img*.

        Одговор: |blank| 

        - :^<img\s*(/)?>$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::
    
    .. dragndrop:: osnove_jezika_html_kviz_5
        :match_1:  < ||| &‎lt;
        :match_2:  > ||| &‎gt;
        :match_3:  & ||| &‎amp;
        :match_4:  " ||| &‎quot;
        
        Повежи специјалне карактере и HTML секвенце којима они одговарају.

.. quizq::

    .. fillintheblank:: osnove_jezika_html_kviz_6

        Посматрај наредни део HTML кода.

        .. code-block:: html

                <body>
                    <h1>Здраво, свете!</h1>
                    <p>Ово је једноставан параграф.</p>
                    <ul>
                        <li>Ставка 1</li>
                        <li>Ставка 2</li>
                    </ul>
                </body>


        Колико чворова које представљају HTML елементе има DOM стабло које одговара приказаном коду?

        Одговор: |blank|

        - :^6$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    Посматрај DOM стабло на наредној слици и HTML код који је дат у наставку, па одговори на питање.

    .. image:: ../../_images/osnove_jezika_html_kviz_7.png
        :width: 400
        :align: center

    .. code-block:: html 

        <body>
            <h1>Здраво!</h1>
            <div>
                <h2>Петља квиз</h2>
                <img>
            </div>
        </body>

    .. mchoice:: osnove_jezika_html_kviz_7
        :answer_a: да
        :answer_b: не
        :correct: b 

        Да ли DOM стабло приказано на слици одговара датом HTML коду?

.. quizq::

    Посматрај DOM стабло на наредној слици и HTML код који је дат у наставку, па одговори на питање.

    .. image:: ../../_images/osnove_jezika_html_kviz_8.png
        :width: 400
        :align: center

    .. code-block:: html 

        <body>
            <h1>Здраво!</h1>
            <div>
                <h2>Петља квиз</h2>
                <img>
            </div>
        </body>

    .. mchoice:: osnove_jezika_html_kviz_8
        :answer_a: да
        :answer_b: не
        :correct: a

        Да ли DOM стабло приказано на слици одговара датом HTML коду?

.. quizq::

    Посматрај пример садржаја веб-странице са четири елемента на наредној слици, па одговори на питање.

    .. image:: ../../_images/osnove_jezika_html_kviz_9.png
        :width: 600
        :align: center

    .. mchoice:: osnove_jezika_html_kviz_9
        :answer_a: блоковским
        :answer_b: линијским
        :answer_c: ниједно од понуђених
        :correct: a

        Којој категорији HTML елемената припадају елементи означени бројевима 1 и 4?

.. quizq::

    .. fillintheblank:: osnove_jezika_html_kviz_10

        Допуни наредни део HTML кода тако да се HTML елемент *ul* јединствено препозна вредношћу *lista* на нивоу веб-странице.

        | <ul |blank| ="lista">
        |    <li>Ставка 1</li>
        |    <li>Ставка 2</li>
        | </ul> 

        - :^id$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: osnove_jezika_html_kviz_11

        Допуни наредни део HTML кода тако да се HTML елементи *li* функционално групишу у категорију *stavka-liste* на нивоу веб-странице.

        | <ul>
        |    <li |blank| ="stavka-liste">Ставка 1</li>
        |    <li |blank| ="stavka-liste">Ставка 2</li>
        | </ul> 

        - :^class$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^class$: Други одговор је тачан.
          :x: Други одговор није тачан.
