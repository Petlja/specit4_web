16.9 Библиотека Flask - квиз
============================

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_1

        Како се назива класа библиотеке Flask којом се креира серверска апликација?

        Одговор: |blank|

        - :^Flask$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_2

        Допуни наредни Python код тако да се функција *kviz* изврши када корисник посети страницу на адреси *http://localhost:5500/kviz*.

        | ``@app.`` |blank| ``(`` |blank| ``)``
        | ``def kviz():``
        |   ``return "<p>Квиз</p>"``

        - :^route$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^("/kviz/?")|('/kviz/?')$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_3

        Допуни наредни Python код тако да се функција *kviz* изврши када корисник посети страницу на адресама *http://localhost:5500/kviz/1* и *http://localhost:5500/kviz/2*, при чему се за одговарајућу адресу прикаже одговарајући број на веб-страници.

        | ``@app.`` |blank| ``(`` |blank| ``)``
        | ``def kviz(broj):``
        |   ``return f"<p>Квиз {broj}</p>"``

        - :^route$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^("/kviz/<broj>/?")|('/kviz/<broj>/?')$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_4

        Како се назива функција библиотеке Flask која израчунава путање на основу назива функција?

        Одговор: |blank|

        - :^url_for$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_5

        Допуни наредни Python код тако да функција *kviz* процесира шаблон који се налази на путањи *templates/kviz.html*, а при чему шаблон очекује да му се проследи низ питања кроз Python листу *pitanja*.

        | ``@app...``
        | ``function kviz():``
        |   ``pitanja = ["Питање 1", "Питање 2", "Питање 3"]``
        |   ``return`` |blank|

        - :^render_template\s*\(\s*(("kviz\.html")|('kviz\.html'))\s*,\s*pitanja\s*=\s*pitanja\s*\)$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_6

        Допуни наредни HTML код тако да динамички шаблон генерише питања из Python листе *pitanja* као уређену листу.

        | ``<ol>``
        |   |blank|
        |     ``<li>{{ pitanje }}</li>``
        |   |blank|
        | ``</ol>`` 

        - :^{%\s*for\s*pitanje\s*in\s*pitanja\s*%}$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^{%\s*endfor\s*%}$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. mchoice:: biblioteka_flask_kviz_7
        :answer_a: Навођење садржаја у блоковима који ће бити замењени у наслеђеном шаблону.
        :answer_b: Повезивање шаблона функцијом за креирање рута.
        :answer_c: Навођењем назива шаблона који се наслеђује у функцији за процесирање шаблона.
        :answer_d: Навођењем команде extends за којом следи назив шаблона који се наслеђује.
        :correct: a, d

        Означи све неопходне кораке приликом наслеђивања шаблона.

.. quizq::

    Посматрај наредну структуру датотека на диску, па одговори на питање.

    .. code-block::

        .
        ├── main.py
        ├── static
        │   ├── melodija.mp3
        └── templates
            ├── kviz.html

    .. fillintheblank:: biblioteka_flask_kviz_8

        Допуни наредни HTML код из шаблона *kviz.html* тако да се на веб-страници прикаже контрола за репродуковање звучног записа *melodija.mp3*.

        | ``<audio controls>``
        |   ``<source src="`` |blank| ``" type="audio/mp3">``
        | ``</audio>``

        - :^{{\s*url_for\s*\(\s*'static'\s*,\s*filename\s*=\s*'stil.css'\s*\)\s*}}$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. mchoice:: biblioteka_flask_kviz_9
        :answer_a: request.params
        :answer_b: request.form
        :answer_c: request.args
        :answer_d: request.data
        :answer_e: ниједно од понуђених
        :correct: c

        Који од наведених речника се користи за дохватање података који су веб-страници послати методом GET?

.. quizq::

    .. mchoice:: biblioteka_flask_kviz_10
        :answer_a: request.params
        :answer_b: request.form
        :answer_c: request.args
        :answer_d: request.data
        :answer_e: ниједно од понуђених
        :correct: b

        Који од наведених речника се користи за дохватање података који су веб-страници послати методом POST?

.. quizq::

    .. fillintheblank:: biblioteka_flask_kviz_11

        Како се назива функција библиотеке Flask којом се региструју поруке (статусне поруке, поруке о грешкама, и др.) приликом обраде HTTP захтева?

        Одговор: |blank|

        Како се назива функција библиотеке Flask којом се приступа претходно регистрованим порукама у оквиру истог HTTP захтева?

        Одговор: |blank|

        - :^flash$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^get_flashed_messages$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. mchoice:: biblioteka_flask_kviz_12
        :answer_a: Код за приступање серверу електронске поште.
        :answer_b: Токен за читање података из базе података.
        :answer_c: Списак акција које је корисник извршио у систему са дељеним уређајима.
        :answer_d: ниједно од понуђених
        :correct: d 

        Који од наведених података је погодно чувати у оквиру колачића?