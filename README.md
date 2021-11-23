# goit-markup-hw-02
Home work 2

Атрибут "aria-label" задает значение для любого тега для читалки.
Например иконки-ссылки:
<a href="/" aria-label="web site link"><код SVG-иконки></a>
Чтобы читалка распознала о чем иконка без надписи и подписи, то есть для любого объекта не имеющего семантического значения. 



"*" - такой селектор влияет вообше на все что есть в документе! В основном он используется для сброса каких-либо предустановок (например убрать все подчеркивания у документов)
*{
    color: skyblue;
}


можно перед объявлением стиля поставить через запятую сразу несколько селекторов
например^
a, p{
list-style: none;    
}

Селектор класса - это селектр для того чтобы присвоить конкретному тегу стиль
Например:
.links{
    color: red;
}

Селектор атрибута - это селектор для всех тех тегов или строк кода где встречается этот атрибут

А есть селектор значения атрибута еще более специфичный способ закрепить стиль для нужного элемента

свойства "inherit" позволяет потомку наследовать все изменения которуе будут у родителя.

"пробел" между селекторами означает "потомка". 
.schedule-body tr:hover {background-color: tomato; color: white;} 
То есть все, что вложено в элемент "tr", который находится в классе "schedule-body", будет окрашиваться так как прописано в объявлениях данного правила CSS.

">" между селекторами означает "ребенка". 
.schedule-body > tr:hover {background-color: tomato; color: white;} 
То есть только ребенки первого уровня, вложеные в элемент "tr", который находится в классе "schedule-body", будет окрашиваться так как прописано в объявлениях данного правила CSS. Оебенки второго и последующих вложенностей не будут окрашиваться по правилу CSS/