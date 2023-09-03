Спољашњи појас елемената (маргина)
==================================

Маргина представља површину која раздваја ивицу елемента од осталих елемената. Попут допуне, и за маргину постоје четири својства којима је могуће подешавати површину спољашњег појаса за различите стране. То су својства ”margin-top” (горња маргина), ”margin-right” (десна маргина), ”margin-bottom” (доња маргина) и ”margin-left” (лева маргина). Њихове вредности могу бити неке од дужина и представљају ширину маргине на одговарајућој страни. Подразумевана вредност маргина зависи од елемента, али у већини случајева је ”0”.

Постоји и својство ”margin” којим се могу навести димензије маргина за све стране одједном. Ово својство функционише на исти начин као својство ”padding”.

.. petlja-editor:: Poglavlje3/23

    index.html
    <!-- Poglavlje3/23/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - маргина</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div>
        <p>
            Овај елемент има горњу и доњу маргину од 100px, док десна и лева маргина заузимају 20% ширине родитељског
            елемента.
        </p>
        </div>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/23/index.css */
    
    div {
        border: black solid 1px;
        width: 50%;
    }

    p {
        border: 1px solid black;
        margin-top: 100px;
        margin-bottom: 100px;
        margin-right: 20%;
        margin-left: 20%;
        background-color: lightblue;
    }

