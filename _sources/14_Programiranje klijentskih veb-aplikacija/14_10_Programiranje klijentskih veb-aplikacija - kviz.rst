Програмирање клијентских веб-апликација - квиз
==============================================

.. quizq::

    .. mchoice:: programiranje_klijentskih_veb_aplikacija_kviz_1
        :answer_a: JavaScript програми се користе за изградњу динамичких веб-апликација.
        :answer_b: JavaScript код се може мењати током извршавања програма.
        :answer_c: JavaScript променљиве могу узимати вредности различитих типова.
        :answer_d: ниједно од понуђених
        :correct: c 

        На које од понуђених одговора се односи особина језика JavaScript која се назива динамичка типизираност?

.. quizq::

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_2

        Допуни наредни JavaScript код тако да променљива *x* не може узимати ниједну другу вредност осим вредности *5*.

        |blank| ``x =`` |blank| ``;``

        - :^const$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^5$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    Посматрај наредни JavaScript код, па одговори на питање.

    .. code-block:: JavaScript

        console.log(5/0);

    .. mchoice:: programiranje_klijentskih_veb_aplikacija_kviz_3
        :answer_a: У конзоли се исписује 1.
        :answer_b: У конзоли се исписује NaN.
        :answer_c: Долази до грешке типа SyntaxError.
        :answer_d: ниједно од понуђених
        :correct: d

        Који је резултат извршавања датог JavaScript кода?

.. quizq::

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_4

        Који је индекс карактера ”а” у ниски ”Ниска”?

        (Унеси само број који одговара индексу, без додатних карактера.)

        Одговор: |blank|

        - :^4$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_5

        Допуни наредни JavaScript код тако да се у конзоли испише дужина ниске *x*.

        | ``let x = "Програмирање";``
        | ``let duzina = x.`` |blank| ``;``
        | ``console.log(duzina); // 12``

        - :^length$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_6

        Допуни наредни JavaScript код тако да се у конзоли испише последњи карактер ниске *x*.

        | ``let x = "Програмирање";``
        | ``let poslednji_karakter = x.`` |blank| ``(`` |blank| ``);``
        | ``console.log(poslednji_karakter); // ”е”``

        - :^charAt$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^(x\.length\s*-\s*1)|11$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    Посматрај наредни JavaScript код, па одговори на питање.

    .. code-block:: JavaScript

      let x = 13 * 4;
      let y = 12 * 5;

      if (x > y) {
        console.log(1);
      } else {
        console.log(-1);
      }

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_7
        
        Која вредност ће бити исписана у конзоли за дати програмски код?

        Одговор: |blank|

        - :^-1$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    Посматрај наредни JavaScript код, па одговори на питање.

    .. code-block:: JavaScript

      let x = "Мала поморанџа пада са дрвета.";

      if (x.split(" ").length === 5) {
        console.log(1);
      } else {
        console.log(-1);
      }

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_8
        
        Која вредност ће бити исписана у конзоли за дати програмски код?

        Одговор: |blank|

        - :^1$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    Посматрај наредни JavaScript код, па одговори на питање.

    .. code-block:: JavaScript

      let x = [12, -3, 4, 0, 9, 0, -4, 1, 7];
      let brojac = 0;

      for (let i = 0; i < x.length; i++) {
        let el = x[i];

        if (el >= 0 && el < 10) {
          brojac++;
        }
      }

      console.log(brojac);

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_9
        
        Која вредност ће бити исписана у конзоли за дати програмски код?

        Одговор: |blank|

        - :^6$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    Посматрај наредни JavaScript код, па одговори на питање.

    .. code-block:: JavaScript

      let x = [1, 2, 3];
      let y = [1, 2, 3];

      if (x === y) {
        console.log(1);
      } else {
        console.log(-1);
      }

    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_10
        
        Која вредност ће бити исписана у конзоли за дати програмски код?

        Одговор: |blank|

        - :^-1$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    Посматрај наредни JavaScript код, па одговори на питање.

    .. code-block:: JavaScript

      function f(el) {
        return el.toUpperCase();
      }

      let x = ["a", "b", "C", "D", "e"];
      let y = [];

      for (let i = 0; i < x.length; i++) {
        let el_x = x[i];
        let el_y = f(el_x);
        y.push(el_y);
      }

      let z = y.join(" ");

      console.log(z);


    .. fillintheblank:: programiranje_klijentskih_veb_aplikacija_kviz_11
        
        Која вредност ће бити исписана у конзоли за дати програмски код?

        Одговор: |blank|

        - :^A B C D E$: Одговор је тачан.
          :x: Одговор није тачан.
