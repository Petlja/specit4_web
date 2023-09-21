JavaScript и DOM API - квиз
===========================

.. quizq::

    .. mchoice:: javascript_i_dom_api_kviz_1
        :answer_a: HTMLElement
        :answer_b: Node
        :answer_c: Element
        :correct: b

        Који од наредних интерфејса DOM API библиотеке имплементира највећи број чворова у DOM стаблу?

.. quizq::

    .. parsonsprob:: javascript_i_dom_api_kviz_2

        Поређај интерфејсе DOM API библиотеке од најопштијег до најспецифичнијег.
        -----
        Node
        Element
        HTMLElement
        HTMLFormElement

.. quizq::

    .. dragndrop:: javascript_i_dom_api_kviz_3
        :match_1: getElementById ||| претрага једног, унапред познатог елемента
        :match_2: querySelector ||| претрага једног елемента на основу сложених селектора
        :match_3: querySelectorAll ||| претрага више елемента на основу сложених селектора

        Повежи методе интерфејса *Document* са одговарајућим сценаријима у којима су најпогоднији за коришћење.

.. quizq::

    .. mchoice:: javascript_i_dom_api_kviz_4
        :answer_a: borderWidth
        :answer_b: BorderWidth
        :answer_c: border-width
        :answer_d: ниједно од понуђених
        :correct: a

        Путем којег од понуђених својстава из DOM API библиотеке је могуће (у језику JavaScript) приступити вредности CSS својства *border-width*?

.. quizq::

    .. fillintheblank:: javascript_i_dom_api_kviz_5

        Допуни наредни JavaScript код тако да се елементу промени величина слова на *16px*.

        | ``let el = document.getElementById("el");``
        | ``el.`` |blank| ``=`` |blank| ``;``

        - :^(style.fontSize)|(style\["fontSize"\])$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^"16px"$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. fillintheblank:: javascript_i_dom_api_kviz_6

        Допуни наредни JavaScript код тако да набрајање уређене листе почиње од *5*.

        | ``let ol = document.querySelector("ol");``
        | ``el.`` |blank| ``=`` |blank| ``;``

        - :^start$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^(5)|("5")|('5')|(`5`)$: Други одговор је тачан.
          :x: Други одговор није тачан.

.. quizq::

    .. fillintheblank:: javascript_i_dom_api_kviz_7

        Допуни наредни JavaScript код тако да се у садржају веб-странице (тј. у садржају HTML елемента *body*) прикаже по пасус за сваку реч из реченице коју корисник уноси у дијалогу за унос текста.

        | ``let recenica = prompt("Унеси реченицу:");``
        | ``let reci = recenica.split(" ");``
        | ``let body = document.querySelector("body");``
        | ``let sadrzaj = "";``
        | 
        | ``for (let i = 0; i < reci.length; i++) {``
        |   ``sadrzaj += "<p>" + reci[i] + "</p>";``
        | ``}``
        |
        | ``body.`` |blank| ``= sadrzaj;``

        - :^innerHTML$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: javascript_i_dom_api_kviz_8

        Како се зове метод интерфејса *EventTarget* из DOM API библиотеке који користиш како би регистровао функцију која извршава акцију на неки кориснички догађај?

        Одговор: |blank|

        - :^addEventListener$: Одговор је тачан.
          :x: Одговор није тачан.

.. quizq::

    .. fillintheblank:: javascript_i_dom_api_kviz_9

        Допуни наредни JavaScript код тако да се на клик дугмета испише у конзоли порука *”Здраво!”*.

        | ``function klik() {``
        |   ``console.log("Здраво!");``
        | ``}``
        | 
        | ``let dugme = querySelector("button");``
        | ``dugme.`` |blank| ``(`` |blank| ``,`` |blank| ``);``

        - :^addEventListener$: Први одговор је тачан.
          :x: Први одговор није тачан.
        - :^("click")|('click')|(`click`)$: Други одговор је тачан.
          :x: Други одговор није тачан.
        - :^klik$: Трећи одговор је тачан.
          :x: Трећи одговор није тачан.
        



