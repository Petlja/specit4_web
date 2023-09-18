Основна својства садржаја - квиз
================================

.. quizq::

    Посматрај наредну слику, па одговори на питање.

    .. image:: ../../_images/osnovna_svojstva_sadrzaja_kviz_1.png
        :width: 400
        :align: center

    .. mchoice:: osnovna_svojstva_sadrzaja_kviz_1
        :answer_a: text-color
        :answer_b: background-color
        :answer_c: color
        :answer_d: font-color
        :answer_e: backdrop-color
        :correct: c

        Које од наредних CSS својстава се користи тако да се постави љубичаста боја као на датој слици?

.. quizq::

    Посматрај наредну слику, па одговори на питање.

    .. image:: ../../_images/osnovna_svojstva_sadrzaja_kviz_2.png
        :width: 400
        :align: center

    .. mchoice:: osnovna_svojstva_sadrzaja_kviz_2
        :answer_a: text-color
        :answer_b: background-color
        :answer_c: color
        :answer_d: font-color
        :answer_e: backdrop-color
        :correct: b

        Које од наредних CSS својстава се користи тако да се постави љубичаста боја као на датој слици?

.. quizq::

    .. fillintheblank:: osnovna_svojstva_sadrzaja_kviz_3

        Допуни наредни CSS код тако да се одговарајућом CSS функцијом примени боја која има наредне уделе светлости (из инзервала 0-255) и прозирност од 30%:
            - удео плаве светлости: 12
            - удео зелене светлости: 34
            - удео црвене светлости: 56

        | selektor {
        |   color: |blank| (|blank|, |blank|, |blank|, |blank|);
        | }

        - :^rgba$: Први одговор је тачан
          :x: Први одговор није тачан
        - :^56$: Други одговор је тачан
          :x: Други одговор није тачан
        - :^34$: Трећи одговор је тачан
          :x: Трећи одговор није тачан
        - :^12$: Четврти одговор је тачан
          :x: Четврти одговор није тачан
        - :^0.50*$: Пети одговор је тачан
          :x: Пети одговор није тачан

.. quizq::

    .. dragndrop:: osnovna_svojstva_sadrzaja_kviz_4
        :match_1: font-size ||| величина слова
        :match_2: font-style ||| искошеност слова
        :match_3: font-weight ||| подебљање слова
        :match_4: text-align ||| хоризонтално поравнање текста
        :match_5: text-transform ||| трансформација слова

        Повежи CSS својства са визуелним карактеристикама на које се односе.

.. quizq::

    .. dragndrop:: osnovna_svojstva_sadrzaja_kviz_5
        :match_1: serif ||| кукичаве фамилије фонтова
        :match_2: sans-serif ||| бескукичаве фамилије фонтова
        :match_3: monospace ||| фамилије фонтова карактера једнаких ширина
        :match_4: cursive ||| писане фамилије фонтова 
        :match_5: fantasy ||| декоративне фамилије фонтова

        Повежи називе фамилије фонтова и њихова значења.


.. quizq::

    Посматрај наредни део CSS кода, па одговори на питање.

    .. code-block:: css

        p {
            font-family: Fira Mono, Console, monospace;
        }

    .. parsonsprob:: osnovna_svojstva_sadrzaja_kviz_6

        Поређај фамилије фонтова од оне са најмањим до оне са највећим приоритетом приказивања текста од стране веб-прегледача.
        -----
        monospace
        Console
        Fira Mono
