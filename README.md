# fluffy-octo-fiesta
formulário responsivo que se adapte a um carrossel e também inclua automação de e-mail

<!DOCTYPE html>
<html>
<head>
	<title>Formulário responsivo ao carrossel</title>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
</head>
<body>

	<div class="container">
		<h2>Formulário de Contato</h2>
		<div id="myCarousel" class="carousel slide" data-ride="carousel">
			<!-- Indicadores -->
			<ol class="carousel-indicators">
				<li data-target="#myCarousel" data-slide-to="0" class="active"></li>
				<li data-target="#myCarousel" data-slide-to="1"></li>
				<li data-target="#myCarousel" data-slide-to="2"></li>
			</ol>

			<!-- Slides do carrossel -->
			<div class="carousel-inner">
				<div class="item active">
					<form id="formulario1" class="formulario">
						<label for="nome">Nome:</label>
						<input type="text" id="nome" name="nome" required>
						<label for="email">E-mail:</label>
						<input type="email" id="email" name="email" required>
						<button type="submit" onclick="enviarEmail()">Enviar</button>
					</form>
				</div>

				<div class="item">
					<form id="formulario2" class="formulario">
						<label for="telefone">Telefone:</label>
						<input type="text" id="telefone" name="telefone" required>
						<label for="mensagem">Mensagem:</label>
						<textarea id="mensagem" name="mensagem" required></textarea>
						<button type="submit" onclick="enviarEmail()">Enviar</button>
					</form>
				</div>

				<div class="item">
					<form id="formulario3" class="formulario">
						<label for="assunto">Assunto:</label>
						<input type="text" id="assunto" name="assunto" required>
						<label for="mensagem">Mensagem:</label>
						<textarea id="mensagem" name="mensagem" required></textarea>
						<button type="submit" onclick="enviarEmail()">Enviar</button>
					</form>
				</div>
			</div>

			<!-- Controles do carrossel -->
			<a class="left carousel-control" href="#myCarousel" data-slide="prev">
				<span class="glyphicon glyphicon-chevron-left"></span>
				<span class="sr-only">Anterior</span>
			</a>
			<a class="right carousel-control" href="#myCarousel" data-slide="next">
				<span class="glyphicon glyphicon-chevron-right"></span>
				<span class="sr-only">Pró
