Начини за задавање правила за стилизовање
=========================================

Вероватно се питаш на који начин се CSS правила придружују неком HTML коду. Испоставља се да постоје три начина на које можеш да то урадиш. За сваки од њих је важно да разумеш намену и да препознаш ситуације у којима је сваки од начина представљају најпожељнији избор.

Први начин јесте увожењем спољашњег CSS документа у HTML документ. У овом начину, сва CSS правила се наводе у посебној датотеци, која уобичајено носи екстензију “.css”. Да би се та правила укључила у неки HTML документ (чиме ће та правила бити примењена на тај документ), у заглављу тог HTML документа је неопходно навести елемент ”link” који има три важна обавезна атрибута:

- Атрибутом ”rel” описујеш у каквом је односу датотека која се укључује. За стилске каскадне листове наводи се вредност ”stylesheet”.
- Атрибутом ”type” наводи се формат у којем је датотека која се укључује записана. За језик CSS наводи се формат ”text/css”.
- Атрибутом ”href” наводи се путања до саме датотеке, што може бити апсолутна адреса (било на локалном веб-серверу или URL адреса ка спољашњем веб-серверу) или релативна адреса.

На пример, ако се CSS датотека ”index.css” налази у истом директоријуму као и HTML датотека ”index.html”, онда се у њу може укључити на следећи начин:

.. code-block:: html

    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>Наслов</title>

        <!-- Пример увожења CSS датотеке -->
        <link rel="stylesheet" type="text/css" href="./index.css">
    </head>
    <body>
        <!-- Остатак HTML кода -->
    </body>
    </html>

Укључивање CSS датотеке на овај начин има неколико предности. Прво, кодови језика HTML и CSS су одвојени, што олакшава развој веб-сајтова. Друго, једну CSS датотеку је могуће укључити у више HTML датотека, што значи да је на овај начин могуће делити CSS код између више веб-страница, уместо да се иста правила копирају за сваку веб-страницу. Због ових разлога, овај приступ је најпожељнији у општем случају.

Други начин за задавање стилова јесте коришћењем елемента ”style”, који се такође наводи у заглављу HTML документа. Елемент ”style” има само један атрибут, а у питању је атрибут ”type” којем се такође наводи вредност ”text/css” као и у случају елемента ”link”. У оквиру садржаја овог атрибута наводе се CSS правила која ће бити примењена. Један пример овог начина је приказан у наредном коду.

.. code-block:: HTML

    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>Наслов</title>

        <!-- Пример навођења CSS правила у заглављу HTML документа -->
        <style type="text/css">
            /* CSS правила се наводе овде */
        </style>
    </head>
    <body>
        <!-- Остатак HTML кода -->
    </body>
    </html>

С обзиром да је CSS код уграђен у HTML страницу није га могуће делити, те се не препоручује за навођење стилова који су заједнички за већи број веб-страница. Ипак, уколико постоје стилови који треба да се примене само на једну веб-страницу, онда треба да преферираш овом начину. Чак и да у првом приступу користиш врло специфичне селекторе у CSS правилима, за које знаш да се не користе на другим веб-страницама, увек је могуће да ће ова чињеница промаћи другим програмерима који раде на истом веб-сајту, па се стилови могу применити и на њиховим веб-страницама без да су то очекивали. Ова појава се назива цурење стилова (енг. style spilling). Коришћење елемента ”style” је један начин да се ово понашање спречи.

Последњи начин за задавање стилова јесте коришћењем атрибута ”style”. Овај атрибут се може применити над било којим елементом садржаја HTML документа, па чак и над елементом ”body” који представља цео садржај. Вредност овог атрибута су CSS декларације (не правила!) која се раздвајају карактером ”;”. Наведене декларације ће бити придружене само на нивоу садржаја елемента над којим је наведен овај атрибут. Један пример овог начина је приказан у наредном коду.


.. code-block:: HTML

    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>Наслов</title>
    </head>
    <body>
        <!-- Пример навођења CSS декларација на нивоу елемента -->
        <div style="/* CSS декларације иду овде */">
            <!-- Остатак садржаја -->
        </div>
    </body>
    </html>

Овај начин навођења стилова је најспецифичнији, те се обично и не прибегава његовој употреби осим у случајевима када је потребно брзо применити неки стил како бисмо видели ефекте (на пример, у фази развоја веб-апликације). Штавише, због мешања HTML и CSS кода, целокупан документ постаје веома нечитљив, те се због тога и не препоручује његова примена.