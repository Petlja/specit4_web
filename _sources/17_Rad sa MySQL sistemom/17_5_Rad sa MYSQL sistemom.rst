Рад са MySQL системом за управљање базама података - квиз
=========================================================


.. quizq::

    .. fillintheblank:: flask_mysql_kviz_1

        Допуни наредни Python код тако да се серверска веб-апликација повеже на базу података *”moja_bp”* у оквиру локалног MySQL СУБП.

        | ``import mysql.connector``
        |
        | ``mydb =`` |blank| ``(``
        |   ``host="localhost", user="root", password="",`` |blank|
        | ``)``

        - :^mysql.connector.connect$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^\s*database\s*=\s*(("moja_bp")|('moja_bp'))\s*$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. mchoice:: flask_mysql_kviz_2
        :answer_a: UPDATE
        :answer_b: SELECT
        :answer_c: DELETE
        :answer_d: INSERT
        :answer_e: ниједно од понуђених
        :correct: a, b, c, d

        Означи врсте SQL наредби за које је неопходна употреба курсора приликом коришћења *MySQLConnection* објеката.

.. quizq::

    .. fillintheblank:: flask_mysql_kviz_3

        Допуни наредни Python код тако да серверска веб-апликација излиста наслове свих књига и њихове ауторе из базе података једне књижаре.

        | ``mydb = mysql.connector...``
        | 
        | ``@app.route...``
        | ``def prikazi_knjige():``
        |
        |   ``kursor =`` |blank|
        |   ``upit = "SELECT naslov, autor FROM knjige"``
        |   ``kursor.`` |blank| ``(upit)``
        |   ``knjige = kursor.`` |blank|
        | 
        |   ``return ...``

        - :^mydb\.cursor\(\s*(dictionary\s*=\s*True)?\s*\)$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^execute$: Други одговор је тачан.
          :x: Други одговор није тачан.
        - :^fetchall\(\s*\)$: Трећи одговор је тачан.
          :x: Трећи одговор није тачан.

.. quizq::

    .. fillintheblank:: flask_mysql_kviz_4

        Допуни наредни Python код тако да серверска веб-апликација излиста наслове свих књига и њихове ауторе из базе података једне књижаре, али само за оне књиге које су издате између 2012. и 2015. године.

        | ``mydb = mysql.connector...``
        | 
        | ``@app.route...``
        | ``def prikazi_knjige_izdate_izmedju_2012_i_2015():``
        |
        |   ``kursor = ...``
        |   ``upit =`` 
        |     ``"SELECT naslov, autor FROM knjige "`` 
        |     ``"WHERE godina_izdavanja BETWEEN %(od)s AND %(do)s "``
        |   ``kursor.`` |blank| ``(upit,`` |blank| ``)``
        |   ``knjige = kursor...``
        | 
        |   ``return ...``

        - :^execute$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^params\s*=\s*{\s*("od"|'od')\s*:\s*2012\s*,\s*("do"|'do')\s*:\s*2015\s*}$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. mchoice:: flask_mysql_kviz_5
        :answer_a: UPDATE
        :answer_b: SELECT
        :answer_c: DELETE
        :answer_d: INSERT
        :answer_e: ниједно од понуђених
        :correct: a, c, d

        Означи врсте SQL наредби за које је неопходна употреба наредбе за потврђивање операције приликом коришћења *MySQLConnection* објеката.