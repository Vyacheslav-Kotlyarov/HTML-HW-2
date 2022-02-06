# HTML-HW-2

Создать и сохранить в Sublime text3 (или любом другом редакторе кода) файл, названный namesurname2.html.


Где name - это Ваше имя (английскими буквами), surname - ваша фамилия(английскими буквами), 2 обозначает номер урока 2.

Сверстать одну страницу сайта ИЛИ блочной ИЛИ табличной версткой.

Для блочной верстки можно использовать GRID, FLEX, block (что нравится)


Требования к сайту (при любом выборе верстки):

1. ширина сайта 80%;

2. на странице должны быть:

- хедер,

- основная часть (3 раздела - слева 15% по ширине, справа 25% по ширине),

- футер.

3. расположение всего блока с версткой по центру страницу.

Контент и цвета, шрифты - на ваше усмотрение, но желательно внутри основной части применять разные цвета для удобства отображения страницы.

Css следует прописать внутри тега style
------------------------------------------------------------------


<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Document</title>
<style type="text/css">
 	
  body {
   width: 80%;
   margin: 0 auto;
  }

 	.row {
    text-align: center;
    margin: 0 auto;
    background: dimgray;
    display: grid;
    grid-auto-rows: 5fr 50% 5fr;
    grid-template-columns: 15% 60% 25%;
    height: 500px;
    justify-content: center;
  
 
   grid-template-areas:
    "header header header"
     "nav article ads" 
      "footer footer footer"
  }

  .header {

    background-color: lightgreen;
    grid-area: header;
}

  .nav{
    background: lightcyan;
    float: left;
 }

  .article{ 
    background:lightseagreen ;
    float: left;
}

  .ads{
     background-color: lightpink;
    float:left;
}
.footer {

  background-color: lightsteelblue;
  grid-area: footer;

}

</style>


</head>
<body>
  <div class="row">
    <div class="row__item header">
      <h1>Header</h1>
  </div>
    <div class="row__item nav">
     <h1>левый блок</h1>
  </div>
    <div class="row__item article">
      <h1>центральный блок</h1>
  </div>
    <div class="row__item ads">
     <h1>правый сектор</h1>
  </div>
    <div class="row__item footer">
     <h1>F00ter</h1></div>
  </div>

	
</body>
</html>
