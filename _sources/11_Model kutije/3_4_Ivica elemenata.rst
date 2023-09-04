Ивица елемената
===============

У језику CSS могуће је управљати различитим карактеристикама ивице елемената. Свака од ових карактеристика има одговарајућа својства. Ова својства можеш да наведеш за сваку страну посебно, или за више страна одједном, на исти начин као што је то случај са допуном елемента.

Стил ивице
__________

Стилом ивице управљаш помоћу својства ”border-style”, односно, својствима ”border-top-style”, ”border-right-style”, ”border-bottom-style” и ”border-right-style”. Неке од могућих вредности ових својстава су:

- Вредност ”solid” означава стил пуне линије.
- Вредност ”dashed” означава стил испрекидане линије. 
- Вредност ”dotted” означава стил тачкасте линије.
- Вредност ”double” означава стил дупле пуне линије.
- Вредност ”hidden” означава да ивица неће бити видљива, али је могуће управљати осталим карактеристикама.

.. petlja-editor:: Poglavlje3/18

    index.html
    <!-- Poglavlje3/18/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - стил ивице</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div>Овај елемент има све ивице постављене у стилу пуне линије.</div>

        <p>Овај елемент има горњу ивицу у стилу испрекидане линије и доњу ивицу у стилу тачкасте линије.</p>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/18/index.css */
    
    div,
    p {
        width: 300px;
        height: 100px;
    }

    div {
        border-style: solid;
    }

    p {
        border-top-style: dashed;
        border-bottom-style: dotted;
    }


Уколико желиш да подесиш било коју од наредних карактеристика ивице, обавезно мораш да прво подесиш стил ивице. У супротном, те карактеристике неће бити примењене.
Ширина ивице
Када поставиш стил ивице, она добија подразумевану ширину од ”1px”. Ово можеш да промениш коришћењем својства ”border-width”, односно неког од својстава ”border-top-width”, ”border-right-width”, ”border-bottom-width” и ”border-left-width”. Ширина ивице се може задати у разним дужинама. 

.. petlja-editor:: Poglavlje3/19

    index.html
    <!-- Poglavlje3/19/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - ширина ивице</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div>Овај елемент има све ивице постављене у стилу пуне линије ширине 10px.</div>

        <p>
        Овај елемент има горњу ивицу у стилу испрекидане линије ширине 20px и доњу ивицу у стилу тачкасте линије ширине
        30px.
        </p>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/19/index.css */
    
    div,
    p {
        width: 300px;
        height: 100px;
    }

    div {
        border-style: solid;
        border-width: 10px;
    }

    p {
        border-top-style: dashed;
        border-top-width: 20px;
        border-bottom-style: dotted;
        border-bottom-width: 30px;
    }


Боја ивице
__________

Након што подесиш стил ивице, приметићеш да је она подразумевано црне боје. Ако желиш да подесиш неку другу боју, можеш да искористиш својство ”border-color” или неко од својстава ”border-top-color”, ”border-right-color”, ”border-bottom-color” и ”border-left-color”. Вредности које ова својства могу добити су боје, задате било путем њихових назива, RGB или HEX формата.

.. petlja-editor:: Poglavlje3/20

    index.html
    <!-- Poglavlje3/20/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - боја ивице</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div>Овај елемент има све ивице постављене у стилу пуне линије, ширине 10px и светлоплаве боје.</div>

        <p>
        Овај елемент има горњу ивицу у стилу испрекидане линије, ширине 20px и светлоцрвене боје и доњу ивицу у стилу
        тачкасте линије ширине 30px и розе боје.
        </p>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/20/index.css */
    
    div,
    p {
        width: 300px;
        height: 100px;
    }

    div {
        border-style: solid;
        border-width: 10px;
        border-color: deepskyblue;
    }

    p {
        border-top-style: dashed;
        border-top-width: 20px;
        border-top-color: salmon;
        border-bottom-style: dotted;
        border-bottom-width: 30px;
        border-bottom-color: deeppink;
    }


Својство ”border”
_________________

Ако желиш да поставиш више карактеристика одједном, поред навођења одговарајућих својстава као што смо до сада приказали, можеш да искористиш и својство ”border” које омогућава скраћени запис примене карактеристика ивице. Ово својство се односи на све ивице одједном, а постоје и варијанте ”border-top”, ”border-right”, ”border-bottom” и ”border-left”. 

Приликом навођења овог својства, обавезно је да наведеш стил ивице као прву карактеристику. Остала својства (боју и ширину), ако желиш да их подесиш, можеш навести у произвољном редоследу.

.. petlja-editor:: Poglavlje3/21

    index.html
    <!-- Poglavlje3/21/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - својство ”border”</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div>Овај елемент има све ивице постављене у стилу пуне линије, ширине 10px и светлоплаве боје.</div>

        <p>
        Овај елемент има горњу ивицу у стилу испрекидане линије, ширине 20px и светлоцрвене боје и доњу ивицу у стилу
        тачкасте линије ширине 30px и розе боје.
        </p>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/21/index.css */
    
    div,
    p {
        width: 300px;
        height: 100px;
    }

    div {
        border: solid 10px deepskyblue;
    }

    p {
        border-top: dashed 20px salmon;
        border-bottom: dotted 30px deeppink;
    }


Закривљење ивице
________________

Ивицу је могуће закривити чиме се добија обла линија у угловима правоугаоника елемента. За подешавање степена закривљења се може користити својство ”border-radius” чија вредност може узимати различите дужине. И овом својству је могуће навести неколико дужина, а у зависности од броја наведених дужина, ефекти се разликују:

- Декларацијом ”border-radius: 15px 50px 30px 5px” ће горњи-леви угао бити закривљен за 15px, горњи-десни угао за 50px, доњи-десни угао за 30px и доњи-леви угао за 5px.
- Декларацијом ”border-radius: 15px 50px” ће горњи-леви и доњи-десни углови бити закривљени за 15px, а горњи-десни и доњи-леви углови за 50px.
- Декларацијом ”border-radius: 20px” ће сва четири угла бити закривљена за 20px.

.. petlja-editor:: Poglavlje3/22

    index.html
    <!-- Poglavlje3/22/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - закривљење ивице</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <div id="div-1">Овај елемент има углове закривљене за 15px 50px 30px 5px, редом.</div>
        <br>
        <div id="div-2">Овај елемент има углове закривљене за 15px 50px 15px 50px, редом.</div>
        <br>
        <div id="div-3">Овај елемент има све углове закривљене за 20px.</div>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/22/index.css */
    
    div {
        width: 300px;
        height: 100px;
        background-color: forestgreen;
        color: azure;
        padding: 20px;
    }

    #div-1 {
        border-radius: 15px 50px 30px 5px;
    }

    #div-2 {
        border-radius: 15px 50px;
    }

    #div-3 {
        border-radius: 20px;
    }

