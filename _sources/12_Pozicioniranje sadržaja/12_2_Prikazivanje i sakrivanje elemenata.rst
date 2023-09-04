Приказивање и сакривање елемената
=================================

Често је потребно да елементе прикажеш са неким другачијим својствима од оних која су им подразумевано додељена. У језику CSS постоји својство display које одређује како HTML елемент треба да буде приказан у оквиру веб-странице. Постоје различите вредности за ово својство које утичу на начин приказа елемента, а најчешће коришћене вредности су: *block, inline, inline-block* и *none*.

Вредности *block* и *inline* користиш да промениш понашање елемента тако да има карактеристике блоковских, односно, линијских елемената, редом. О овим карактеристикама је било речи раније. Постављањем вредности *inline-block* за својство display омогућаваш HTML елементу да се понаша и као блоковски и као линијски елемент. Прецизније, HTML елемент на кога делује ова вредност се приказује у истом реду са текстом и другим *inline* елементима, али му се такође може поставити ширина и висина, као код *block* елемената.

.. petlja-editor:: Poglavlje3/30

    index.html
    <!-- Poglavlje3/30/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS позиционирање - својство "display"</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <p>Блоковски елементи:</p>
        <div id="blokovski">
        <div class="plavi">Плави</div>
        <div class="crveni">Црвени</div>
        <div class="zlatni">Златни</div>
        </div>

        <p>Линијски елементи:</p>
        <div id="linijski">
        <div class="plavi">Плави</div>
        <div class="crveni">Црвени</div>
        <div class="zlatni">Златни</div>
        </div>

        <p>Блок-линијски елементи:</p>
        <div id="blok-linijski">
        <div class="plavi">Плави</div>
        <div class="crveni">Црвени</div>
        <div class="zlatni">Златни</div>
        </div>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/30/index.css */
    
    div {
        width: 50px;
        height: 50px;
    }

    #blokovski,
    #linijski,
    #blok-linijski {
        height: 150px;
        width: 100%;
        border: 1px solid black;
    }

    .plavi {
        background-color: dodgerblue;
    }

    .crveni {
        background-color: firebrick;
    }

    .zlatni {
        background-color: goldenrod;
    }

    /* Правила од значаја за овај пример */

    #blokovski div {
        display: block;
    }

    #linijski div {
        display: inline;
    }

    #blok-linijski div {
        display: inline-block;
    }


Поред ових вредности, својство *display* може имати и вредност *none*. Ову вредност користиш када је потребно да уклониш HTML елемент са веб-странице.

У ту сврху можеш да користиш још једно својство језика CSS. У питању је својство *visibility*, које има могуће вредности *hidden* и *visible*. Вредност *hidden* користиш ради прикривања HTML елемената на веб-страници, док се вредношћу *visible* приказују претходно прикривени елементи.

Важно је да разумеш разлику између декларација *display: none* и *visibility: hidden*. Применом прве декларације на неки HTML елемент, ти тај елемент уклањаш из DOM стабла, чиме утичеш на распоред осталих елемената на веб-страници. Са друге стране, применом друге декларације, тај елемент и даље заузима исти простор на веб-страници, али је невидљив.

.. petlja-editor:: Poglavlje3/31

    index.html
    <!-- Poglavlje3/31/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS позиционирање - приказивање и сакривање</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div id="leva-kolona">
        <p>Ова колона садржи 3 елемента, од којих је један сакривен декларацијом ”visibility: hidden”.</p>
        <div id="plavi"></div>
        <div id="crveni" class="sakriven"></div>
        <div id="zlatni"></div>
        </div>
        <div id="desna-kolona">
        <p>Ова колона садржи 3 елемента, од којих је један изузет из DOM стабла декларацијом ”display: none".</p>
        <div id="plavi"></div>
        <div id="crveni" class="izuzet"></div>
        <div id="zlatni"></div>
        </div>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/31/index.css */
    
    div {
        width: 300px;
        height: 100px;
    }

    #leva-kolona,
    #desna-kolona {
        position: absolute;
        width: 400px;
        height: 400px;
        border: 5px solid black;
        margin: 10px;
    }

    #leva-kolona {
        top: 0px;
        left: 0px;
        background-color: bisque;
    }

    #desna-kolona {
        top: 0px;
        right: 0px;
        background-color: darkseagreen;
    }

    #plavi {
        background-color: dodgerblue;
    }

    #crveni {
        background-color: firebrick;
    }

    #zlatni {
        background-color: goldenrod;
    }

    /* Правила од значаја за овај пример */

    .sakriven {
        visibility: hidden;
    }

    .izuzet {
        display: none;
    }

