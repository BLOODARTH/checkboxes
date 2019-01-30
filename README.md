<?php 
  session_start(); 

  if (!isset($_SESSION['username'])) {
  	$_SESSION['msg'] = "You must log in first";
  	header('location: index.php');
  }
  if (isset($_GET['logout'])) {
  	session_destroy();
  	unset($_SESSION['username']);
  	header("location: index.php");
  }
?>

<!DOCTYPE HTML>
<!--
	Forty by HTML5 UP
	html5up.net | @ajlkn
	Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)
-->
<html>
	<head>
		<title>Tonatico</title>
		<meta "charset=utf-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
		<link rel="stylesheet" href="assets/css/main.css" />
		<noscript><link rel="stylesheet" href="assets/css/noscript.css" /></noscript>
	</head>
	<body class="is-preload">

		<!-- Wrapper -->
			<div id="wrapper">

				<!-- Header -->
				<!-- Note: The "styleN" class below should match that of the banner element. -->
					<header id="header" class="alt style2">
						<a href="index2.php" class="logo"><strong>NISSAN</strong> <span>X-TRAIL</span></a>
						<nav>
							<a href="#menu">Menu</a>
						</nav>
					</header>

				<!-- Menu -->
					<nav id="menu">
						<ul class="links">
							<li><a href="index2.php">Inicio</a></li>
							<li><a href="Viajar.php">Viajar</a></li>
							<li><a href="video.php">Video</a></li>
							<li><a href="elements.html">Nissan</a></li>
						</ul>
						<ul class="actions stacked">

							 <?php  if (isset($_SESSION['username'])) : ?>
    							<p>Bienvenido <strong><?php echo $_SESSION['username']; ?></strong></p>						
    						<?php endif ?>							
							<li><a href="index.php?logout='1'" class="button fit">Salir</a></li>
						</ul>
					</nav>

				<!-- Banner -->
				<!-- Note: The "styleN" class below should match that of the header element. -->
					<section id="banner" class="style2">
						<div class="inner">
							<span class="image">
								<img src="images/Tonatico1.jpg" alt="" />
							</span>
							<header class="major">
								<h1>Tonatico</h1>
							</header>
							<div class="content">
								<p>Es uno de los pocos lugares que reúnen bellezas naturales, monumentos históricos y tradiciones ancestrales.</p>
							</div>
						</div>
					</section>
				<!-- Main -->
					<div id="main">
						<!-- One -->
							<section id="one">
								<div class="inner">
									<header class="major">
										<h2>Actividades a realizar:</h2>
									</header>

									<!-- Form -->				

						    <form method="post" action="#">
							<div class="row gtr-uniform">										
								<!-- Break -->													
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico1" value="2">
									<input type="checkbox" id="Tonatico1" name="Tonatico1" value="1">
									<label for="Tonatico1">Usar el GPS de X-Trail para llegar a tu destino</label>
								</div>
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico2" value="2">
									<input type="checkbox" id="Tonatico2" name="Tonatico2" value="1" >
									<label for="Tonatico2">Ir al Parque del Sol a admirar el paisaje/ cascada del salto</label>
								</div>			
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico3" value="2">
									<input type="checkbox" id="Tonatico3" name="Tonatico3" value="1">
									<label for="Tonatico3">Caminar por el zócalo</label>
								</div>
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico4" value="2">
									<input type="checkbox" id="Tonatico4" name="Tonatico4" value="1">
									<label for="Tonatico4">Probar un helado en la Heladería La Michoacana</label>
								</div>				
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico5" value="2">
									<input type="checkbox" id="Tonatico5" name="Tonatico5" value="1">
									<label for="Tonatico5">Conocer la Iglesia de Nuestra señora de Tonatico</label>
								</div>		
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico6" value="2">
									<input type="checkbox" id="Tonatico6" name="Tonatico6" value="1">
									<label for="Tonatico6">Probar la sopa de hongo en el restaurante del “Amigo Toño”</label>
								</div>		
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico7" value="2">
									<input type="checkbox" id="Tonatico7" name="Tonatico7" value="1">
									<label for="Tonatico7">Probar la sopa de hongo en el restaurante del “Amigo Toño”</label>
								</div>
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico8" value="2">
									<input type="checkbox" id="Tonatico8" name="Tonatico8" value="1">
									<label for="Tonatico8">Usar la detección del punto ciego mientras manejas”</label>
								</div>
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico9" value="2">
									<input type="checkbox" id="Tonatico9" name="Tonatico9" value="1">
									<label for="Tonatico9">Tomarte una cerveza en Los Tarros</label>
								</div>
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico10" value="2">
									<input type="checkbox" id="Tonatico10" name="Tonatico10" value="1">
									<label for="Tonatico10">Usar las funciones de Intelligent Mobility </label>
								</div>
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico11" value="2">
									<input type="checkbox" id="Tonatico11" name="Tonatico11" value="1">
									<label for="Tonatico11">Descubrir las Grutas de la Estrella </label>
								</div>			
								<div class="col-6 col-12-small">
									<input type="checkbox" id="Tonatico12" name="Tonatico12" value="1">
									<label for="Tonatico12">Visitar el mercado</label>
								</div>	
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico13" value="2">
									<input type="checkbox" id="Tonatico13" name="Tonatico13" value="1">
									<label for="Tonatico13">Desayunar chilaquiles en el restaurante de la señora Lilia </label>
								</div>	
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico14" value="2">
									<input type="checkbox" id="Tonatico14" name="Tonatico14" value="1">
									<label for="Tonatico14">Probar una cerveza en el Bar Chequer (junto al restaurante de la sra. Lilia)</label>
								</div>	
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico15" value="2">
									<input type="checkbox" id="Tonatico15" name="Tonatico15" value="1">
									<label for="Tonatico15">Probar un platillo típico en Los Portales de la sra. Rebeca</label>
								</div>	
								<div class="col-6 col-12-small">
									<input type="hidden"  name="tonatico16" value="2">
									<input type="checkbox" id="Tonatico16" name="Tonatico16" value="1">
									<label for="Tonatico16">Usa el Intelligent Cruise  Control X-Trail en la carretera?</label>
								</div>	

															<!-- Break -->
								<div class="col-12">
									<ul class="actions">
								<li><input type="submit" value="Enviar Cambios" class="primary" /></li>
																	
								</ul>
								</div>
								</div>
								<br><br><iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15107.31776078416!2d-99.67632177233031!3d18.805752908187916!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85cdbba5344ab2c7%3A0x38e0de82cc25a78a!2zVG9uYXRpY28sIE3DqXgu!5e0!3m2!1ses-419!2smx!4v1547244052995" width="350" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>
						</form>
					</div>
			</section>




						
				<!-- Footer -->
					<footer id="footer">
						<div class="inner">
							<ul class="icons">
								<li><a href="#" class="icon alt fa-twitter"><span class="label">Twitter</span></a></li>
								<li><a href="#" class="icon alt fa-facebook"><span class="label">Facebook</span></a></li>
								<li><a href="#" class="icon alt fa-instagram"><span class="label">Instagram</span></a></li>
							</ul>
							<ul class="copyright">
								<li>&copy; TROOPSMX</li><li>NISSAN <a href="https://www.nissan.com.mx/x-trail/?gclid=Cj0KCQiAmuHhBRD0ARIsAFWyPwgqdbbVqRWOK6IfMeb81QyXejZ-BztsfSHXd4WHWy4Ch7ZzIRwqXhEaArr3EALw_wcB&gclsrc=aw.ds">X-TRAIL</a></li>
							</ul>
						</div>
					</footer>

			</div>

		<!-- Scripts -->
			<script src="assets/js/jquery.min.js"></script>
			<script src="assets/js/jquery.scrolly.min.js"></script>
			<script src="assets/js/jquery.scrollex.min.js"></script>
			<script src="assets/js/browser.min.js"></script>
			<script src="assets/js/breakpoints.min.js"></script>
			<script src="assets/js/util.js"></script>
			<script src="assets/js/main.js"></script>

	</body>


	<div class="content">
  	<!-- notification message -->
  	<?php if (isset($_SESSION['success'])) : ?>
      <div class="error success" >
      	<h3>
          <?php 
          	echo $_SESSION['success']; 
          	unset($_SESSION['success']);
          ?>
      	</h3>
      </div>
  	<?php endif ?>

    <!-- logged in user information -->
   
</div>
</html>
