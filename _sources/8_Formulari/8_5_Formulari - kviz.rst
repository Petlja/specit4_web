Формулари - квиз
================

.. quizq::

    .. mchoice:: formulari_kviz_1
        :answer_a: input
        :answer_b: textarea
        :answer_c: form
        :answer_d: email
        :correct: a

        Који од наредних HTML елемената је најпогоднији избор за поље у којем корисник уноси адресу електронске поште?

.. quizq:: 

    .. dragndrop:: formulari_kviz_2
        :match_1: radio    ||| ексклузивно дугме
        :match_2: checkbox ||| неексклузивно дугме
        :match_3: date     ||| поље за одабир датума
        :match_4: password ||| поље за унос лозинке
        :match_5: submit   ||| дугме за подношење формулара

        Повежи HTML елементе и делове формулара које они описују.

.. quizq::

    Посматрај HTML код који је дат у наставку, па одговори на питање.

    .. code-block:: html 

        <form>
            Какве напитке највише волиш?
            <br>
            
            <input type="radio" value="vruce">
            <label> вруће
            <br>
            
            <input type="radio" value="hladne">
            <label> хладне
        </form>

    .. mchoice:: formulari_kviz_3
        :answer_a: да
        :answer_b: не
        :correct: b 

        Да ли је наредно тврђење тачно: Корисник може да одабере највише једну од опција дугмићима са ознакама "вруће" и ”хладно”?

.. quizq:: 

    .. dragndrop:: formulari_kviz_4
        :match_1: textarea ||| Вишелинијско текстуално поље
        :match_2: button   ||| Обично дугме
        :match_3: select   ||| Падајућа листа
        :match_4: fieldset ||| Елемент са груписање поља
        :match_5: legend   ||| Опис групе

        Повежи HTML елементе и делове формулара које они описују.

.. quizq::

    .. fillintheblank:: formulari_kviz_5

        Допуни наредни HTML код тако да се формулар поднесе на страницу *anketa.html*.

        | <form |blank| ="|blank|">
        |     <input type="text" name="ime">
        |     <br>
        |     <input type="submit" value="Поднеси формулар">
        | </form>

        - :^action$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^anketa\.html$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. fillintheblank:: formulari_kviz_6

        Допуни наредни HTML код тако да се подаци из формулара поднесу на страницу кроз тело HTTP захтева.

        | <form |blank| ="|blank|">
        |     <input type="text" name="ime">
        |     <br>
        |     <input type="submit" value="Поднеси формулар">
        | </form>

        - :^method$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^(post)|(POST)$: Други одговор је тачан.
          :x: Други одговор није тачан.
