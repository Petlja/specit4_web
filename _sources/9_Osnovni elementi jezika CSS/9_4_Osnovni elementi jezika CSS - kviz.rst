Основни елементи језика CSS - квиз
==================================

.. quizq:: 

    .. fillintheblank:: osnovni_elementi_jezika_css_kviz_1

        Допуни наредни CSS код тако да се написаним правилом примени својство *visina* са вредношћу *15cm*.

        | moj-element {
        |   |blank| : |blank| ;
        | }

        - :^visina$: Први одговор је тачан
          :x: Први одговор није тачан
        - :^15cm$: Други одговор је тачан
          :x: Други одговор није тачан

.. quizq:: 

    
    .. mchoice:: osnovni_elementi_jezika_css_kviz_2
        :answer_a: да 
        :answer_b: не
        :correct: a

        Да ли се једно CSS правило може састојати од више CSS декларација?

.. quizq:: 

    
    .. parsonsprob:: osnovni_elementi_jezika_css_kviz_3

        Поређај следеће начине за задавање правила за стилизовање од најопштијег до најспецифичнијег.
        -----
        Елемент *link*
        Елемент *style+
        Атрибут *style*

.. quizq:: 

    
    .. fillintheblank:: osnovni_elementi_jezika_css_kviz_4

        Допуни наредни код тако да се на датој веб-страници увезу правила за стилизовање из датотеке *dizajn.css*. Препостави да се датотека налази у истом директоријуму као и HTML датотека која садржи наредни код.

        | <link type="|blank|" href="|blank|" rel="|blank|" >

        - :^text/css$: Први одговор је тачан
          :x: Први одговор није тачан
        - :^(\./)?dizajn\.css$: Други одговор је тачан
          :x: Други одговор није тачан
        - :^stylesheet$: Трећи одговор је тачан
          :x: Трећи одговор није тачан

.. quizq:: 

    
    .. mchoice:: osnovni_elementi_jezika_css_kviz_5
        :answer_a: да 
        :answer_b: не
        :correct: b

        Да ли је наредно тврђење тачно: Цурење стилова се може спречити коришћењем елемента *link* за задавање правила за стилизовање у комбинацији са дељеним CSS датотекама?

.. quizq:: 

    
    .. fillintheblank:: osnovni_elementi_jezika_css_kviz_6

        Допуни наредни код тако да се дато CSS правило примени на елемент чији је идентификатор *lista*.

        | |blank| {
        |   color: black;
        | }

        - :^#lista$: Одговор је тачан
          :x: Одговор није тачан

.. quizq:: 

    
    .. fillintheblank:: osnovni_elementi_jezika_css_kviz_7

        Допуни наредни код тако да се дато CSS правило примени на све елементе који припадају класи *lista*.

        | |blank| {
        |   color: black;
        | }

        - :^\.lista$: Одговор је тачан
          :x: Одговор није тачан

.. quizq:: 

    
    .. fillintheblank:: osnovni_elementi_jezika_css_kviz_8

        Посматрај DOM стабло са наредне слике, па одговори на питање.

        .. image:: ../../_images/osnovni_elementi_jezika_css_kviz_8.png
            :width: 400
            :align: center

        Допуни наредни код тако да се дато CSS правило примени само на означене елементе *img*.

        | |blank| {
        |   color: black;
        | }

        - :^div\s+img$: Одговор је тачан
          :x: Одговор није тачан