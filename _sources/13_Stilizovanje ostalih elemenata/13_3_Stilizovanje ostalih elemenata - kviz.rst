Стилизовање осталих елемената - квиз
====================================

.. quizq:: 

    .. dragndrop:: stilizovanje_ostalih_elemenata_1
        :match_1: decimal ||| 1, 2, 3, ...
        :match_2: upper-roman ||| I, II, III, ...
        :match_3: lower-greek ||| α, β, γ, ...
        :match_4: upper-alpha ||| A, B, C, ...

        Повежи вредности CSS својства *list-style-type* и одговарајућа набрајања.

.. quizq::

    .. fillintheblank:: stilizovanje_ostalih_elemenata_2

        Допуни наредни CSS код тако да се ивице елемената *td* у табели приказују спојено.

        | td {
        |   border: 1px solid black;
        | }
        |
        | table {
        |   |blank|: |blank| ;
        | }

        - :^border-collapse$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^collapse$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. mchoice:: stilizovanje_ostalih_elemenata_3
        :answer_a: caption-position: bottom
        :answer_b: caption-side: bottom
        :answer_c: caption: bottom
        :answer_d: ниједно од понуђених
        :correct: b 

        Која од наредних декларација се може искористити за приказивање наслова табеле испод табеле?