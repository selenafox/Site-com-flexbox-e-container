# Site-com-flexbox-e-container
coelitos, treinos com flexbox e containers
  *o html começa aqui!*
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
		<title>Coelitos</title>
			<link rel="stylesheet" type="text/css" href="teste1.css">
</head>
<body>
	<header class="header">
		<a href="#">Coelhinhos</a>
			<nav>
				<ul class="menu">
					<li><a href="#">Sobre</a></li>
					<li><a href="#">Produtos</a></li>
					<li><a href="#">Informações</a></li>
					<li><a href="#">Compartilhe</a></li>
				</ul>
			</nav>
	</header>
<h1>Section Flexbox</h1>
	<section class="flex">
		<div>
			<img src="coelho1.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho2.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho3.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho4.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho5.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho6.png">
				<p>Legenda</p>
		</div>
	</section>

	<section class="grid1">
		<div>
			<img src="coelho1.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho2.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho3.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho4.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho5.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho6.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho1.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho2.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho3.png">
				<p>Legenda</p>
		</div>
		<div>
			<img src="coelho4.png">
				<p>Legenda</p>
		</div>
	</section>

</body>
</html>

*o Html termina aqui!*

*O css começa aqui!*
body, ul, li, p{ /*configurações padrão para estes itens*/
	margin: 0px;
	padding: 0px;
	list-style: none;
	font-size: 1.2rem; /*tamano ideal de fonte */
	font-family: arial;
}
body header a {
	font-size: 1.2rem;
	font-family: arial; /*fonte da letra*/
}

body ul li {
	margin: 0px; /*tirar a margem*/
	padding: 0px; /*espaçamentp*/
	list-style: none; /*tirar da forma de lista*/
	font-size: 1.2rem;
	font-family: arial;
}
a {
	text-decoration: none;
	color: white;
}
body h1 {
	font-family: arial;
	text-align: center;
	margin-top: 50px;
}
 
 img {
 	max-width: 100%;
 	display:block;
 }
.header {
	display: flex; /*colocar a logo ao lado*/
	justify-content: space-between; /*espaços entre os itens*/
	padding: 20px; /*tamanho dos espaços*/
	align-items: center; /*alinhando os itens no centro, no caso a logo*/
	flex-wrap: wrap; /*quebra de itens quando a tela for menor*/
	background-color: black;
}
.menu { /*criando um menu nabrra de navegção*/
	display: flex; 
}
.menu li {
	margin-left: 20px;/*tamanho dos espaços entre os itens do menu*/
}
.menu li a { /*área de contato para clique maior*/
	display: block; 
	padding: 10px;
	background: tomato;
}
/*css flexbox 1*/
.flex{
	display: flex; /*garantir a flex box*/
	flex-wrap: : wrap; /* quebra de imagens*/
	max-width: 1000px; /*tamanho maximo da caixa*/
	margin: 0 auto;
}
.flex > div {
	flex: 1 1 500px;
	margin: 5px; /*margem das imagens*/
}

/* css grid*/

.grid1 {
	display: grid;
	grid-template-columns: repeat(3, 1fr);
	max-width: 1000;
	margin: 0 auto;
	grid-gap: 10px;
}

*o css termina aqui!*
