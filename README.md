# <span style="color: purple;">**Questions**
## <span style="color: DarkSlateBlue;"> **1. Хэш-таблицы**
<span style="color: DarkSlateBlue; font-size: 16px"> <ins>__Хэш-таблица__</ins></span> - это структуры данных, которая хранит пары "ключ-значение" и обеспечивает быстрый доступ к данным по ключу за счёт использования хэш-функции. 

<span style="color: DarkSlateBlue; font-size: 16px;"> <ins>__Хэш-функция__</ins></span> - это функция, которая преобразует ключ в целое число, используемое для определения индекса в массиве хэш-таблицы. 

<span style="color: DarkSlateBlue; font-size: 16px"> <ins>__Хэшируемость__</ins></span> - это свойство объекта, позволяющее вычислить хэш-код с помощью функции hash().  

<p style="border-left: 3px solid DarkSlateBlue; padding-left: 10px;">
В Python хэш-таблицы используются в словарях (dict) и множествах (set). 
Ключи должны быть неизменяемые, чтобы их хэш-код не менялся. <i>Хэшируемые типы</i> в Python: <code>str</code>, <code>int</code>, <code>float</code>, <code>bool</code>, <code>frozenset</code>, <code>tuple</code>.  <em>Нехэшируемые</em>: <code>list</code>, <code>dict</code>, <code>set</code>. 

<table border="0" style="border-collapse: collapse; width: 100%; margin: 20px auto; font-family: sans-serif; font-size: 14px;">
    <tr>
        <th colspan="2">Метод открытой адресации</th>
        <th colspan="2">Метод цепочек</th>
    </tr>
    <tr>
        <th>+</th>
        <th>-</th>
        <th>+</th>
        <th>-</th>
    </tr>
    <tr>
        <td>Быстрый обход</td>
        <td>Зависимость от способа обхода</td>
        <td>Простота реализации</td>
        <td>Расход памяти на ссылку</td>
    </tr>
    <tr>
        <td>Меньший расход памяти</td>
        <td>Зависимость от размера внутреннего массива</td>
        <td></td>
        <td>Медленный обход</td>
    </tr>
</table>