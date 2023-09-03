Стилизовање табела
==================

Попут листи, и разне елементе који учествују у формирању табеларног приказа садржаја је могуће стилизовати различитим CSS својствима. У овој лекцији ћеш упознати својства која су својеврсна табелама.

Подразумевано, табеле немају ивицу, али она им се лако може придружити добро познатим CSS својством *border* (и осталим својствима из те фамилије). Ивицу можеш поставити око читаве табеле (применом својства *border* на HTML елемент *table*), али и на нивоу појединачних ћелија (применом својства *border* на HTML елементе *td* или *th*). Уколико се определиш за оба приступа, онда се можеш одлучити да ли табела треба да прикаже све ивице или да споји суседне ивице како би се добио традиционални табеларни приказ. Ову опцију можеш контролисати навођењем својства *border-collapse*, чија вредност separate означава раздвојене ивице, а вредност *collapse* означава спојене ивице.

.. petlja-editor:: Poglavlje3/36

    index.html
    <!-- Poglavlje3/36/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - стилизовање табела</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <p>Однос разног воћа и њиховог броја у килограму:</p>
        <table id="bez-spojenih-ivica">
        <tr>
            <th>Воћкице</th>
            <th>Број у kg</th>
        </tr>
        <tr>
            <td>Јабуке</td>
            <td>&lt; 20</td>
        </tr>
        <tr>
            <td>Боровнице</td>
            <td>&gt; 100</td>
        </tr>
        </table>

        <p>Однос разног поврћа и њиховог броја у килограму:</p>
        <table id="sa-spojenim-ivicama">
        <tr>
            <th>Поврће</th>
            <th>Број у kg</th>
        </tr>
        <tr>
            <td>Шаргарепе</td>
            <td>&lt; 20</td>
        </tr>
        <tr>
            <td>Чери парадајз</td>
            <td>&gt; 50</td>
        </tr>
        </table>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/36/index.css */
    
    table,
    th,
    td {
        border: solid 1px black;
    }

    #bez-spojenih-ivica {
        border-collapse: separate;
    }

    #sa-spojenim-ivicama {
        border-collapse: collapse;
    }


Својство *caption-side* користиш за подешавање позиције наслова табеле. Као што ти је познато, наслов табеле се увек наводи (ако се наводи) као први потомак елемента *table* и подразумевано се приказује изнад табеле. Овом понашању одговара вредност *top* својства *caption-side*. Са друге стране, постављањем овог својства на вредност *bottom*, омогућаваш наслову да се пребаци испод табеле. 

.. petlja-editor:: Poglavlje3/37

    index.html
    <!-- Poglavlje3/37/index.html -->
    
    <!DOCTYPE html>
    <html lang="sr">
    <head>
        <meta charset="utf-8">
        <title>CSS - стилизовање табела</title>

        <link rel="stylesheet" type="text/css" href="index.css">
    </head>
    <body>
        <table id="siroka-tabela">
        <caption>
            Табела 1: Однос разног воћа и њиховог броја у килограму.
        </caption>
        <tr>
            <th>Воћкице</th>
            <th>Број у kg</th>
        </tr>
        <tr>
            <td>Јабуке</td>
            <td>&lt; 20</td>
        </tr>
        <tr>
            <td>Боровнице</td>
            <td>&gt; 100</td>
        </tr>
        </table>

        <p>Однос разног поврћа и њиховог броја у килограму:</p>
        <table id="obojena-tabela">
        <tr>
            <th>Поврће</th>
            <th>Број у kg</th>
        </tr>
        <tr class="neparni-red">
            <td>Шаргарепе</td>
            <td>&sim; 20</td>
        </tr>
        <tr class="parni-red">
            <td>Чери парадајз</td>
            <td>&gt; 50</td>
        </tr>
        </table>
    </body>
    </html>
    ~~~
    index.css
    /* Poglavlje3/37/index.css */
    
    table,
    th,
    td {
        border: solid 1px black;
        padding: 10px;
    }

    #siroka-tabela {
        width: 100%;
        caption-side: bottom;
    }

    #obojena-tabela {
        border-collapse: collapse;
        caption-side: top;
    }

    #obojena-tabela th {
        background-color: dodgerblue;
        color: white;
    }

    #obojena-tabela .neparni-red {
        background-color: azure;
    }

    #obojena-tabela .parni-red {
        background-color: rgba(0, 191, 255, 0.5);
    }

