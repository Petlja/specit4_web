Позиционирање садржаја - квиз
=============================

.. quizq::

    .. dragndrop:: pozicioniranje_sadrzaja_kviz_1
        :match_1: top    ||| померање на доле
        :match_2: right  ||| померање у лево
        :match_3: bottom ||| померање на горе
        :match_4: left   ||| померање у десно

        Повежи наредна CSS својства за померање елемената и њихова значења у односу на смер у којем врше померање елемената.

.. quizq::

    .. mchoice:: pozicioniranje_sadrzaja_kviz_2
        :answer_a: фиксно
        :answer_b: релативно
        :answer_c: апсолутно
        :answer_d: статичко
        :answer_e: ниједно од понуђених
        :correct: d

        Која од наредних врста позиционирања представља подразумевани тип позиционирања елемената?


.. quizq::

    .. fillintheblank:: pozicioniranje_sadrzaja_kviz_3

        Које CSS својство се мора навести како би CSS својства за померање елемената (*top*, *bottom*, *right*, *left*) имала утицај на позиционирање елемената?

        Одговор: |blank|

        - :^position$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: pozicioniranje_sadrzaja_kviz_4

        Допуни наредни CSS код тако да се елемент *p* позиционира 30 пиксела од горње ивице у односу на његово подразумевано позиционирање.

        | p {
        |   |blank|: 30px;
        |   |blank|: |blank| ;
        | }

        - :^top$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^position$: Други одговор је тачан.
          :x: Други одговор није тачан.
        - :^relative$: Трећи одговор је тачан.
          :x: Трећи одговор није тачан.

.. quizq::

    .. fillintheblank:: pozicioniranje_sadrzaja_kviz_5

        Допуни наредни CSS код тако да се елемент *p* позиционира 20 пиксела од десне ивице погледа веб-прегледача.

        | p {
        |   |blank|: 20px;
        |   |blank|: |blank| ;
        | }

        - :^right$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^position$: Други одговор је тачан.
          :x: Други одговор није тачан.
        - :^fixed$: Трећи одговор је тачан.
          :x: Трећи одговор није тачан.

.. quizq::

    Посматрај наредне делове HTML и CSS кодова, па одговори на питање.

    .. code-block:: HTML

        <!-- HTML код -->
        <body>
            <header>
                <nav>
                    <span>
                        <a></a>
                    </span>
                </nav>
            </header>
        </body>

    .. code-block:: CSS

        /* CSS код */
        a {
            position: absolute;
            left: 10px;
        }

    .. mchoice:: pozicioniranje_sadrzaja_kviz_6
        :answer_a: header
        :answer_b: nav
        :answer_c: span
        :answer_d: ниједно од понуђених
        :correct: d

        У односу на ивицу којег од понуђених елемената ће елемент *a* бити позициониран?

.. quizq::

    Посматрај наредне делове HTML и CSS кодова, па одговори на питање.

    .. code-block:: HTML

        <!-- HTML код -->
        <body>
            <header>
                <nav>
                    <span>
                        <a></a>
                    </span>
                </nav>
            </header>
        </body>

    .. code-block:: CSS

        /* CSS код */
        header {
            position: relative;
        }

        nav {
            position: relative;
        }

        a {
            position: absolute;
            left: 10px;
        }

    .. mchoice:: pozicioniranje_sadrzaja_kviz_7
        :answer_a: header
        :answer_b: nav
        :answer_c: span
        :answer_d: ниједно од понуђених
        :correct: b

        У односу на ивицу којег од понуђених елемената ће елемент *a* бити позициониран?

.. quizq::

    Посматрај наредну слику, па одговори на питање.

    .. image:: ../../_images/pozicioniranje_sadrzaja_kviz_8.png
        :width: 600
        :align: center

    .. parsonsprob:: pozicioniranje_sadrzaja_kviz_8

        Поређај елементе од оног са највећом до оног са најмањом вредношћу CSS својства *z-index*.
        -----
        зелени
        плави
        црвени
        жути

.. quizq::

    Посматрај наредну слику, па одговори на питање.

    .. image:: ../../_images/pozicioniranje_sadrzaja_kviz_9.png
        :width: 600
        :align: center

    .. mchoice:: pozicioniranje_sadrzaja_kviz_9
        :answer_a: visibility
        :answer_b: remove
        :answer_c: display
        :answer_d: delete
        :answer_e: ниједно од понуђених
        :correct: a
        
        Које од наредних CSS својстава се може користити да се плави елемент на слике уклони из приказа веб-странице тако да остали елементи не мењају свој распоред?