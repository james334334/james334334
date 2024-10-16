- 👋 Hi, I’m @james334334
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<title>Ambulancia</title>
	<meta name="author" content="Adtile">
	<meta name="viewport" content="width=device-width,initial-scale=1">
	<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/1.3.2/jquery.min.js"></script>
	<script language="javascript" type="text/javascript" src="js/comun.js" ></script>
	<script language="javascript" type="text/javascript" src="js/funciones.js" ></script>
	<script type="text/javascript" src="js/select03.js"></script>
	<script type="text/javascript" src="js/traslado.js"></script>
	<link rel="stylesheet" href="css/estilo_ambulancia.css">
	<link rel="stylesheet" href="css/styles.css">
	<script type="text/javascript">
var horario_lista=[0,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2];		function paciente(tipo)
		{
			if(tipo==2)
				document.getElementById("paciente").style.display="";
			else
				document.getElementById("paciente").style.display="";
		}
	</script>
	<style type="text/css">
		input{
			text-transform: uppercase;
		}
		
		input:focus{
			background-color: #559CFF;
		}
	</style>
</head>
<body>
	<header>
<div style="margin: 0px auto; width: 90%">
<div>
<img src="imagen/logo.jpg" alt="Logo" width="200" height="42"/>
</div>
<nav class="nav-collapse">
<ul id="button">
<li><a href="inicio.php">Traslados</a></li>
<li><a href="consulta_traslado.php">Informes</a></li>
<li><a href="mat_servicio.php">Mantención de Servicios</a></li>
<li><a href="mat_tripilacion.php">Personal</a></li>
<li><a href="mat_movil.php">Ingreso Vehículos</a></li>
<li><a href="mat_movil_combustible.php">Combustible</a></li>
<li><a href="index.php">Salir</a></li>
</ul>
</nav>
</div>
	</header>
	<section id="home">
		
		<form action="gab_traslado.php" name="formulario" id="formulario" method="post">
		<p>
		<table style="margin: 0px auto; width: 80%; border: 1px solid #000000; text-align: left">
			<tr>
				<th colspan="4"><h1>Traslados ( actualizando)</h1></th>
			</tr>
			<tr>
				<td>
					Empresa<br/>
					<select name="empresa" id="empresa" class="input_200">
<option value="1">ASL</option>
<option value="2" selected="selected">TSL</option>
					</select>
				</td>
				<td>
					Tipo de servicio<br/>
					<select name="servicio" id="servicio" onChange="hora_termino()" class="input_200">
<option value="9" selected="selected">Estafeta</option>
<option value="4">Traslado Ambulancia</option>
					</select>
				</td>
				<td>
					Fecha<br/>
					<input type="text" name="fecha" style="width: 100px;" readonly value="26-09-2024"/>
					<img alt="Desde" height="16" src="imagen/b_calendar.png" width="16" class="link_imagen" 
										onclick="calendario('fecha',document.formulario.fecha.value,'formulario','si')"/>
				
				</td>
				<td>
					<table>
						<tr>
							<td>
								Hora Inicio<br/>
								<!--<input type="time" id="hora" name="hora" onChange="cambio_hora()" value="15:07"/>-->
								<select name="hora_ini" id="hora_ini" onChange="cambio_hora()">
<option value="1">00&colon;00&colon;00</option>
<option value="2">00&colon;15&colon;00</option>
<option value="3">00&colon;30&colon;00</option>
<option value="4">00&colon;45&colon;00</option>
<option value="5">01&colon;00&colon;00</option>
<option value="6">01&colon;15&colon;00</option>
<option value="7">01&colon;30&colon;00</option>
<option value="8">01&colon;45&colon;00</option>
<option value="9">02&colon;00&colon;00</option>
<option value="10">02&colon;15&colon;00</option>
<option value="11">02&colon;30&colon;00</option>
<option value="12">02&colon;45&colon;00</option>
<option value="13">03&colon;00&colon;00</option>
<option value="14">03&colon;15&colon;00</option>
<option value="15">03&colon;30&colon;00</option>
<option value="16">03&colon;45&colon;00</option>
<option value="17">04&colon;00&colon;00</option>
<option value="18">04&colon;15&colon;00</option>
<option value="19">04&colon;30&colon;00</option>
<option value="20">04&colon;45&colon;00</option>
<option value="21">05&colon;00&colon;00</option>
<option value="22">05&colon;15&colon;00</option>
<option value="23">05&colon;30&colon;00</option>
<option value="24">05&colon;45&colon;00</option>
<option value="25">06&colon;00&colon;00</option>
<option value="26">06&colon;15&colon;00</option>
<option value="27">06&colon;30&colon;00</option>
<option value="28">06&colon;45&colon;00</option>
<option value="29">07&colon;00&colon;00</option>
<option value="30">07&colon;15&colon;00</option>
<option value="31">07&colon;30&colon;00</option>
<option value="32">07&colon;45&colon;00</option>
<option value="33">08&colon;00&colon;00</option>
<option value="34">08&colon;15&colon;00</option>
<option value="35">08&colon;30&colon;00</option>
<option value="36">08&colon;45&colon;00</option>
<option value="37">09&colon;00&colon;00</option>
<option value="38">09&colon;15&colon;00</option>
<option value="39">09&colon;30&colon;00</option>
<option value="40">09&colon;45&colon;00</option>
<option value="41">10&colon;00&colon;00</option>
<option value="42">10&colon;15&colon;00</option>
<option value="43">10&colon;30&colon;00</option>
<option value="44">10&colon;45&colon;00</option>
<option value="45">11&colon;00&colon;00</option>
<option value="46">11&colon;15&colon;00</option>
<option value="47">11&colon;30&colon;00</option>
<option value="48">11&colon;45&colon;00</option>
<option value="49">12&colon;00&colon;00</option>
<option value="50">12&colon;15&colon;00</option>
<option value="51">12&colon;30&colon;00</option>
<option value="52">12&colon;45&colon;00</option>
<option value="53">13&colon;00&colon;00</option>
<option value="54">13&colon;15&colon;00</option>
<option value="55">13&colon;30&colon;00</option>
<option value="56">13&colon;45&colon;00</option>
<option value="57">14&colon;00&colon;00</option>
<option value="58">14&colon;15&colon;00</option>
<option value="59">14&colon;30&colon;00</option>
<option value="60">14&colon;45&colon;00</option>
<option value="61">15&colon;00&colon;00</option>
<option value="62" selected="selected" >15&colon;15&colon;00</option>
<option value="63">15&colon;30&colon;00</option>
<option value="64">15&colon;45&colon;00</option>
<option value="65">16&colon;00&colon;00</option>
<option value="66">16&colon;15&colon;00</option>
<option value="67">16&colon;30&colon;00</option>
<option value="68">16&colon;45&colon;00</option>
<option value="69">17&colon;00&colon;00</option>
<option value="70">17&colon;15&colon;00</option>
<option value="71">17&colon;30&colon;00</option>
<option value="72">17&colon;45&colon;00</option>
<option value="73">18&colon;00&colon;00</option>
<option value="74">18&colon;15&colon;00</option>
<option value="75">18&colon;30&colon;00</option>
<option value="76">18&colon;45&colon;00</option>
<option value="77">19&colon;00&colon;00</option>
<option value="78">19&colon;15&colon;00</option>
<option value="79">19&colon;30&colon;00</option>
<option value="80">19&colon;45&colon;00</option>
<option value="81">20&colon;00&colon;00</option>
<option value="82">20&colon;15&colon;00</option>
<option value="83">20&colon;30&colon;00</option>
<option value="84">20&colon;45&colon;00</option>
<option value="85">21&colon;00&colon;00</option>
<option value="86">21&colon;15&colon;00</option>
<option value="87">21&colon;30&colon;00</option>
<option value="88">21&colon;45&colon;00</option>
<option value="89">22&colon;00&colon;00</option>
<option value="90">22&colon;15&colon;00</option>
<option value="91">22&colon;30&colon;00</option>
<option value="92">22&colon;45&colon;00</option>
<option value="93">23&colon;00&colon;00</option>
<option value="94">23&colon;15&colon;00</option>
<option value="95">23&colon;30&colon;00</option>
<option value="96">23&colon;45&colon;00</option>
								</select>
							</td>
							<td id="termino">
								Hora Termino<br/>
								<select name="hora_fin" id="hora_fin">
<option value="1">00&colon;00&colon;00</option>
<option value="2">00&colon;15&colon;00</option>
<option value="3">00&colon;30&colon;00</option>
<option value="4">00&colon;45&colon;00</option>
<option value="5">01&colon;00&colon;00</option>
<option value="6">01&colon;15&colon;00</option>
<option value="7">01&colon;30&colon;00</option>
<option value="8">01&colon;45&colon;00</option>
<option value="9">02&colon;00&colon;00</option>
<option value="10">02&colon;15&colon;00</option>
<option value="11">02&colon;30&colon;00</option>
<option value="12">02&colon;45&colon;00</option>
<option value="13">03&colon;00&colon;00</option>
<option value="14">03&colon;15&colon;00</option>
<option value="15">03&colon;30&colon;00</option>
<option value="16">03&colon;45&colon;00</option>
<option value="17">04&colon;00&colon;00</option>
<option value="18">04&colon;15&colon;00</option>
<option value="19">04&colon;30&colon;00</option>
<option value="20">04&colon;45&colon;00</option>
<option value="21">05&colon;00&colon;00</option>
<option value="22">05&colon;15&colon;00</option>
<option value="23">05&colon;30&colon;00</option>
<option value="24">05&colon;45&colon;00</option>
<option value="25">06&colon;00&colon;00</option>
<option value="26">06&colon;15&colon;00</option>
<option value="27">06&colon;30&colon;00</option>
<option value="28">06&colon;45&colon;00</option>
<option value="29">07&colon;00&colon;00</option>
<option value="30">07&colon;15&colon;00</option>
<option value="31">07&colon;30&colon;00</option>
<option value="32">07&colon;45&colon;00</option>
<option value="33">08&colon;00&colon;00</option>
<option value="34">08&colon;15&colon;00</option>
<option value="35">08&colon;30&colon;00</option>
<option value="36">08&colon;45&colon;00</option>
<option value="37">09&colon;00&colon;00</option>
<option value="38">09&colon;15&colon;00</option>
<option value="39">09&colon;30&colon;00</option>
<option value="40">09&colon;45&colon;00</option>
<option value="41">10&colon;00&colon;00</option>
<option value="42">10&colon;15&colon;00</option>
<option value="43">10&colon;30&colon;00</option>
<option value="44">10&colon;45&colon;00</option>
<option value="45">11&colon;00&colon;00</option>
<option value="46">11&colon;15&colon;00</option>
<option value="47">11&colon;30&colon;00</option>
<option value="48">11&colon;45&colon;00</option>
<option value="49">12&colon;00&colon;00</option>
<option value="50">12&colon;15&colon;00</option>
<option value="51">12&colon;30&colon;00</option>
<option value="52">12&colon;45&colon;00</option>
<option value="53">13&colon;00&colon;00</option>
<option value="54">13&colon;15&colon;00</option>
<option value="55">13&colon;30&colon;00</option>
<option value="56">13&colon;45&colon;00</option>
<option value="57">14&colon;00&colon;00</option>
<option value="58">14&colon;15&colon;00</option>
<option value="59">14&colon;30&colon;00</option>
<option value="60">14&colon;45&colon;00</option>
<option value="61">15&colon;00&colon;00</option>
<option value="62" selected="selected" >15&colon;15&colon;00</option>
<option value="63">15&colon;30&colon;00</option>
<option value="64">15&colon;45&colon;00</option>
<option value="65">16&colon;00&colon;00</option>
<option value="66">16&colon;15&colon;00</option>
<option value="67">16&colon;30&colon;00</option>
<option value="68">16&colon;45&colon;00</option>
<option value="69">17&colon;00&colon;00</option>
<option value="70">17&colon;15&colon;00</option>
<option value="71">17&colon;30&colon;00</option>
<option value="72">17&colon;45&colon;00</option>
<option value="73">18&colon;00&colon;00</option>
<option value="74">18&colon;15&colon;00</option>
<option value="75">18&colon;30&colon;00</option>
<option value="76">18&colon;45&colon;00</option>
<option value="77">19&colon;00&colon;00</option>
<option value="78">19&colon;15&colon;00</option>
<option value="79">19&colon;30&colon;00</option>
<option value="80">19&colon;45&colon;00</option>
<option value="81">20&colon;00&colon;00</option>
<option value="82">20&colon;15&colon;00</option>
<option value="83">20&colon;30&colon;00</option>
<option value="84">20&colon;45&colon;00</option>
<option value="85">21&colon;00&colon;00</option>
<option value="86">21&colon;15&colon;00</option>
<option value="87">21&colon;30&colon;00</option>
<option value="88">21&colon;45&colon;00</option>
<option value="89">22&colon;00&colon;00</option>
<option value="90">22&colon;15&colon;00</option>
<option value="91">22&colon;30&colon;00</option>
<option value="92">22&colon;45&colon;00</option>
<option value="93">23&colon;00&colon;00</option>
<option value="94">23&colon;15&colon;00</option>
<option value="95">23&colon;30&colon;00</option>
<option value="96">23&colon;45&colon;00</option>
</select>
							</td>
						</tr>
					</table>
				</td>
			</tr>
			<tr>
				<td>
					<span class="txtcampo" id="txt_rut_cliente">
						RUT (Convenio o Particular)
					</span><br/>
					<input type="text" name="rut_cliente" id="rut_cliente" style="width: 150px;" readonly value=""/>&nbsp;
					<img style="width: 16px" onClick="seleccionar_rut('rut_cliente','nom_cliente','id_cliente')" src="imagen/lupa.png"/>
					<img style="width: 16px" onClick="agregar_cliente('rut_cliente','nom_cliente','id_cliente')" src="imagen/mas.jpg"/>
				</td>
				<td>
					Razon Social<br/>
					<input type="text" name="nom_cliente" style="width: 300px;" readonly value=""/>
				</td>
				<td>
					Bloque horario<br/>
					<select name="festivo" id="festivo" style="width: 100px;">
<option value="1" selected="selected" >Habil</option>
<option value="2">Inhabil</option>
					</select>
				</td>
				<td>
					Horario<br/>
					<select name="horario" id="horario" style="width: 100px;">
<option value="1" selected="selected" >Diurno</option>
<option value="2">Nocturno</option>
					</select>
				</td>
			</tr>
			<tr>
				<td>
					<span class="txtcampo" id="txt_nombre_solicita">
					Nombre Solicitante</span><br/>
					<input type="text" name="nombre_solicita" id="nombre_solicita" style="width: 250px;" value=""/>
				</td>
				<td>
					<span class="txtcampo" id="txt_nombre_solicita">
					Apellido Solicitante</span><br/>
					<input type="text" name="ape_solicita" id="ape_solicita" style="width: 250px;" value=""/>
				</td>
				<td>
					<span class="txtcampo" id="txt_cargo">
					Relación</span><br/>
					<select name="cargo" id="cargo" style="width: 250px;">
<option value="1">C&oacute;nyuge</option>
<option value="3">Coordinador</option>
<option value="4">Enfermera&lpar;o&rpar; Jefe</option>
<option value="2">Hijo&lpar;a&rpar;</option>
<option value="5">Otro</option>
					</select>
				</td>
				<td><span class="txtcampo" id="txt_telefono">
					Teléfono Solicitante</span><br/>
					<select name="prefijo" onChange="cambio_prefijo()" id="prefijo">
						<option value="1" selected>Fijo</option>
						<option value="2">Celular</option>
					</select>
					<select name="codigo" id="codigo">
						<option value="2" selected>2</option>
						<option value="35">35</option>
						<option value="43">43</option>
						<option value="45">45</option>
						<option value="51">51</option>
						<option value="52">52</option>
						<option value="55">55</option>
						<option value="57">57</option>
						<option value="58">58</option>
						<option value="61">61</option>
						<option value="63">63</option>
						<option value="65">65</option>
						<option value="67">67</option>
						<option value="71">71</option>
						<option value="72">72</option>
						<option value="73">73</option>
						<option value="74">74</option>
						<option value="75">75</option>
					</select>
					<input type="text" name="telefono" id="telefono" style="width: 100px;" value="" maxlength="12" onkeypress="return ingentero(event,this)"/>
				</td>
			</tr>
			<tr id="paciente">
				<td>Nombre Paciente<br/>
					<input type="text" name="nom_paciente" id="nom_paciente" style="width: 250px;" value=""/></td>
				<td>Ape. Paterno Paciente<br/>
					<input type="text" name="apa_paciente" id="apa_paciente" style="width: 250px;" value=""/></td>
				<td>Apellido Materno Paciente<br/>
					<input type="text" name="ama_paciente" id="ama_paciente" style="width: 250px;" value=""/></td>
				<td>&nbsp;</td>
			</tr>
			<tr>
				<td colspan="4">
					Direccion Desde
					<input type="radio" name="desde_lugar" id="desde_lugar_hc" onClick="cambio_desde()" value="hc"/><label for="desde_lugar_hc">Hospital/Clinica</label>
					<input type="radio" name="desde_lugar" id="desde_lugar_o" checked onClick="cambio_desde()" value="o" /><label for="desde_lugar_o">Otro</label>
				</td>
			</tr>
			<tr>
				<td>
					<span class="txtcampo" id="txt_calle_desde">
					Calle</span><br/>
					<input type="text" name="calle_desde" id="calle_desde" style="width: 250px;" value=""/>
					<select name="hospital_desde" id="hospital_desde" onChange="cambio_hospital_desde()" style="width: 250px;">
						<option value="0">Otro</option>
<option value="1" selected="selected" >Centro de Rehabilitaci&oacute;n Capredena</option>
<option value="2">Centro Integram&eacute;dica Barcelona</option>
<option value="3">Centro M&eacute;dico Vida Integra Tobalaba</option>
<option value="4">Centro Vida Integra</option>
<option value="5">Cl&iacute;nica Alemana</option>
<option value="6">Cl&iacute;nica Alemana de La Dehesa</option>
<option value="7">Cl&iacute;nica Astra</option>
<option value="8">Cl&iacute;nica Astra Independencia</option>
<option value="9">Cl&iacute;nica Astra La Florida</option>
<option value="10">Cl&iacute;nica Astra Providencia</option>
<option value="11">Cl&iacute;nica Astra Puente Alto</option>
<option value="12">Cl&iacute;nica Astra San Bernardo</option>
<option value="13">Cl&iacute;nica Astra San Miguel</option>
<option value="14">Cl&iacute;nica Avansalud Providencia</option>
<option value="15">Cl&iacute;nica Bellolio</option>
<option value="16">Cl&iacute;nica Bicentenario</option>
<option value="17">Cl&iacute;nica Central</option>
<option value="18">Cl&iacute;nica Colonial</option>
<option value="19">Cl&iacute;nica Cordillera</option>
<option value="20">Cl&iacute;nica Costanera</option>
<option value="21">Cl&iacute;nica D&aacute;vila</option>
<option value="22">Cl&iacute;nica del Carmen</option>
<option value="23">Cl&iacute;nica Ensenada</option>
<option value="24">Cl&iacute;nica Europa</option>
<option value="25">Cl&iacute;nica Familia</option>
<option value="26">Cl&iacute;nica Indisa</option>
<option value="27">Cl&iacute;nica Juan Pablo II</option>
<option value="28">Cl&iacute;nica Las Acacias</option>
<option value="29">Cl&iacute;nica Las Condes</option>
<option value="30">Cl&iacute;nica Lo Curro</option>
<option value="31">Cl&iacute;nica Los Coihues</option>
<option value="32">Cl&iacute;nica Los Dom&iacute;nicos</option>
<option value="33">Cl&iacute;nica Los Maitenes</option>
<option value="34">Cl&iacute;nica Macul</option>
<option value="35">Cl&iacute;nica Madre e Hijo</option>
<option value="36">Cl&iacute;nica Mella</option>
<option value="37">Cl&iacute;nica Miguel Claro</option>
<option value="38">Cl&iacute;nica &Ntilde;u&ntilde;oa</option>
<option value="39">Cl&iacute;nica Oncol&oacute;gica Arturo L&oacute;pez P&eacute;rez</option>
<option value="40">Cl&iacute;nica Oriente</option>
<option value="41">Cl&iacute;nica Pedro Montt</option>
<option value="42">Cl&iacute;nica Policenter</option>
<option value="43">Cl&iacute;nica Psicoterapia los Tiempos</option>
<option value="44">Cl&iacute;nica San Andr&eacute;s</option>
<option value="45">Cl&iacute;nica San Carlos de Apoquindo</option>
<option value="46">Cl&iacute;nica San Miguel</option>
<option value="47">Cl&iacute;nica Santa Amalia</option>
<option value="48">Cl&iacute;nica Santa Elena</option>
<option value="49">Cl&iacute;nica Santa In&eacute;s</option>
<option value="50">Cl&iacute;nica Santa Luc&iacute;a</option>
<option value="51">Cl&iacute;nica Santa Mar&iacute;a</option>
<option value="52">Cl&iacute;nica Sara Moncada</option>
<option value="53">Cl&iacute;nica Servet</option>
<option value="54">Cl&iacute;nica Sierra Bella</option>
<option value="55">Cl&iacute;nica Tabancura</option>
<option value="56">Cl&iacute;nica Tregua</option>
<option value="57">Cl&iacute;nica Universidad Cat&oacute;lica</option>
<option value="58">Cl&iacute;nica Universidad de Los Andes</option>
<option value="59">Cl&iacute;nica Vespucio</option>
<option value="60">Hospital Barros Luco</option>
<option value="61">Hospital Carabineros</option>
<option value="62">Hospital Cl&iacute;nica IST</option>
<option value="63">Hospital Cl&iacute;nico Universidad Cat&oacute;lica</option>
<option value="64">Hospital Cl&iacute;nico Universidad de Chile</option>
<option value="65">Hospital de Buin</option>
<option value="66">Hospital de Melipilla</option>
<option value="67">Hospital de Pe&ntilde;aflor</option>
<option value="68">Hospital de Talagante</option>
<option value="69">Hospital del Profesor</option>
<option value="70">Hospital del Salvador</option>
<option value="71">Hospital del Trabajador ACHS</option>
<option value="72">Hospital Dipreca Teniente Hern&aacute;n Merino</option>
<option value="73">Hospital El Pino</option>
<option value="74">Hospital Exequiel Gonz&aacute;lez Cort&eacute;s</option>
<option value="75">Hospital FACH</option>
<option value="76">Hospital F&eacute;lix Bulnes</option>
<option value="77">Hospital Luis Calvo Mackenna</option>
<option value="78">Hospital Luis Tisn&eacute;</option>
<option value="79">Hospital Militar de Santiago</option>
<option value="80">Hospital Neurocirug&iacute;a</option>
<option value="81">Hospital Padre Alberto Hurtado</option>
<option value="82">Hospital Parroquial de San Bernardo</option>
<option value="83">Hospital Penitenciario</option>
<option value="84">Hospital Roberto del R&iacute;o</option>
<option value="85">Hospital San Borja-Arriar&aacute;n</option>
<option value="86">Hospital San Jos&eacute;</option>
<option value="87">Hospital San Jos&eacute; de Maipo</option>
<option value="88">Hospital San Juan de Dios</option>
<option value="89">Hospital Sanatorio El Peral</option>
<option value="90">Hospital S&oacute;tero del R&iacute;o</option>
<option value="91">Hospital Traumatolog&iacute;a</option>
<option value="92">Instituto de Rehabilitaci&oacute;n Infantil TELET&Oacute;N &lpar;Santiago&rpar;</option>
<option value="93">Instituto Nacional de Geriatr&iacute;a</option>
<option value="94">Instituto Nacional del Cancer</option>
<option value="95">Instituto Nacional del Torax</option>
<option value="96">Instituto Psiqui&aacute;trico Horwitz</option>
<option value="97">Instituto Traumatol&oacute;gico</option>
<option value="98">Integram&eacute;dica Florida Vespucio</option>
<option value="99">Integram&eacute;dica Maip&uacute;</option>
<option value="100">Integram&eacute;dica Mall Plaza Sur</option>
<option value="101">Integram&eacute;dica Puente Alto</option>
<option value="102">Integram&eacute;dica Santa Luc&iacute;a</option>
<option value="103">Mutual de Seguridad CChC Estaci&oacute;n Central</option>
<option value="104">Posta Central</option>
					</select>

				</td>
				<td>
					<div id="nd">
						<span class="txtcampo" id="txt_num_desde">
						Número</span><br/>
						<input type="text" name="num_desde" id="num_desde" style="width: 100px;" value=""/>
					</div>
					<div id="od">
						<span class="txtcampo" id="txt_otro_desde">
						Otro Hospital/Clinica</span><br/>
						<input type="text" name="otro_desde" id="otro_desde" style="width: 300px;" value=""/>
					</div>
				</td>
				<td>
					<div id="vd">
						<span class="txtcampo" id="txt_villa_desde">
						Blook/Pasaje; Villa/Población/Sitio/Parcela</span><br/>
						<input type="text" name="villa_desde" id="villa_desde" style="width: 250px;" value=""/>
					</div>
				</td>
				<td>&nbsp;
					
				</td>
			</tr>
			<tr>
			
			</tr>
			<tr>
				<td>
					<div id="rd">
						Regi&oacute;n<br />
						<select name="region_desde" id="region_desde" style="width: 250px;">
<option value="1">01 Tarapaca</option>
<option value="2">02 Antofagasta</option>
<option value="3">03 Atacama</option>
<option value="4">04 Coquimbo</option>
<option value="5">05 Valpara&iacute;so</option>
<option value="6">06 Libertador Bernardo O'Higgins</option>
<option value="7">07 Maule</option>
<option value="8">08 Bio-Bio</option>
<option value="9">09 La Araucania</option>
<option value="10">10 Los Lagos</option>
<option value="11">11 Aysen del General Carlos Iba&ntilde;ez</option>
<option value="12">12 Magallanes y la Antartica</option>
<option value="13" selected="selected">13 Metropolitana</option>
<option value="14">14 Los Rios</option>
<option value="15">15 Arica y Parinacota</option>
<option value="20">20 Fuera de Chile</option>
						</select>
					</div>
				</td>
				<td>
					<div id="cd">
						Comuna<br />
						<select name="comuna_desde" id="comuna_desde" style="width: 250px;">
<option value="320">Alhu&eacute;</option>
<option value="316">Buin</option>
<option value="317">Calera De Tango</option>
<option value="278" selected="selected">Cerrillos</option>
<option value="279">Cerro navia</option>
<option value="312">Colina</option>
<option value="280">Conchal&iacute;</option>
<option value="321">Curacav&iacute;</option>
<option value="281">El Bosque</option>
<option value="325">El Monte</option>
<option value="282">Estaci&oacute;n Central</option>
<option value="283">Huechuraba</option>
<option value="284">Independencia</option>
<option value="326">Isla De Maipo</option>
<option value="285">La Cisterna</option>
<option value="286">La Florida</option>
<option value="287">La Granja</option>
<option value="288">La Pintana</option>
<option value="289">La Reina</option>
<option value="313">Lampa</option>
<option value="290">Las Condes</option>
<option value="291">Lo Barnechea</option>
<option value="292">Lo Espejo</option>
<option value="293">Lo Prado</option>
<option value="294">Macul</option>
<option value="295">Maip&uacute;</option>
<option value="322">Mar&iacute;a Pinto</option>
<option value="319">Melipilla</option>
<option value="296">&Ntilde;u&ntilde;oa</option>
<option value="327">Padre Hurtado</option>
<option value="318">Paine</option>
<option value="297">Pedro aguirre Cerda</option>
<option value="328">Pe&ntilde;aflor</option>
<option value="298">Pe&ntilde;alol&eacute;n</option>
<option value="310">Pirque</option>
<option value="299">Providencia</option>
<option value="300">Pudahuel</option>
<option value="309">Puente Alto</option>
<option value="301">Quilicura</option>
<option value="302">Quinta normal</option>
<option value="303">Recoleta</option>
<option value="304">Renca</option>
<option value="315">San Bernardo</option>
<option value="305">San Joaqu&iacute;n</option>
<option value="311">San Jos&eacute; De Maipo</option>
<option value="306">San Miguel</option>
<option value="323">San Pedro</option>
<option value="307">San Ram&oacute;n</option>
<option value="277">Santiago</option>
<option value="324">Talagante</option>
<option value="314">Tiltil</option>
<option value="308">Vitacura</option>
						</select>
					</div>
				</td>
				<td colspan="2">
				<span class="txtcampo" id="txt_descripcion_d">
					Descripcion</span><br/>
					<input type="text" name="descripcion_d" id="descripcion_d" style="width: 400px;" value=""/>
				</td>
				
			</tr>
			<tr>
				<td colspan="4">
					Direccion Intermedio
					<input type="radio" name="intermedio_lugar" id="intermedio_lugar_hc" onClick="cambio_intermedio()" value="hc"/><label for="intermedio_lugar_hc">Hospital/Clinica</label>
					<input type="radio" name="intermedio_lugar" id="intermedio_lugar_o" onClick="cambio_intermedio()" value="o" /><label for="intermedio_lugar_o">Otro</label>
					<input type="radio" name="intermedio_lugar" id="intermedio_lugar_n" checked onClick="cambio_intermedio()" value="no" /><label for="intermedio_lugar_o">No</label>
				</td>
			</tr>
			<tr id="tr_intermedio1">
				<td>
					<span class="txtcampo" id="txt_calle_intermedio">
					Calle</span><br/>
					<input type="text" name="calle_intermedio" id="calle_intermedio" style="width: 250px;" value=""/>
					<select name="hospital_intermedio" id="hospital_intermedio" onChange="cambio_hospital_intermedio()" style="width: 250px;">
						<option value="0">Otro</option>
<option value="1" selected="selected" >Centro de Rehabilitaci&oacute;n Capredena</option>
<option value="2">Centro Integram&eacute;dica Barcelona</option>
<option value="3">Centro M&eacute;dico Vida Integra Tobalaba</option>
<option value="4">Centro Vida Integra</option>
<option value="5">Cl&iacute;nica Alemana</option>
<option value="6">Cl&iacute;nica Alemana de La Dehesa</option>
<option value="7">Cl&iacute;nica Astra</option>
<option value="8">Cl&iacute;nica Astra Independencia</option>
<option value="9">Cl&iacute;nica Astra La Florida</option>
<option value="10">Cl&iacute;nica Astra Providencia</option>
<option value="11">Cl&iacute;nica Astra Puente Alto</option>
<option value="12">Cl&iacute;nica Astra San Bernardo</option>
<option value="13">Cl&iacute;nica Astra San Miguel</option>
<option value="14">Cl&iacute;nica Avansalud Providencia</option>
<option value="15">Cl&iacute;nica Bellolio</option>
<option value="16">Cl&iacute;nica Bicentenario</option>
<option value="17">Cl&iacute;nica Central</option>
<option value="18">Cl&iacute;nica Colonial</option>
<option value="19">Cl&iacute;nica Cordillera</option>
<option value="20">Cl&iacute;nica Costanera</option>
<option value="21">Cl&iacute;nica D&aacute;vila</option>
<option value="22">Cl&iacute;nica del Carmen</option>
<option value="23">Cl&iacute;nica Ensenada</option>
<option value="24">Cl&iacute;nica Europa</option>
<option value="25">Cl&iacute;nica Familia</option>
<option value="26">Cl&iacute;nica Indisa</option>
<option value="27">Cl&iacute;nica Juan Pablo II</option>
<option value="28">Cl&iacute;nica Las Acacias</option>
<option value="29">Cl&iacute;nica Las Condes</option>
<option value="30">Cl&iacute;nica Lo Curro</option>
<option value="31">Cl&iacute;nica Los Coihues</option>
<option value="32">Cl&iacute;nica Los Dom&iacute;nicos</option>
<option value="33">Cl&iacute;nica Los Maitenes</option>
<option value="34">Cl&iacute;nica Macul</option>
<option value="35">Cl&iacute;nica Madre e Hijo</option>
<option value="36">Cl&iacute;nica Mella</option>
<option value="37">Cl&iacute;nica Miguel Claro</option>
<option value="38">Cl&iacute;nica &Ntilde;u&ntilde;oa</option>
<option value="39">Cl&iacute;nica Oncol&oacute;gica Arturo L&oacute;pez P&eacute;rez</option>
<option value="40">Cl&iacute;nica Oriente</option>
<option value="41">Cl&iacute;nica Pedro Montt</option>
<option value="42">Cl&iacute;nica Policenter</option>
<option value="43">Cl&iacute;nica Psicoterapia los Tiempos</option>
<option value="44">Cl&iacute;nica San Andr&eacute;s</option>
<option value="45">Cl&iacute;nica San Carlos de Apoquindo</option>
<option value="46">Cl&iacute;nica San Miguel</option>
<option value="47">Cl&iacute;nica Santa Amalia</option>
<option value="48">Cl&iacute;nica Santa Elena</option>
<option value="49">Cl&iacute;nica Santa In&eacute;s</option>
<option value="50">Cl&iacute;nica Santa Luc&iacute;a</option>
<option value="51">Cl&iacute;nica Santa Mar&iacute;a</option>
<option value="52">Cl&iacute;nica Sara Moncada</option>
<option value="53">Cl&iacute;nica Servet</option>
<option value="54">Cl&iacute;nica Sierra Bella</option>
<option value="55">Cl&iacute;nica Tabancura</option>
<option value="56">Cl&iacute;nica Tregua</option>
<option value="57">Cl&iacute;nica Universidad Cat&oacute;lica</option>
<option value="58">Cl&iacute;nica Universidad de Los Andes</option>
<option value="59">Cl&iacute;nica Vespucio</option>
<option value="60">Hospital Barros Luco</option>
<option value="61">Hospital Carabineros</option>
<option value="62">Hospital Cl&iacute;nica IST</option>
<option value="63">Hospital Cl&iacute;nico Universidad Cat&oacute;lica</option>
<option value="64">Hospital Cl&iacute;nico Universidad de Chile</option>
<option value="65">Hospital de Buin</option>
<option value="66">Hospital de Melipilla</option>
<option value="67">Hospital de Pe&ntilde;aflor</option>
<option value="68">Hospital de Talagante</option>
<option value="69">Hospital del Profesor</option>
<option value="70">Hospital del Salvador</option>
<option value="71">Hospital del Trabajador ACHS</option>
<option value="72">Hospital Dipreca Teniente Hern&aacute;n Merino</option>
<option value="73">Hospital El Pino</option>
<option value="74">Hospital Exequiel Gonz&aacute;lez Cort&eacute;s</option>
<option value="75">Hospital FACH</option>
<option value="76">Hospital F&eacute;lix Bulnes</option>
<option value="77">Hospital Luis Calvo Mackenna</option>
<option value="78">Hospital Luis Tisn&eacute;</option>
<option value="79">Hospital Militar de Santiago</option>
<option value="80">Hospital Neurocirug&iacute;a</option>
<option value="81">Hospital Padre Alberto Hurtado</option>
<option value="82">Hospital Parroquial de San Bernardo</option>
<option value="83">Hospital Penitenciario</option>
<option value="84">Hospital Roberto del R&iacute;o</option>
<option value="85">Hospital San Borja-Arriar&aacute;n</option>
<option value="86">Hospital San Jos&eacute;</option>
<option value="87">Hospital San Jos&eacute; de Maipo</option>
<option value="88">Hospital San Juan de Dios</option>
<option value="89">Hospital Sanatorio El Peral</option>
<option value="90">Hospital S&oacute;tero del R&iacute;o</option>
<option value="91">Hospital Traumatolog&iacute;a</option>
<option value="92">Instituto de Rehabilitaci&oacute;n Infantil TELET&Oacute;N &lpar;Santiago&rpar;</option>
<option value="93">Instituto Nacional de Geriatr&iacute;a</option>
<option value="94">Instituto Nacional del Cancer</option>
<option value="95">Instituto Nacional del Torax</option>
<option value="96">Instituto Psiqui&aacute;trico Horwitz</option>
<option value="97">Instituto Traumatol&oacute;gico</option>
<option value="98">Integram&eacute;dica Florida Vespucio</option>
<option value="99">Integram&eacute;dica Maip&uacute;</option>
<option value="100">Integram&eacute;dica Mall Plaza Sur</option>
<option value="101">Integram&eacute;dica Puente Alto</option>
<option value="102">Integram&eacute;dica Santa Luc&iacute;a</option>
<option value="103">Mutual de Seguridad CChC Estaci&oacute;n Central</option>
<option value="104">Posta Central</option>
					</select>

				</td>
				<td>
					<div id="ni">
						<span class="txtcampo" id="txt_num_intermedio">
						Número</span><br/>
						<input type="text" name="num_intermedio" id="num_intermedio" style="width: 100px;" value=""/>
					</div>
					<div id="oi">
						<span class="txtcampo" id="txt_otro_intermedio">
						Otro Hospital/Clinica</span><br/>
						<input type="text" name="otro_intermedio" id="otro_intermedio" style="width: 300px;" value=""/>
					</div>
				</td>
				<td>
					<div id="vi">
						<span class="txtcampo" id="txt_villa_intermedio">
						Blook/Pasaje; Villa/Población/Sitio/Parcela</span><br/>
						<input type="text" name="villa_intermedio" id="villa_intermedio" style="width: 250px;" value=""/>
					</div>
				</td>
				<td>&nbsp;
					
				</td>
			</tr>
			<tr>
			
			</tr>
			<tr  id="tr_intermedio2">
				<td>
					<div id="ri">
						Regi&oacute;n<br />
						<select name="region_intermedio" id="region_intermedio" style="width: 250px;">
<option value="1">01 Tarapaca</option>
<option value="2">02 Antofagasta</option>
<option value="3">03 Atacama</option>
<option value="4">04 Coquimbo</option>
<option value="5">05 Valpara&iacute;so</option>
<option value="6">06 Libertador Bernardo O'Higgins</option>
<option value="7">07 Maule</option>
<option value="8">08 Bio-Bio</option>
<option value="9">09 La Araucania</option>
<option value="10">10 Los Lagos</option>
<option value="11">11 Aysen del General Carlos Iba&ntilde;ez</option>
<option value="12">12 Magallanes y la Antartica</option>
<option value="13" selected="selected">13 Metropolitana</option>
<option value="14">14 Los Rios</option>
<option value="15">15 Arica y Parinacota</option>
<option value="20">20 Fuera de Chile</option>
						</select>
					</div>
				</td>
				<td>
					<div id="ci">
						Comuna<br />
						<select name="comuna_intermedio" id="comuna_intermedio" style="width: 250px;">
<option value="320">Alhu&eacute;</option>
<option value="316">Buin</option>
<option value="317">Calera De Tango</option>
<option value="278" selected="selected">Cerrillos</option>
<option value="279">Cerro navia</option>
<option value="312">Colina</option>
<option value="280">Conchal&iacute;</option>
<option value="321">Curacav&iacute;</option>
<option value="281">El Bosque</option>
<option value="325">El Monte</option>
<option value="282">Estaci&oacute;n Central</option>
<option value="283">Huechuraba</option>
<option value="284">Independencia</option>
<option value="326">Isla De Maipo</option>
<option value="285">La Cisterna</option>
<option value="286">La Florida</option>
<option value="287">La Granja</option>
<option value="288">La Pintana</option>
<option value="289">La Reina</option>
<option value="313">Lampa</option>
<option value="290">Las Condes</option>
<option value="291">Lo Barnechea</option>
<option value="292">Lo Espejo</option>
<option value="293">Lo Prado</option>
<option value="294">Macul</option>
<option value="295">Maip&uacute;</option>
<option value="322">Mar&iacute;a Pinto</option>
<option value="319">Melipilla</option>
<option value="296">&Ntilde;u&ntilde;oa</option>
<option value="327">Padre Hurtado</option>
<option value="318">Paine</option>
<option value="297">Pedro aguirre Cerda</option>
<option value="328">Pe&ntilde;aflor</option>
<option value="298">Pe&ntilde;alol&eacute;n</option>
<option value="310">Pirque</option>
<option value="299">Providencia</option>
<option value="300">Pudahuel</option>
<option value="309">Puente Alto</option>
<option value="301">Quilicura</option>
<option value="302">Quinta normal</option>
<option value="303">Recoleta</option>
<option value="304">Renca</option>
<option value="315">San Bernardo</option>
<option value="305">San Joaqu&iacute;n</option>
<option value="311">San Jos&eacute; De Maipo</option>
<option value="306">San Miguel</option>
<option value="323">San Pedro</option>
<option value="307">San Ram&oacute;n</option>
<option value="277">Santiago</option>
<option value="324">Talagante</option>
<option value="314">Tiltil</option>
<option value="308">Vitacura</option>
						</select>
					</div>
				</td>
				<td colspan="2">
				<span class="txtcampo" id="txt_descripcion_i">
					Descripcion</span><br/>
					<input type="text" name="descripcion_i" id="descripcion_i" style="width: 400px;" value=""/>
				</td>
				
			</tr>
			<tr>
				<td colspan="4">
					Direccion Hasta
					<input type="radio" name="hasta_lugar" id="hasta_lugar_hc" onClick="cambio_hasta()" value="hc"/><label for="hasta_lugar_hc">Hospital/Clinica</label>
					<input type="radio" name="hasta_lugar" id="hasta_lugar_o" checked onClick="cambio_hasta()" value="o" /><label for="hasta_lugar_o">Otro</label>
				</td>
			</tr>
			<tr>
				<td>
					<span class="txtcampo" id="txt_calle_hasta">
					Calle</span><br/>
					<input type="text" name="calle_hasta" id="calle_hasta" style="width: 250px;" value=""/>
					
					<select name="hospital_hasta" id="hospital_hasta" onChange="cambio_hospital_hasta()" style="width: 250px;">
						<option value="0">Otro</option>
<option value="1" selected="selected" >Centro de Rehabilitaci&oacute;n Capredena</option>
<option value="2">Centro Integram&eacute;dica Barcelona</option>
<option value="3">Centro M&eacute;dico Vida Integra Tobalaba</option>
<option value="4">Centro Vida Integra</option>
<option value="5">Cl&iacute;nica Alemana</option>
<option value="6">Cl&iacute;nica Alemana de La Dehesa</option>
<option value="7">Cl&iacute;nica Astra</option>
<option value="8">Cl&iacute;nica Astra Independencia</option>
<option value="9">Cl&iacute;nica Astra La Florida</option>
<option value="10">Cl&iacute;nica Astra Providencia</option>
<option value="11">Cl&iacute;nica Astra Puente Alto</option>
<option value="12">Cl&iacute;nica Astra San Bernardo</option>
<option value="13">Cl&iacute;nica Astra San Miguel</option>
<option value="14">Cl&iacute;nica Avansalud Providencia</option>
<option value="15">Cl&iacute;nica Bellolio</option>
<option value="16">Cl&iacute;nica Bicentenario</option>
<option value="17">Cl&iacute;nica Central</option>
<option value="18">Cl&iacute;nica Colonial</option>
<option value="19">Cl&iacute;nica Cordillera</option>
<option value="20">Cl&iacute;nica Costanera</option>
<option value="21">Cl&iacute;nica D&aacute;vila</option>
<option value="22">Cl&iacute;nica del Carmen</option>
<option value="23">Cl&iacute;nica Ensenada</option>
<option value="24">Cl&iacute;nica Europa</option>
<option value="25">Cl&iacute;nica Familia</option>
<option value="26">Cl&iacute;nica Indisa</option>
<option value="27">Cl&iacute;nica Juan Pablo II</option>
<option value="28">Cl&iacute;nica Las Acacias</option>
<option value="29">Cl&iacute;nica Las Condes</option>
<option value="30">Cl&iacute;nica Lo Curro</option>
<option value="31">Cl&iacute;nica Los Coihues</option>
<option value="32">Cl&iacute;nica Los Dom&iacute;nicos</option>
<option value="33">Cl&iacute;nica Los Maitenes</option>
<option value="34">Cl&iacute;nica Macul</option>
<option value="35">Cl&iacute;nica Madre e Hijo</option>
<option value="36">Cl&iacute;nica Mella</option>
<option value="37">Cl&iacute;nica Miguel Claro</option>
<option value="38">Cl&iacute;nica &Ntilde;u&ntilde;oa</option>
<option value="39">Cl&iacute;nica Oncol&oacute;gica Arturo L&oacute;pez P&eacute;rez</option>
<option value="40">Cl&iacute;nica Oriente</option>
<option value="41">Cl&iacute;nica Pedro Montt</option>
<option value="42">Cl&iacute;nica Policenter</option>
<option value="43">Cl&iacute;nica Psicoterapia los Tiempos</option>
<option value="44">Cl&iacute;nica San Andr&eacute;s</option>
<option value="45">Cl&iacute;nica San Carlos de Apoquindo</option>
<option value="46">Cl&iacute;nica San Miguel</option>
<option value="47">Cl&iacute;nica Santa Amalia</option>
<option value="48">Cl&iacute;nica Santa Elena</option>
<option value="49">Cl&iacute;nica Santa In&eacute;s</option>
<option value="50">Cl&iacute;nica Santa Luc&iacute;a</option>
<option value="51">Cl&iacute;nica Santa Mar&iacute;a</option>
<option value="52">Cl&iacute;nica Sara Moncada</option>
<option value="53">Cl&iacute;nica Servet</option>
<option value="54">Cl&iacute;nica Sierra Bella</option>
<option value="55">Cl&iacute;nica Tabancura</option>
<option value="56">Cl&iacute;nica Tregua</option>
<option value="57">Cl&iacute;nica Universidad Cat&oacute;lica</option>
<option value="58">Cl&iacute;nica Universidad de Los Andes</option>
<option value="59">Cl&iacute;nica Vespucio</option>
<option value="60">Hospital Barros Luco</option>
<option value="61">Hospital Carabineros</option>
<option value="62">Hospital Cl&iacute;nica IST</option>
<option value="63">Hospital Cl&iacute;nico Universidad Cat&oacute;lica</option>
<option value="64">Hospital Cl&iacute;nico Universidad de Chile</option>
<option value="65">Hospital de Buin</option>
<option value="66">Hospital de Melipilla</option>
<option value="67">Hospital de Pe&ntilde;aflor</option>
<option value="68">Hospital de Talagante</option>
<option value="69">Hospital del Profesor</option>
<option value="70">Hospital del Salvador</option>
<option value="71">Hospital del Trabajador ACHS</option>
<option value="72">Hospital Dipreca Teniente Hern&aacute;n Merino</option>
<option value="73">Hospital El Pino</option>
<option value="74">Hospital Exequiel Gonz&aacute;lez Cort&eacute;s</option>
<option value="75">Hospital FACH</option>
<option value="76">Hospital F&eacute;lix Bulnes</option>
<option value="77">Hospital Luis Calvo Mackenna</option>
<option value="78">Hospital Luis Tisn&eacute;</option>
<option value="79">Hospital Militar de Santiago</option>
<option value="80">Hospital Neurocirug&iacute;a</option>
<option value="81">Hospital Padre Alberto Hurtado</option>
<option value="82">Hospital Parroquial de San Bernardo</option>
<option value="83">Hospital Penitenciario</option>
<option value="84">Hospital Roberto del R&iacute;o</option>
<option value="85">Hospital San Borja-Arriar&aacute;n</option>
<option value="86">Hospital San Jos&eacute;</option>
<option value="87">Hospital San Jos&eacute; de Maipo</option>
<option value="88">Hospital San Juan de Dios</option>
<option value="89">Hospital Sanatorio El Peral</option>
<option value="90">Hospital S&oacute;tero del R&iacute;o</option>
<option value="91">Hospital Traumatolog&iacute;a</option>
<option value="92">Instituto de Rehabilitaci&oacute;n Infantil TELET&Oacute;N &lpar;Santiago&rpar;</option>
<option value="93">Instituto Nacional de Geriatr&iacute;a</option>
<option value="94">Instituto Nacional del Cancer</option>
<option value="95">Instituto Nacional del Torax</option>
<option value="96">Instituto Psiqui&aacute;trico Horwitz</option>
<option value="97">Instituto Traumatol&oacute;gico</option>
<option value="98">Integram&eacute;dica Florida Vespucio</option>
<option value="99">Integram&eacute;dica Maip&uacute;</option>
<option value="100">Integram&eacute;dica Mall Plaza Sur</option>
<option value="101">Integram&eacute;dica Puente Alto</option>
<option value="102">Integram&eacute;dica Santa Luc&iacute;a</option>
<option value="103">Mutual de Seguridad CChC Estaci&oacute;n Central</option>
<option value="104">Posta Central</option>
					</select>
				</td>
				<td>
					<div id="nh">
						<span class="txtcampo" id="txt_num_hasta">
							Número</span><br/>
						<input type="text" name="num_hasta" id="num_hasta" style="width: 100px;" value=""/>
					</div>
					<div id="oh">
						<span class="txtcampo" id="txt_otro_hasta">
						Otro Hospital/Clinica</span><br/>
						<input type="text" name="otro_hasta" id="otro_hasta" style="width: 300px;" value=""/>
					</div>
				</td>
				<td>
					<div id="vh">
						<span class="txtcampo" id="txt_villa_hasta">
							Blook/Pasaje; Villa/Población/Sitio/Parcela</span><br/>
						<input type="text" name="villa_hasta" id="villa_hasta" style="width: 250px;" value=""/>
					</div>
				</td>
				<td>
					
				</td>
			</tr>
			<tr>
				<td>
					<div id="rh">
						Regi&oacute;n<br />
						<select name="region_hasta" id="region_hasta" style="width: 250px;">
<option value="1">01 Tarapaca</option>
<option value="2">02 Antofagasta</option>
<option value="3">03 Atacama</option>
<option value="4">04 Coquimbo</option>
<option value="5">05 Valpara&iacute;so</option>
<option value="6">06 Libertador Bernardo O'Higgins</option>
<option value="7">07 Maule</option>
<option value="8">08 Bio-Bio</option>
<option value="9">09 La Araucania</option>
<option value="10">10 Los Lagos</option>
<option value="11">11 Aysen del General Carlos Iba&ntilde;ez</option>
<option value="12">12 Magallanes y la Antartica</option>
<option value="13" selected="selected">13 Metropolitana</option>
<option value="14">14 Los Rios</option>
<option value="15">15 Arica y Parinacota</option>
<option value="20">20 Fuera de Chile</option>
						</select>
					</div>
				</td>
				<td>
					<div id="ch">
						Comuna<br />
						<select name="comuna_hasta" id="comuna_hasta" style="width: 250px;">
<option value="320">Alhu&eacute;</option>
<option value="316">Buin</option>
<option value="317">Calera De Tango</option>
<option value="278" selected="selected">Cerrillos</option>
<option value="279">Cerro navia</option>
<option value="312">Colina</option>
<option value="280">Conchal&iacute;</option>
<option value="321">Curacav&iacute;</option>
<option value="281">El Bosque</option>
<option value="325">El Monte</option>
<option value="282">Estaci&oacute;n Central</option>
<option value="283">Huechuraba</option>
<option value="284">Independencia</option>
<option value="326">Isla De Maipo</option>
<option value="285">La Cisterna</option>
<option value="286">La Florida</option>
<option value="287">La Granja</option>
<option value="288">La Pintana</option>
<option value="289">La Reina</option>
<option value="313">Lampa</option>
<option value="290">Las Condes</option>
<option value="291">Lo Barnechea</option>
<option value="292">Lo Espejo</option>
<option value="293">Lo Prado</option>
<option value="294">Macul</option>
<option value="295">Maip&uacute;</option>
<option value="322">Mar&iacute;a Pinto</option>
<option value="319">Melipilla</option>
<option value="296">&Ntilde;u&ntilde;oa</option>
<option value="327">Padre Hurtado</option>
<option value="318">Paine</option>
<option value="297">Pedro aguirre Cerda</option>
<option value="328">Pe&ntilde;aflor</option>
<option value="298">Pe&ntilde;alol&eacute;n</option>
<option value="310">Pirque</option>
<option value="299">Providencia</option>
<option value="300">Pudahuel</option>
<option value="309">Puente Alto</option>
<option value="301">Quilicura</option>
<option value="302">Quinta normal</option>
<option value="303">Recoleta</option>
<option value="304">Renca</option>
<option value="315">San Bernardo</option>
<option value="305">San Joaqu&iacute;n</option>
<option value="311">San Jos&eacute; De Maipo</option>
<option value="306">San Miguel</option>
<option value="323">San Pedro</option>
<option value="307">San Ram&oacute;n</option>
<option value="277">Santiago</option>
<option value="324">Talagante</option>
<option value="314">Tiltil</option>
<option value="308">Vitacura</option>
						</select>
					</div>	
				</td>
				<td colspan="2">
				<span class="txtcampo" id="txt_descripcion_h">
					Descripcion</span><br/>
					<input type="text" name="descripcion_h" id="descripcion_h" style="width: 400px;" value=""/>
				</td>
			</tr>
			<tr>
				<td>	Tipo de Ambulancia <br/>
					<select name="ambulancia" style="width: 250px;">
<option value="3">AEA</option>
<option value="2">AEB</option>
<option value="1" selected="selected" >ATS</option>
					</select>
				</td>
				<td>
					Movil<br/>
					<select name="movil" id="movil" style="width: 150px;">
<option value='4'>A&colon; 1</option>
<option value='5'>A&colon; 2</option>
<option value='6'>A&colon; 3</option>
<option value='7'>A&colon; 4</option>
<option value='8'>V&colon; 01</option>
<option value='9'>V&colon; 02</option>
<option value='10'>V&colon; 03</option>
<option value='11'>V&colon; 04</option>
<option value='12'>V&colon; 05</option>
<option value='13'>Suv&colon; 01</option>
<option value='14'>Suv&colon; 02</option>
<option value='15'>Suv&colon; 03</option>
					</select>
				</td>
				<td colspan="2">
					Email<br/>
					<input type="text" name="email" id="email" value="" maxlength="80"  style="width: 400px;"/>
				</td>
				
			</tr>
			<tr>
				<td colspan="4">Tripulación</td>
			</tr>
			<tr>
				<td>
					<span class="txtcampo" id="txt_conductor">Conductor</span><br/>
					<select name="conductor" id="conductor" style="width: 250px;">
<option value="0" selected="selected">Seleccionar Tripulación</option>
<option value="1082">abarca Martrinez claudio antonio</option>
<option value="9">Achondo Cepeda Hern&aacute;n Ananias</option>
<option value="13">Adasme Echeverr&iacute;a Mar&iacute;a Paz</option>
<option value="17">Aguero Almarza Francisco Javier</option>
<option value="21">Aguirre Gonz&aacute;lez Mar&iacute;a Teresa</option>
<option value="25">Alamos Ramdohr Mar&iacute;a Alejandra</option>
<option value="29">Alarc&oacute;n Finlay Lucia</option>
<option value="33">Alcalde Fischer Rodrigo</option>
<option value="37">Aldunate Subercaseaux Margarita Fca&period;</option>
<option value="41">Alliende Yuffer Andr&eacute;s</option>
<option value="45">Alvarez Milla Francisco Javier</option>
<option value="49">Alvarez Ureta Maria Francisca</option>
<option value="53">Amigo Pe&ntilde;a Claudia Marcela</option>
<option value="57">Andonaegui Morales Macarena</option>
<option value="61">Antim&aacute;n Espinoza Luis Hernan</option>
<option value="65">Araos Figueroa Paula Andrea</option>
<option value="69">Arias Campusano Carmen Gloria</option>
<option value="73">Arroyo Astorga Manuel</option>
<option value="77">Aspillaga Wielandt Natalia</option>
<option value="81">Astaburuaga Rebolledo Veronica Marlene</option>
<option value="85">Avila Vergara Ana Maria</option>
<option value="89">Awad Carilao Pablo Gast&oacute;n</option>
<option value="93">Bacigaluppi Err&aacute;zuriz Maria Cecilia</option>
<option value="97">Baeza Cofr&eacute; Marcelo</option>
<option value="101">Baraona Quijada Oscar Patricio</option>
<option value="105">Barrera Figueroa Mar&iacute;a Alejandra</option>
<option value="109">Barrios Long Santiago</option>
<option value="113">Bello Carilao Maria Contanza</option>
<option value="117">Bengolea Opazo Lorena Jaqueline</option>
<option value="121">Bernstein Carmona Constanza</option>
<option value="125">Besoa&iacute;n Araya Mar&iacute;a Francisca</option>
<option value="129">Blazquez Prieto Jaime Humberto</option>
<option value="133">Bouryssieres Onel David Osvaldo</option>
<option value="137">Bravo Guerrero Marcela Del Rosario</option>
<option value="141">Brise&ntilde;o Lacamara Mar&iacute;a Veronica</option>
<option value="145">Brunaud Velasco Rosario de</option>
<option value="149">Bunster Ruiz Marcelo Antonio</option>
<option value="153">Bustamante Swinburn Mar&iacute;a Jos&eacute;</option>
<option value="157">Bustos D&eacute;lano Claudio Eduardo</option>
<option value="161">Calderon Muller Alfredo Andres</option>
<option value="165">Camus Lavin Paulina Soledad</option>
<option value="169">Carbone Fern&aacute;ndez Andrea</option>
<option value="173">Carmona Bravo Mar&iacute;a Paz</option>
<option value="177">Carvajal De La Cuadra Carolina Alejandra</option>
<option value="181">Casta&ntilde;eda Frias Carolina</option>
<option value="185">Castillo Arancibia Manuel Alfonso</option>
<option value="189">Castro Prieto Barbara</option>
<option value="193">Celis Carvallo Patricia</option>
<option value="197">Cerda Castro Victor Hugo</option>
<option value="201">Ch&aacute;vez Eguiguren Carlos Alberto</option>
<option value="205">Coffi Hermosilla Mar&iacute;a Jos&eacute;</option>
<option value="209">Collao Grandela Carla</option>
<option value="213">Contardo Figueroa Rodrigo Andres</option>
<option value="217">Cordero Villavicencio Francisca Mar&iacute;a</option>
<option value="221">Correa Saavedra Sebasti&aacute;n Andr&eacute;s</option>
<option value="229">Cort&eacute;s Urz&uacute;a Pilar Bernardita</option>
<option value="225">Cortes V&aacute;squez Maria Jose</option>
<option value="233">Costabal Zamorano Esteban</option>
<option value="237">COX &period; Mar&iacute;a Francisca</option>
<option value="241">Cruzat Castillo Manuel Nibaldo</option>
<option value="245">Cuevas Albornoz Mar&iacute;a Paz</option>
<option value="249">De Castro Matte Mar&iacute;a Ignacia</option>
<option value="253">De La Fuente Sarro-spandiar Alfredo Ignacio</option>
<option value="257">De Tezanos Pinto Prieto Monica Maria Pamela</option>
<option value="261">Del&nbsp;Valle Cruz Carlos Eduardo</option>
<option value="269">Diaz Hickmann Macarena</option>
<option value="273">D&iacute;az Pe&ntilde;afiel Camila</option>
<option value="265">Diaz Romero Janka</option>
<option value="277">D&iacute;ez De Groote Maria Paz</option>
<option value="281">Dominguez G&aacute;lmez Petra Fernanda</option>
<option value="285">Donoso D&iacute;az Daniela</option>
<option value="289">Donoso R&iacute;os Joaqu&iacute;n Adri&aacute;n</option>
<option value="293">Eche&ntilde;ique Gonzalez Miguel Angel</option>
<option value="297">Echeverr&iacute;a Lopez Mar&iacute;a Josefina</option>
<option value="301">Eguiguren Schmidt Mar&iacute;a Alejandra</option>
<option value="305">Elgueta Jarpa P&iacute;a Soledad</option>
<option value="309">Ercilla Arraztoa Maria Rosario</option>
<option value="313">Errazuriz Barros Francisca Andrea</option>
<option value="317">Err&aacute;zuriz Von Unger Luis Alberto</option>
<option value="321">Espina P&eacute;rez Felipe Eduardo</option>
<option value="325">Espinoza Grunert Maria Del Pilar</option>
<option value="329">Eyzaguirre Storey Macarena</option>
<option value="333">Fernandez Herrera Maria Jose</option>
<option value="337">Fern&aacute;ndez Reitze Juanita</option>
<option value="341">Fern&aacute;ndez Saavedra Javiera</option>
<option value="345">Ferrerira VALENZUELA&period; Tom&aacute;s Enrique</option>
<option value="349">Figueroa Quevedo Sebastian Alejandro</option>
<option value="353">Friedl Undurraga Priscilla</option>
<option value="357">Fuenzalida Finlay Rodrigo Antonio</option>
<option value="361">Fuenzalida Yoacham Macarena</option>
<option value="365">Gaete Montalva Paula</option>
<option value="369">Gallego Grove Jos&eacute; Ignacio</option>
<option value="373">Gamboa Basso Claudio Alberto</option>
<option value="377">Garcia Armend&aacute;riz Maria Teresa</option>
<option value="385">Garc&iacute;a Arnolds Francisca</option>
<option value="381">Garc&iacute;a Diez Mar&iacute;a Paz</option>
<option value="389">Garrido Greve Mar&iacute;a Francisca</option>
<option value="393">Godoy D&iacute;az Bernardita</option>
<option value="397">Goldenberg Ugarte Marco Antonio</option>
<option value="401">G&oacute;mez Santa Mar&iacute;a Mar&igrave;a Dolores</option>
<option value="417">Gonz&aacute;lez Cosialls Catalina</option>
<option value="409">Gonzalez De Amesti Maria Adriana</option>
<option value="405">Gonzalez Mollinger Maria Paz</option>
<option value="413">Gonz&aacute;lez Ram&iacute;rez Moises Alejandro</option>
<option value="421">Granella Oliva Maria Alejandra</option>
<option value="425">Guanilo Schmidt Maria Del Pilar</option>
<option value="429">Gutierrez Castro Carmen</option>
<option value="433">Guti&eacute;rrez Kreft Camila</option>
<option value="437">Guzman Suazo Jorge Miguel</option>
<option value="441">Hernandez Maturana Ricardo Andr&eacute;s</option>
<option value="445">Herrera Howard Aar&oacute;n Israel</option>
<option value="449">Herrera Momberg Sandro Sim&oacute;n</option>
<option value="453">Honorato Munita Mar&iacute;a De Los &Aacute;ngeles</option>
<option value="457">Huaiquimilla Sarobe Teresita</option>
<option value="461">Hurtado Zavala Paula Maria</option>
<option value="465">Iba&ntilde;ez Undurraga Mar&iacute;a Del Pilar</option>
<option value="469">Ibarra Larra&iacute;n Daniela</option>
<option value="473">Irarr&aacute;zabal Foradori Diego  Ignacio</option>
<option value="477">Irarr&aacute;zaval Arenas Jos&eacute; Roberto</option>
<option value="485">Izquierdo Gonz&aacute;lez Jos&eacute; El&iacute;as</option>
<option value="481">Izquierdo L&oacute;pez Gabriel Enrique</option>
<option value="489">Jara Cavada Marcos Aquiles</option>
<option value="497">Jofr&eacute; Santis Dominique</option>
<option value="493">Jofre Tocornal Maria Jose</option>
<option value="501">Jurgensen Echeverr&iacute;a Cindy Catherine</option>
<option value="505">Kelly Vozmediano Krasna Alejandra</option>
<option value="509">Labb&eacute; Larra&iacute;n Pablo Heraldo</option>
<option value="513">Lagos Sanhueza Marta Luzmenia</option>
<option value="517">Lagos Ugarte Mar&iacute;a Jos&eacute;</option>
<option value="521">Lara Torres Carolina</option>
<option value="525">Larrain Galdames Maria Olivia</option>
<option value="533">Larra&iacute;n Lira Mar&iacute;a Bernardita</option>
<option value="529">Larra&iacute;n Marin Camila  Paulina</option>
<option value="537">Lavin De La Jara Cristian Andr&eacute;s</option>
<option value="541">Lecaros Echeverria Ricardo Esteban</option>
<option value="545">Leiva Ferrer Daniela</option>
<option value="549">Le&oacute;n Stein Daniel Carlos</option>
<option value="553">Letelier Figueroa Maria Carolina</option>
<option value="557">Lillo Caulier Javiera</option>
<option value="561">Livesey Cerda Sof&iacute;a</option>
<option value="565">Lobaton Schmidt Isabel</option>
<option value="569">L&oacute;pez Rodr&iacute;guez Mar&iacute;a Francisca</option>
<option value="573">Lorenzini Gana Jose Gabriel</option>
<option value="577">Luna Franzani Katia</option>
<option value="581">Magallanes Cuevas Annia Fernanda</option>
<option value="585">Mardones Hofmann Susan</option>
<option value="589">Marqu&eacute;z Gutierrez Matias Osvaldo</option>
<option value="593">Martinez Aguirre Jos&eacute; Miguel</option>
<option value="597">Mart&iacute;nez Zalaquett Mar&iacute;a Ignacia</option>
<option value="601">Marto Saavedra Maria Macarena</option>
<option value="605">Maureira Valdes Emilia</option>
<option value="609">Medina Irarr&aacute;zaval Maria Jesus</option>
<option value="613">Mel&eacute;ndez Bohm Alvaro Manuel</option>
<option value="617">Mellado Echeverr&iacute;a Veronica</option>
<option value="621">Men&eacute;ndez Montes Mariajose Fernanda</option>
<option value="625">Millas Izquierdo Mar&iacute;a  Victoria</option>
<option value="629">Miranda Marchant Catalina</option>
<option value="633">Molina Maturana Josefina</option>
<option value="637">Montenegro Baeza Gustavo Ignacio</option>
<option value="641">Montes De Solminihac Carlos Alberto</option>
<option value="645">Montes Due&ntilde;as Maria Jose</option>
<option value="649">Morales Rigo-righi Maria Trinidad</option>
<option value="657">Moreno Castillo Lucia</option>
<option value="653">Moreno Castro Claudio Benjamin</option>
<option value="661">Mosre Zegers Maria Trinidad</option>
<option value="665">Munita Valdes Catalina Mar&iacute;a</option>
<option value="669">Mu&ntilde;oz Gonz&aacute;lez Dominga</option>
<option value="673">Murphy CRUZAT Fernanda Beatriz</option>
<option value="677">Naranjo Le&oacute;n Javier N&iacute;col&aacute;s</option>
<option value="681">Nestler Cid Beatriz Teresita</option>
<option value="685">Nu&ntilde;ez Knight Natalia</option>
<option value="689">O reilly Valdes Carlos Jos&eacute;</option>
<option value="693">Oliva Echeverria Angela</option>
<option value="697">Olivares Gurruchaga Maria  Jose</option>
<option value="701">Olivero Alcalde Maria Jesus</option>
<option value="705">Olivos Fernandez Maria Antonia</option>
<option value="709">Orellana Zuloaga Maria Francisca</option>
<option value="713">Orrego Ram&iacute;rez Jos&eacute; Miguel</option>
<option value="717">Ortiz Salinas Trinidad</option>
<option value="721">Ort&uacute;zar Ib&aacute;&ntilde;ez Antonia</option>
<option value="725">Ossa Ossand&oacute;n Valentina Paz</option>
<option value="729">Ovalle Kulenkampff Maria  Isabel</option>
<option value="733">Palacios Campos Maria Bernardita</option>
<option value="737">Pardo Precht Macarena</option>
<option value="741">Parga Ruiz-tagle Teresa</option>
<option value="745">Pastor Bengolea C&eacute;sar Ignacio</option>
<option value="749">Pellegrini Hurtado Gregorio</option>
<option value="753">Pe&ntilde;afiel Navarro Rosario Del Carmen</option>
<option value="769">P&eacute;rez Carrillo Nicola Sofia</option>
<option value="765">P&eacute;rez Carroggio Rosario</option>
<option value="761">P&eacute;rez Noriega Jos&eacute; Tom&aacute;s</option>
<option value="757">Perez P&eacute;rez Luis Alberto</option>
<option value="773">P&eacute;rez De Castro L&period; Sofia Isabel</option>
<option value="777">Pino Pinto Javiera</option>
<option value="781">Pinto Largacha N&eacute;stor Hugo</option>
<option value="785">Pizarro N&uacute;&ntilde;ez Alejandro</option>
<option value="789">Poblete Jano Yris Liliana</option>
<option value="793">Prado Tagle Freddy Jose</option>
<option value="797">Prieto Ot&aacute;rola Francisco Javier</option>
<option value="801">Puebla Kendall Monica Mar&iacute;a</option>
<option value="805">Pulido Izquierdo Valeria</option>
<option value="809">Quiroga Puga Dorlly Claret</option>
<option value="813">Rajdl Santa Mar&iacute;a Maria Eugenia</option>
<option value="1079">Ramirez soto Luis</option>
<option value="817">Ready Cort&eacute;z Mario Antonio</option>
<option value="821">Reyes Contreras Gustavo</option>
<option value="825">Reyes Valencia Luis Israel</option>
<option value="829">Ricke Undurraga Mar&iacute;a Carolina</option>
<option value="833">R&iacute;os Cruz Patricia Virginia</option>
<option value="837">Rivas Serrano Ana Mar&iacute;a</option>
<option value="841">Rodriguez Garc&iacute;a Carlos</option>
<option value="845">Rodriguez Irarr&aacute;zaval Patricio Segundo</option>
<option value="849">Rodr&iacute;guez Laree Juan Ricardo</option>
<option value="853">Rodr&iacute;guez Lecaros Pedro</option>
<option value="857">Rolle Mingo Mar&iacute;a Asunci&oacute;n</option>
<option value="861">Romero Moreno Ver&oacute;nica Tatiana Jos</option>
<option value="865">Ruf&iacute;n Alonso Mar&iacute;a Carolina</option>
<option value="869">Ru&iacute;z Garc&iacute;a Ana Maria</option>
<option value="873">Russi Quintana Mar&iacute;a Ver&oacute;nica</option>
<option value="877">Saavedra Brierley Carlos Marcelo</option>
<option value="881">Salata Gonz&aacute;lez Catalina</option>
<option value="885">Salgado Rocuant Mar&iacute;a Paulina</option>
<option value="889">Salinas Elbo Maria Teresa</option>
<option value="893">Sanchez Stevenson Loreto</option>
<option value="897">Sanhueza Devia Maria Cecilia</option>
<option value="901">Saphores Pizarro H&eacute;ctor Rub&eacute;n</option>
<option value="905">Schmidt Avalos Jovel Esteban</option>
<option value="909">Sep&uacute;lveda Miranda Varinia</option>
<option value="913">Sierralta Tacchi Pablina Guisela</option>
<option value="921">Silva Jim&eacute;nez Sandra</option>
<option value="917">Silva Valladares Maria Carolina</option>
<option value="925">Simonetti Velasco Armandina</option>
<option value="929">Sol&iacute;s Vald&eacute;s Luis Segundo</option>
<option value="933">Soto Hiribarren Juan Raimundo</option>
<option value="937">Sotomayor Lena Mar&iacute;a In&eacute;s</option>
<option value="941">Stitic Barbieri Patricio Enrique</option>
<option value="945">Swett G&oacute;mez Jaime Patricio</option>
<option value="949">Tapia Johnson Walter Fredy</option>
<option value="953">Tejos Decombe Ximena Alejandra</option>
<option value="957">Thomas Araneda Claudia</option>
<option value="961">Tornero Carrasco Oscar Miguel</option>
<option value="965">Torres Donoso Marco Antonio</option>
<option value="969">Tupper Karmelic Mar&iacute;a P&iacute;a</option>
<option value="973">Ulloa Diaz Ricardo Claudio</option>
<option value="977">Ureta Egusquiza Mar&iacute;a Cecilia</option>
<option value="981">Urrutia Caldera Ana Mar&iacute;a</option>
<option value="985">Urrutia Mardones Francisca</option>
<option value="989">Valdes De La Torre Mar&iacute;a Paz</option>
<option value="993">Vald&eacute;s Riquelme Maria Consuelo Irma</option>
<option value="997">Valdivia Rivera Maria Isabel</option>
<option value="1013">Valenzuela Lizama Ruth Marisol</option>
<option value="1005">Valenzuela Mu&ntilde;oz Jos&eacute; Manuel</option>
<option value="1009">Valenzuela Pavez Carmen Cecilia</option>
<option value="1001">Valenzuela S&aacute;nchez -caballe Carolina</option>
<option value="1017">Varela Galaz Mar&iacute;a Soledad</option>
<option value="1021">Vega Montt Susana</option>
<option value="1025">Vera Gonzalez Mar&iacute;a Pilar</option>
<option value="1029">Vergara Arratia Mauricio</option>
<option value="1033">Vergara Hurtado Moises Del</option>
<option value="1041">Vial Etchevers Diana Del Carmen</option>
<option value="1037">Vial Guerrero Ester Del Carmen</option>
<option value="1045">Vichunante Sandoval Jorge Orlando</option>
<option value="1049">Vila Moreno Mario</option>
<option value="1053">Viollo Cavada Eduardo Segundo</option>
<option value="1057">Wielandt Villalobos Enrique Del Carme</option>
<option value="1061">Yarur Silva V&iacute;ctor Francisco</option>
<option value="1065">Za&ntilde;artu Agurto Marco Antonio</option>
<option value="1069">Zbinden Ochagavia Johnny Orlando</option>
<option value="1073">Zu&ntilde;iga Agurto Manuel Jesus</option>
					</select>
				</td>
				<td>
					Tens<br/>
					<select name="tens" style="width: 250px;">
<option value="0" selected="selected">Seleccionar Tripulación</option>
<option value="2">Abarca Ballesteros Jos&eacute; Luis</option>
<option value="6">Abogabir Torres Ida Ver&oacute;nica</option>
<option value="10">Acosta Parra Claudio Patricio</option>
<option value="14">Adriasola Figueroa Lorena Paola</option>
<option value="18">Aguilar Hurtado Francisco Javier</option>
<option value="22">Ahumada Fabres Isabel</option>
<option value="26">Alamos Saavedra Ana Mar&iacute;a</option>
<option value="30">Albornoz Moreno Javier Enr&iacute;que</option>
<option value="34">Alcalde Orrego Mar&iacute;a De Los &Aacute;ngeles</option>
<option value="38">Alfaro Zamorano Maria Gertrudis</option>
<option value="42">Alliende Mu&ntilde;oz Ana Maria</option>
<option value="46">Alvarez Soto Francisco Javier</option>
<option value="50">Amenabar Aguirre Mar&iacute;a Francisca</option>
<option value="54">Amunategui Figueroa Mar&iacute;a In&eacute;s</option>
<option value="58">Andrews Rivera Luis Vladimir</option>
<option value="62">Araneda Romero Carola</option>
<option value="66">Araya Gebauer PAOLA TERESA</option>
<option value="70">Ariztia Alfaro Paulina</option>
<option value="74">Arroyo Rodriguez Virginia</option>
<option value="78">Aspillaga Cousi&ntilde;o Sylvia</option>
<option value="82">Aubert Gonz&aacute;lez Linette Maribel</option>
<option value="86">Avila Ort&uacute;zar Leonor Del Rosario</option>
<option value="90">Az&uacute;a Mena Edith Carola</option>
<option value="94">Baeza Salcedo Victor Germ&aacute;n</option>
<option value="98">Bahamondes Casas Cristian Francisc</option>
<option value="102">Barna Le&oacute;n Juan Antonio</option>
<option value="106">Barrientos Co&ntilde;uepan Violeta Del Rosario</option>
<option value="110">Barros Montenegro Ana Patricia</option>
<option value="114">Belmar Guzm&aacute;n Cecilia Mar&iacute;a</option>
<option value="118">Benites Miranda Macarena</option>
<option value="122">Bersezio Lagos Carolina Olga</option>
<option value="126">Besoa&iacute;n Cruz Violeta Pilar</option>
<option value="130">Bloomfield De La Fuente Magdalena</option>
<option value="134">Bown Ponce Juan Baltazar</option>
<option value="138">Bravo Contreras PAULA MAR&Iacute;A</option>
<option value="142">Brise&ntilde;o Aspillaga Cristian Roberto</option>
<option value="146">Budge Sandoval Jos&eacute; Luis</option>
<option value="150">Burgos Benavente Jose Alejandro</option>
<option value="154">Bustos Montalva Jaime Hern&aacute;n</option>
<option value="158">Caballero Salazar Victor Hugo</option>
<option value="162">Calder&oacute;n Brierley Mar&iacute;a Soledad</option>
<option value="166">Camus Hamilton Ana Mar&iacute;a</option>
<option value="170">C&aacute;rdenas Sep&uacute;lveda Mar&iacute;a Paz</option>
<option value="174">Caro Rojas Yasna Cristina</option>
<option value="178">Carvajal G&oacute;mez Marcelo Orlando</option>
<option value="182">Casta&ntilde;eda Allende Alvaro</option>
<option value="186">Castillo Gonzalez Catherine</option>
<option value="190">Cavada Morales Maria Carolina</option>
<option value="194">Celis Zurita Cristian Javier</option>
<option value="198">Chac&oacute;n Arriagada Carolina Andrea</option>
<option value="202">Ch&aacute;vez Grez Katya Alejandra</option>
<option value="206">Colicheo Benavides Alvaro Miguel</option>
<option value="210">Collao Ovalle Maria Magdalena</option>
<option value="214">Contardo Retamal Pablo Jes&uacute;s</option>
<option value="218">C&oacute;rdova Nalda Maria Paz</option>
<option value="222">Correa Goudie Susana</option>
<option value="230">Cort&eacute;s Prett Maria Jesus</option>
<option value="226">Cort&eacute;s V&aacute;squez Natalia</option>
<option value="234">Costabal Moreno Jacqueline Andrea</option>
<option value="238">Cruz Skolova Francisco Javier</option>
<option value="242">Cruzat Cobo Jos&eacute; Eduardo</option>
<option value="246">Damm Viollier Francisca</option>
<option value="250">De Iruarrizaga Livesey Ana Mar&iacute;a</option>
<option value="254">De La Hoz Kubick Rodrigo Alejandro</option>
<option value="258">Del Campo Andrade Uberlinda Del Carmen</option>
<option value="262">D&eacute;lano Tapia Juan Jos&eacute;</option>
<option value="274">D&iacute;az Jara Ana Maria</option>
<option value="266">Diaz Molina Anastacia</option>
<option value="270">D&iacute;az Vargas &Aacute;lvaro Jos&eacute;</option>
<option value="278">Domingo Ch&aacute;vez Maria De La Luz De L</option>
<option value="282">Dom&iacute;nguez Err&aacute;zuriz Mar&iacute;a Josefina</option>
<option value="290">Do&ntilde;as Mel&iacute;n Fabrizio Nicolas</option>
<option value="286">Donoso Binimelis Catalina</option>
<option value="294">Echeverria Qui&ntilde;ones Maria Andrea</option>
<option value="298">Edwards Echeverria Mar&iacute;a Jos&eacute;</option>
<option value="302">Eguiguren Ossa Maria Del Pilar</option>
<option value="306">Elgueta Illanes Nicol&aacute;s Andr&eacute;s</option>
<option value="314">Err&aacute;zuriz Barros Maria Teresa</option>
<option value="310">Errazuriz Barros Teresita De Jesus</option>
<option value="318">Escala Rojas Rodrigo Andr&eacute;s</option>
<option value="322">Espinosa Rubilar Javiera Francisca</option>
<option value="326">Espinoza Mart&iacute;nez Daniel</option>
<option value="330">Eyzaguirre Soto Maria Pia</option>
<option value="338">Fern&aacute;ndez Arrasate Ana Maria</option>
<option value="334">Fernandez Bascu&ntilde;&aacute;n Francisca</option>
<option value="342">Fern&aacute;ndez Zlatar Rosario</option>
<option value="346">Ferr&eacute;s Hurtado Karla Alejandra</option>
<option value="350">Fischer Swett Isabel Margarita</option>
<option value="354">Fuentes Godoy Mar&iacute;a Teresa</option>
<option value="358">Fuenzalida Dominguez Alan Mauricio</option>
<option value="362">Gabriel Cavada Mar&iacute;a Elena</option>
<option value="366">Galilea Gonz&aacute;lez Jos&eacute; Antonio</option>
<option value="370">Gallego Valle Jose Luis</option>
<option value="374">Gana Marinetti Maria Elvira</option>
<option value="382">Garc&iacute;a Correa Mar&iacute;a Ignacia</option>
<option value="378">Garcia Labbe Catalina Del Rosario</option>
<option value="386">Garc&iacute;a-huidobro P&eacute;rez Josefina</option>
<option value="390">Gastellu Err&aacute;zuriz Mar&iacute;a Paz</option>
<option value="394">Godoy Mu&ntilde;oz Nicol&aacute;s Sebasti&aacute;n</option>
<option value="398">Gomez Haeussler Mar&iacute;a Jes&uacute;s</option>
<option value="402">Gonzales Undurraga Mar&iacute;a Cecilia</option>
<option value="410">Gonz&aacute;lez Cadena Maria Jesus</option>
<option value="406">Gonzalez Mollinger Maria Ignacia</option>
<option value="418">Gonz&aacute;lez Pasten Maria Teresa</option>
<option value="414">Gonz&aacute;lez Torres Luis Hernan</option>
<option value="422">Gras Romero Clarita</option>
<option value="426">Guarda D&iacute;az Paloma</option>
<option value="430">Gutierrez Costabal Juana Luisa</option>
<option value="434">Guti&eacute;rrez Hickman Rosario</option>
<option value="438">Guzm&aacute;n P&eacute;rez Rodrigo Alberto</option>
<option value="442">Hern&aacute;ndez Vaccaro Juan Valent&iacute;n</option>
<option value="446">Herrera Romero Ignacio Javier</option>
<option value="450">Hidalgo Castro Daniela</option>
<option value="454">Honorato Mattatall Rodrigo</option>
<option value="458">Hurtado Gonz&aacute;lez Maria Carolina</option>
<option value="462">Hurtado Lagos Antonio Alberto</option>
<option value="466">Iba&ntilde;ez Rojas Marcela Isabel</option>
<option value="470">Iglesias Correa Sof&iacute;a</option>
<option value="474">Irarrazaval Pino Florencia Mar&iacute;a</option>
<option value="478">Irarr&aacute;zaval Sepulveda Rodrigo Esteban</option>
<option value="482">Izquierdo Cubillos Matias Sinnuet</option>
<option value="486">Jaque Curruhuinca Jos&eacute; Ignacio</option>
<option value="490">Jeanneret Fernandez Mar&iacute;a Francisca</option>
<option value="494">Jofr&eacute; Hargous Alejandra</option>
<option value="498">Jorquera Santa Cruz Maria Jesus</option>
<option value="502">Kast Miranda Ricardo Sebastian</option>
<option value="506">Koehn Tupper Alexandra Stephania</option>
<option value="510">Lagno Carre&ntilde;o Felipe Francisco</option>
<option value="514">Lagos Lastra Maria Paz</option>
<option value="518">Landauro De Vidts Clara</option>
<option value="522">Larraguibel Poblete Jacinta Adelaida</option>
<option value="526">Larra&iacute;n Barros Belen Del Carmen</option>
<option value="530">Larra&iacute;n Cobo Maria Ignacia</option>
<option value="534">Latrach Castro Pilar Macarena</option>
<option value="538">Lav&iacute;n Prieto Camilo Andr&eacute;s</option>
<option value="542">Lecourt Guzm&aacute;n Mar&iacute;a Soledad</option>
<option value="546">Lemaitre Valdes Paula</option>
<option value="550">Le&oacute;n Marconi Nicol&aacute;s Dami&aacute;n</option>
<option value="554">Letelier Silva Juan Bautista</option>
<option value="558">Lino Bzdigian Antonia Isabel</option>
<option value="562">Lizana Mora Mar&iacute;a Isabel</option>
<option value="566">Lobos Guridi Alejandra</option>
<option value="570">L&oacute;pez P&eacute;rez Victoria Teresita</option>
<option value="574">Lorie Fernandez Isabel De La Trinida</option>
<option value="578">Mackenney Mekis Marco Antonio</option>
<option value="582">Magnano Scianca Consuelo</option>
<option value="586">Mardones Mu&ntilde;oz Maria Carolina</option>
<option value="590">M&aacute;rquez Cruz Francisco Jos&eacute;</option>
<option value="594">Martinez Malebran Carla Andrea</option>
<option value="598">Mart&iacute;nez Rioja Joaqu&iacute;n</option>
<option value="602">Matte De La Cerda Mar&iacute;a Paula</option>
<option value="606">Mayol Garc&iacute;a Mar&iacute;a Jos&eacute;</option>
<option value="610">Medina Parra Sarita</option>
<option value="614">Mella Abarca Francisco Javier</option>
<option value="618">Mendez Larrain Leandro Salvador</option>
<option value="622">Mercado Ugarte Catalina</option>
<option value="626">Milnes Retamal Manuela</option>
<option value="630">Mitjans Arrasate Magdalena</option>
<option value="634">Monckeberg Marin M&oacute;nica</option>
<option value="638">Montenegro Marchant Maria Florencia</option>
<option value="642">Montes Vicuna Antonia</option>
<option value="646">Montesinos Moya Florencia</option>
<option value="650">Morales Villagr&aacute;n Ismael Rolando</option>
<option value="658">Moreno Kosterlitz Trinidad</option>
<option value="654">Moreno Zanzani David Ignacio Hern&aacute;n</option>
<option value="662">Moure Cuevas Francisca Javiera</option>
<option value="666">Munita Ruiz-tagle Maria Macarena</option>
<option value="670">Mu&ntilde;oz Gonzalez Valentina Javiera</option>
<option value="674">Musalem Marquez Ignacio</option>
<option value="678">Navarrete Gomez Cristian Ignacio</option>
<option value="682">Nieto Viera Victoria Paz</option>
<option value="686">N&uacute;&ntilde;ez Johnson Bernardita</option>
<option value="690">Olavarr&iacute;a Ib&aacute;&ntilde;ez Daniela Paz</option>
<option value="698">Olivares Casanova Magdalena</option>
<option value="694">Olivares Torres Teresita</option>
<option value="702">Olivos Carvallo Sof&iacute;a</option>
<option value="706">Opazo Oyarz&uacute;n Maria Antonia</option>
<option value="710">Orellana Garc&iacute;a-huidobro Mar&iacute;a Bego&ntilde;a</option>
<option value="714">Ortega Lira Jos&eacute; Tom&aacute;s</option>
<option value="718">Ortiz Pincheira Juan Pablo</option>
<option value="722">Osorio Tchobanian Fabi&aacute;n Alexander</option>
<option value="726">Ossand&oacute;n Tagle Bernardita</option>
<option value="730">Ovalle Saez Francisca</option>
<option value="734">Parada Moure Bernardita</option>
<option value="738">Paredes Mendicoa Renata</option>
<option value="742">Parot Altschwager Jos&eacute; Miguel</option>
<option value="746">Pavez Parada Maria Patricia</option>
<option value="750">Pe&ntilde;a Quintanillo Antonia</option>
<option value="754">Peralta &period; Mar&iacute;a Del Rosario</option>
<option value="758">Perez Degetau Mar&iacute;a De Los &Aacute;ngeles</option>
<option value="762">P&eacute;rez Luna Mar&iacute;a Beatriz</option>
<option value="766">P&eacute;rez Quintana Joaquin</option>
<option value="770">Perez De Arce Manglano Constanza</option>
<option value="774">P&eacute;rez-cotapos Valencia Mar&iacute;a Catalina</option>
<option value="778">Pino Ugarteche Marcelo Alejandro</option>
<option value="782">Pinto Lindarte Maricarmen</option>
<option value="786">Planzer Calder&oacute;n Gianina Elizabeth</option>
<option value="790">Poblete C&aacute;rdenas Carmen Rosa</option>
<option value="794">Prado Letelier Giovanna</option>
<option value="798">Prieto Maturana Maria Laura</option>
<option value="802">Puebla Gonz&aacute;lez Gabriela</option>
<option value="806">Quezada Bisso Jeimson Alexander</option>
<option value="810">Quiroz Suazo Ra&uacute;l Leandro</option>
<option value="814">Ram&iacute;rez D&iacute;az Mar&iacute;a Isabel</option>
<option value="818">Repenning G&aacute;lvez Roberto Eugenio</option>
<option value="822">Reyes Mu&ntilde;oz Martin Cristian</option>
<option value="826">Reymond Armijo Emilia</option>
<option value="830">Ried Undurraga Edgard</option>
<option value="834">R&iacute;os Gonz&aacute;lez H&eacute;ctor</option>
<option value="838">Rivas Nogu&eacute;s Teresa Lee</option>
<option value="846">Rodr&iacute;guez Claro Rafael Antonio</option>
<option value="850">Rodr&iacute;guez Poblete Horacio</option>
<option value="842">Rodriguez Simian Mar&iacute;a Teresa</option>
<option value="854">Rojas O Reilly Guillermo</option>
<option value="858">Rolle Decombe Laura Isabel</option>
<option value="862">Rosenblitt Silva Paulina</option>
<option value="866">Ruiz Fuentes Ricardo Luis</option>
<option value="870">Ruiz De Gamboa Ureta Mar&iacute;a Eugenia</option>
<option value="874">Saa Riquelme Mar&iacute;a Del Carmen</option>
<option value="878">Saavedra Olgu&iacute;n Mar&iacute;a Consuelo</option>
<option value="882">Salazar Alamos Mar&iacute;a Elena</option>
<option value="886">Salgado Cabrera Mar&iacute;a Magdalena</option>
<option value="890">Salinas De La Cerda Carmen Luz Purisima</option>
<option value="894">S&aacute;nchez Bustamante Teresita</option>
<option value="898">Sanhueza Parada Blanca Sofia</option>
<option value="902">Sariego Acevedo Ram&oacute;n Guillermo</option>
<option value="906">Schmidt Lagos Isabel Del Carmen</option>
<option value="910">Sep&uacute;lveda Barraza Carlos Eduardo</option>
<option value="918">Silva Maturana Daniel Alfonso</option>
<option value="922">Silva Miranda Ana Paola</option>
<option value="914">Silva Valencia Mar&iacute;a Elena</option>
<option value="926">Sipkova Bulicich Emma Del Rosario</option>
<option value="930">Solo De Zaldivar Pinto Bernardita</option>
<option value="934">Soto Cifuentes Marcela</option>
<option value="938">Stambuk Verdejo Jos&eacute; Estanislao</option>
<option value="942">Swett Barros Ismael</option>
<option value="946">Swinburn Beiza Luz Mar&iacute;a</option>
<option value="950">Tapia Salinas Marcos</option>
<option value="954">Tellez Torretti Amaro</option>
<option value="958">Tocornal Aguirre Daniel Heriberto</option>
<option value="962">Tornini Fern&aacute;ndez Isabel</option>
<option value="966">Torres Diaz Nancy Ang&eacute;lica</option>
<option value="970">Ugarte Reyes Claudia</option>
<option value="974">Undurraga Cruzat Christian</option>
<option value="978">Ureta Lastra Ver&oacute;nica De Los Ang</option>
<option value="982">Urrutia Infante Juan Carlos</option>
<option value="986">Urruticoechea Machuca Mar&iacute;a Elisa</option>
<option value="994">Vald&eacute;s Holzapfel Maria Francisca</option>
<option value="990">Valdes Ponce Cecilia</option>
<option value="998">Valdivia Del R&iacute;o Jos&eacute; Agust&iacute;n</option>
<option value="1010">Valenzuela D&iacute;az In&eacute;s</option>
<option value="1006">Valenzuela Parra Maria De La Luz</option>
<option value="1014">Valenzuela Saavedra Maria Jose</option>
<option value="1002">Valenzuela Seguel Juan Ignacio</option>
<option value="1018">Vargas Villarreal Gabriela</option>
<option value="1022">Velasco Chac&oacute;n Gloria</option>
<option value="1026">Vera Pe&ntilde;a Rafael Gerardo</option>
<option value="1030">Vergara Donoso Carolina Fernanda</option>
<option value="1034">VIAL Calder&oacute;n Mauricio Jos&eacute;</option>
<option value="1042">Vial Meza Gerardo Alfonso</option>
<option value="1038">Vial Seco Mar&iacute;a Del Pilar</option>
<option value="1046">Vicu&ntilde;a Soto Cristi&aacute;n Salvador</option>
<option value="1050">Vildoso Miranda Eduardo</option>
<option value="1054">Vizcaya Barasorda Rosa Mar&iacute;a Isabel</option>
<option value="1058">Wild Godoy Mirta Alejandra</option>
<option value="1062">Zabala Rosende Amalia De Las Merced</option>
<option value="1066">Za&ntilde;artu Rojas Mar&iacute;a Paz</option>
<option value="1070">Zegers Samaniego Ronald Heinz</option>
<option value="1074">Z&uacute;&ntilde;iga Duhart Mar&iacute;a In&eacute;s</option>
					</select>
				</td>
				<td>
					Enfermero<br/>
					<select name="enfermero" style="width: 250px;">
<option value="0" selected="selected">Seleccionar Tripulación</option>
<option value="3">Abarz&uacute;a Lobos Mar&iacute;a Ignacia</option>
<option value="7">Abusleme Riveros Jeannette Cecilia</option>
<option value="11">Acosta Correa Jimena</option>
<option value="15">Aguero Latorre Sebasti&aacute;n</option>
<option value="19">Aguilera Hurtado Barbara Virginia</option>
<option value="23">Ahumada Fabres Hern&aacute;n Exequiel</option>
<option value="27">Alarcon Concha Sandra M&oacute;nica</option>
<option value="31">Albornoz Montero Gustavo</option>
<option value="35">Alcalde Ibacache Mar&iacute;a Ignacia</option>
<option value="39">Allende PALMA Maria Cecilia</option>
<option value="43">Alliende Petschen Paulina</option>
<option value="47">Alvarez Dell Bernardita</option>
<option value="51">Amen&aacute;bar Barr&iacute;a Manuel Ren&eacute;</option>
<option value="55">Amun&aacute;tegui Cuevas Claudio Fernando</option>
<option value="59">Andrighetti Pacheco Mar&iacute;a Emilia</option>
<option value="63">Aranguiz Valderrama Carola</option>
<option value="67">Araya Busch Fidel Antonio</option>
<option value="71">Arregui Donoso Gisele Alejandra</option>
<option value="75">Arrue Torres Felipe Eduardo</option>
<option value="79">Aspillaga Miranda Mar&iacute;a Carolina</option>
<option value="83">Avenda&ntilde;o Meli&ntilde;il Jeannette Del Carme</option>
<option value="87">Avil&eacute;s Opazo Jacqueline</option>
<option value="91">Babic Cruz Claudio Antonio</option>
<option value="95">Baeza Opazo Maria&nbsp;Teresa</option>
<option value="99">Bambach Ruiz Marisol Del Pilar</option>
<option value="103">Barranco Cummins Jos&eacute; Antonio</option>
<option value="107">Barriga Fuentes Juan Andres</option>
<option value="111">Barros SILVA Paola</option>
<option value="115">Benavente Ramirez Robert Bernardo</option>
<option value="119">Benitez Arce Carolina Andrea</option>
<option value="123">Besa Mu&ntilde;oz Catalina Ofelia</option>
<option value="127">Bezanilla Rozas Mar&iacute;a Paz</option>
<option value="131">Boetsch Villar Magdalena</option>
<option value="135">Brahm Err&aacute;zuriz Rafael Francisco</option>
<option value="139">Bravo Correa Christian Alfredo</option>
<option value="143">Browne Vial Fernando Alejandro</option>
<option value="147">Bugue&ntilde;o Miranda Angelica</option>
<option value="151">Burmester Destefani Guillermo Antonio</option>
<option value="155">Bustos Masramon Ram&oacute;n Eduardo</option>
<option value="159">Cabrera Vicencio Myriam Soledad</option>
<option value="163">Callejas Walker Marco Antonio</option>
<option value="167">Canales Soto Mar&iacute;a Luisa</option>
<option value="171">Cariqueo Gonz&aacute;lez Daniel Alejandro</option>
<option value="179">Carvajal Bastidas Pablo Andr&eacute;s</option>
<option value="175">Carvajal Sep&uacute;lveda Juan Carlos</option>
<option value="183">Castillo Cifuentes Mar&iacute;a Amalia</option>
<option value="187">Castro Puertas Tamara</option>
<option value="191">Caviedes Orphanopoulos Lorena Andrea</option>
<option value="195">Cerda Lorca Ana Mar&iacute;a</option>
<option value="199">Chand&iacute;a Bunster Julio Andr&eacute;s</option>
<option value="203">Cila Calderon Jaime Antonio</option>
<option value="207">Colicheo Anticevic Ana Magdalena</option>
<option value="211">Concha Quintana Josefina</option>
<option value="215">Contesse Sanhueza Catalina Paz</option>
<option value="219">Cornejo Perez Jessica Del Carmen</option>
<option value="223">Correa Amen&aacute;bar Alex Osvaldo</option>
<option value="227">Cort&eacute;s Castillo Javier Sebasti&aacute;n</option>
<option value="231">Costa Cifuentes Paula Ana</option>
<option value="235">Covarrubias Jeldres Francisca Mar&iacute;a</option>
<option value="239">CRUZAT Orbegoso Trinidad</option>
<option value="243">Cuadra Genie Ra&uacute;l Alejandro</option>
<option value="247">Darraidou Obreque Carolina</option>
<option value="251">De La Cerda Almarza Muriel Alejandra</option>
<option value="255">De La Jara P&eacute;rez Claudia Jacqueline</option>
<option value="259">Del Campo Ferrer Alejandro Javier</option>
<option value="263">Delfau Bobadilla Jose Manuel</option>
<option value="267">Diaz Manzano Rosa Mercedes</option>
<option value="271">D&iacute;az Urz&uacute;a Franklin Jos&eacute;</option>
<option value="275">Diez Fabres Luz Mar&iacute;a</option>
<option value="279">Dominguez Rubilar Maria Victoria</option>
<option value="283">Dom&iacute;nguez Vergara Gabriel Emilio</option>
<option value="287">Donoso Dittborn Andr&eacute;s Felipe</option>
<option value="291">Douglas Mundaca Isabel Margarita</option>
<option value="295">Echeverria San Martin Magdalena</option>
<option value="299">Edwards Castro Robinson David</option>
<option value="303">Eguiguren Hidalgo Magdalena</option>
<option value="307">Ellis Vial Francisco De Jes&uacute;s</option>
<option value="315">Err&aacute;zuriz Kast Jos&eacute; Mauricio</option>
<option value="311">Errazuriz Pinto Benjamin Ren&eacute;</option>
<option value="319">Escobar Vasquez Guido Enrique</option>
<option value="323">Espinosa Armstrong Maria Valentina</option>
<option value="327">Estay Yavar Jos&eacute; Antonio</option>
<option value="331">Faine Herrera Mar&iacute;a Luisa</option>
<option value="335">Fern&aacute;ndez Arrau Pilar Del Carmen</option>
<option value="339">Fern&aacute;ndez Becker Ana Maria</option>
<option value="343">Fern&aacute;ndez Lopez Mar&iacute;a Josefina</option>
<option value="347">Figueroa Valdes Maria Betania</option>
<option value="351">Flores Besa Andrea Paz</option>
<option value="355">Fuentes Ovalle Daniel Alejandro</option>
<option value="359">Fuenzalida D&eacute;lano Esteban Andr&eacute;s</option>
<option value="363">Gaete Vicu&ntilde;a Teresita</option>
<option value="367">Galilea L&oacute;pez Maria Carolina</option>
<option value="371">Gallego Subercaseaux Mar&iacute;a Paz</option>
<option value="375">Gana De Solminihac Mar&iacute;a Cristina</option>
<option value="379">Garcia Kast Maria Paz</option>
<option value="383">Garc&iacute;a Silva Macarena Del Pilar</option>
<option value="387">Garc&iacute;a-huidobro Campos Paula</option>
<option value="391">Gaymer Perez Loreto</option>
<option value="395">Goldenberg Gaete Kharim Elizabeth</option>
<option value="399">Gom&eacute;z De Landa Maria Jose</option>
<option value="419">Gonz&aacute;lez Campos Bernardita Maria</option>
<option value="411">Gonz&aacute;lez Ch&aacute;vez Romina</option>
<option value="403">Gonzalez Letelier Mar&iacute;a Ignacia</option>
<option value="415">Gonz&aacute;lez Lucero Claudia Andrea</option>
<option value="407">Gonzalez Munita Ana Maria</option>
<option value="423">Guajardo Aste &Aacute;ngela</option>
<option value="427">Guerra Ovalle Alejandrina</option>
<option value="431">Guti&eacute;rrez Curutchet Mar&iacute;a Josefina</option>
<option value="435">Guzman Varela Loreto De Los Angele</option>
<option value="439">Haggar Pavez Mario Alexis</option>
<option value="447">Herrera Aguirre Maria Jesus</option>
<option value="443">Herrera Larrain Luz Mar&iacute;a</option>
<option value="451">Hirth Mavroski Aurelio Eduardo</option>
<option value="455">Honorato Torres Patricia Andrea</option>
<option value="459">Hurtado Ibaceta Bernardita</option>
<option value="463">Iba&ntilde;ez Arteaga Sofia</option>
<option value="467">Iba&ntilde;ez Rodr&iacute;guez Natalia Del Pilar</option>
<option value="471">Illanes Page Maria De La Paz</option>
<option value="479">Irarr&aacute;zaval Casanova Ariel Alfredo</option>
<option value="475">Irarrazaval Hidalgo Mar&iacute;a  Francisca</option>
<option value="483">Izquierdo Contreras Waldo Alberto</option>
<option value="487">Jara Cerda Sebastian Francisco</option>
<option value="491">Jim&eacute;nez Za&ntilde;artu Maria Ignacia</option>
<option value="495">Jofr&eacute; Larrain Fabi&aacute;n Andr&eacute;s</option>
<option value="499">Jorquera Luna Daniela De Jesus</option>
<option value="503">Kaulen Astaburuaga Romina Eunice</option>
<option value="507">Kunstmann Echeverr&iacute;a Gerardo Arturo</option>
<option value="515">Lagos Contreras Maria Jesus</option>
<option value="511">Lagos Palma Javiera Paz</option>
<option value="519">Lant&eacute;n Molina Mar&iacute;a Consuelo</option>
<option value="523">Larraguibel Zapico Maria Constanza</option>
<option value="527">Larra&iacute;n Bravo Antonio Jos&eacute;</option>
<option value="531">Larra&iacute;n Gutierrez Catalina</option>
<option value="535">Laurie Rivera Sebastian Jesus</option>
<option value="539">Lazo Cruzat Valentina Netti</option>
<option value="543">Lehuede Diaz Mar&iacute;a Eugenia</option>
<option value="547">Lemus Lecaros Mar&iacute;a Teresa</option>
<option value="551">Leosthene Donoso Constanza Anita</option>
<option value="555">Leyton Rodr&iacute;guez Fernando Antonio</option>
<option value="559">Lira Correa Luz Maria</option>
<option value="563">Lizarazu Schmidt Mar&iacute;a Fernanda</option>
<option value="567">Loeser Peralta Daniela</option>
<option value="571">L&oacute;pez Parodi Ana Mar&iacute;a</option>
<option value="575">Lozano Ram&iacute;rez Teresita Maria De Je</option>
<option value="579">Maestro Parot Francisca Jose</option>
<option value="583">Malbec Gana Isidora Paz</option>
<option value="587">Marin Donaire Mar&iacute;a Antonia</option>
<option value="591">Marraccini Mellado Maria Jesus</option>
<option value="599">Mart&iacute;nez Aninat Maria Piedad</option>
<option value="595">Mart&iacute;nez Urzua Guadalupe</option>
<option value="603">Matte Gonz&aacute;lez Trinidad</option>
<option value="607">Mc Intyre Manr&iacute;quez Adriana Mar&iacute;a</option>
<option value="611">Mege Varas Margarita Del Carmen</option>
<option value="615">Mella Astaburuaga Camila Andrea</option>
<option value="619">Mendez Castro Blanca Maria</option>
<option value="623">Mery Rojas Benjam&iacute;n</option>
<option value="627">Milnes Morales Francisca</option>
<option value="631">Mol Garcia-huidobro Josefa</option>
<option value="635">Mondaca Gerbaud Maria Belen</option>
<option value="639">Montenegro D&iacute;az Maria Trinidad</option>
<option value="643">Montes Canessa Nicole</option>
<option value="647">Montoya De La Taille Trentin Trinidad De Los Ange</option>
<option value="651">Morales Leiva Esteban Alejandro</option>
<option value="655">Moreno Ruiz-tagle Crist&oacute;bal</option>
<option value="659">Morere Bezanilla Bernardita</option>
<option value="663">Moya Barrientos Bernardita</option>
<option value="667">Mu&ntilde;oz Barros L&iacute;a</option>
<option value="671">Mu&ntilde;oz De  La Cerda Gabriela Eloisa</option>
<option value="675">Musalem Valenzuela Alberto  Enrique</option>
<option value="687">&Ntilde;anculeo Izquerdo Maria Trinidad</option>
<option value="679">Navarro Gomez Felipe Alfonso</option>
<option value="683">Noguera Zapico Magdalena Francisca</option>
<option value="691">Olcay Ruiz Vicente Ignacio</option>
<option value="699">Olivares Hevia Mar&iacute;a Del Rosario</option>
<option value="695">Olivares Silva Ana Maria</option>
<option value="703">Olivos Letelier Constanza Andrea</option>
<option value="707">Orellana Oyarzun Javiera Ignacia</option>
<option value="711">Ormaz&aacute;bal Ortlieb Trinidad</option>
<option value="715">Ortiz Montenegro Maria Jesus</option>
<option value="719">Ortuzar Lang Mar&iacute;a Trinidad</option>
<option value="723">Ossa Escudero Bel&eacute;n Jazm&iacute;n</option>
<option value="727">Ostornol Brice&ntilde;o Bernardita</option>
<option value="731">Ovalle Aspillaga Francisca</option>
<option value="735">Parada Latife Margarita</option>
<option value="739">Paredes Gana Mar&iacute;a Del Rosario</option>
<option value="743">Parraguez Parot Beatriz</option>
<option value="747">Pavez Favereau Maria Magdalena</option>
<option value="751">Pe&ntilde;a Colicheo Maria Emilia</option>
<option value="767">P&eacute;rez Barona Josefina</option>
<option value="755">Perez Calvimontes Tom&aacute;s</option>
<option value="759">Perez Chavarry Mar&iacute;a Ignacia</option>
<option value="763">P&eacute;rez Luna Noemi</option>
<option value="771">Perez De Arce Angulo Florencia</option>
<option value="775">P&eacute;rez-cotapos Ben&iacute;tez Mar&iacute;a Ignacia</option>
<option value="779">Pino Melendez Steffan Andr&eacute;s</option>
<option value="783">Pizarro Vargas Adriana</option>
<option value="787">Plass Aguirre Juliana  Elizabeth</option>
<option value="791">Poblete Moreno Beatriz Maria</option>
<option value="795">Prado Sep&uacute;lveda Humberto</option>
<option value="799">Prieto Covarrubias Yanelis Ariana</option>
<option value="803">Puente Alfaro Jackeline Del Carmen</option>
<option value="807">Quintana Le&oacute;n Nestor Daniel</option>
<option value="811">Quiroz Benjam&iacute;n Guillermo Antonio</option>
<option value="815">Ramos Vial Luc&iacute;a</option>
<option value="819">Retamal Gonz&aacute;lez Luis Gonzalo</option>
<option value="823">Reyes Lopez Mar&iacute;a Isabel</option>
<option value="827">Riba Balmaceda Monica</option>
<option value="831">Riesco Tapia Magdalena</option>
<option value="835">Riquelme Lagos Elvira</option>
<option value="839">Riveros Olivares Maria Veronica</option>
<option value="851">Rodr&iacute;guez Delgado Carmen</option>
<option value="847">Rodr&iacute;guez Infante Mar&iacute;a&nbsp;De</option>
<option value="843">Rodriguez Mingo Susana</option>
<option value="855">Rojas Mingo Mar&iacute;a Ximena</option>
<option value="859">Romero Vial Patricio Abel</option>
<option value="863">Rubio Mujica Mar&iacute;a Eugenia</option>
<option value="867">Ruiz Celis Mar&iacute;a Beatriz</option>
<option value="871">Ruiz-tagle Bascu&ntilde;an Mar&iacute;a Macarena</option>
<option value="875">Saavedra Gonz&aacute;lez Mar&iacute;a De Los Angeles</option>
<option value="879">Saez Casas Francisca</option>
<option value="883">Salazar Rivera Maria Paz</option>
<option value="887">Salgado Ben&iacute;tez Mar&iacute;a Magdalena</option>
<option value="891">Salinas Bravo Leonor</option>
<option value="895">S&aacute;nchez Salam&eacute; Maria Teresa</option>
<option value="899">Santa Cruz Aldunate Pedro Arturo</option>
<option value="903">Sarmiento Altamirano Pilar</option>
<option value="907">Sekler Arteaga Isabel Margarita</option>
<option value="911">Sep&uacute;lveda Gonz&aacute;lez Manuel</option>
<option value="919">Silva Maturana Pablo Ernesto</option>
<option value="923">Silva Soto Luisa Macarena</option>
<option value="915">Silva Vera Carmen Paz</option>
<option value="927">Soffia Silva Carmen Patricia</option>
<option value="931">Somarriva Godoy Jaime Alfredo</option>
<option value="935">Soto Quezada David</option>
<option value="939">Stark Rojas Mar&iacute;a Carolina</option>
<option value="943">Swett Mechsner Juan Alberto</option>
<option value="947">Tafur Saavedra Monica Andrea</option>
<option value="951">Tapia Pacheco Alejandro Ambrosi</option>
<option value="955">Theza Soto An&iacute;bal</option>
<option value="959">Tocornal Fern&aacute;ndez Marcia Andrea</option>
<option value="963">Toro Torres Mar&iacute;a&nbsp;Soledad</option>
<option value="967">Torres Marin Humbertina</option>
<option value="971">Ugarte Armijo Mar&iacute;a Beatriz</option>
<option value="975">Urbina Alfaro Patricia</option>
<option value="979">Uriarte Montt Erik Patricio</option>
<option value="983">Urrutia Rojas Francisca</option>
<option value="987">Uzal Morales Ximena Denise</option>
<option value="991">Valdes Covarrubias Cecilia</option>
<option value="995">Vald&eacute;s Valderrama Alejandra</option>
<option value="999">Valdivia Ram&iacute;rez Beatriz De Las Merc</option>
<option value="1011">Valenzuela Correa Victoria Del  Carmen</option>
<option value="1007">Valenzuela Diesel Carmen Cecilia</option>
<option value="1003">Valenzuela Sarmiento Carlos Maximo</option>
<option value="1015">Varas Z&uacute;&ntilde;iga Guillermo Sergio</option>
<option value="1019">Vasquez Riquelme Claudio</option>
<option value="1023">Venzano Espinoza Fresia de</option>
<option value="1027">Verdugo Piumarta Maria Veronica</option>
<option value="1031">Vergara Correa Alicia</option>
<option value="1039">Vial Cruz Carlos Patricio</option>
<option value="1043">Vial Sepulveda Carolina</option>
<option value="1035">Vial Ya&ntilde;ez Mar&iacute;a Cecilia</option>
<option value="1047">Vidal Aldunate Marisa</option>
<option value="1051">Villablanca P&eacute;rez Oscar Eduardo</option>
<option value="1055">Walder Marzano Rodrigo</option>
<option value="1059">Wilson Sanhueza Juan Roberto</option>
<option value="1063">Zalazar Moraga Mar&iacute;a De Los Angeles</option>
<option value="1067">Za&ntilde;artu Garrido Soledad Francisca</option>
<option value="1071">Zenteno Masramon Marisol Del Carmen</option>
<option value="1075">Zurita Vergara Carmen Gloria</option>
					</select>
				</td>
				<td>
					Medico<br/>
					<select name="medico" style="width: 250px;">
<option value="0" selected="selected">Seleccionar Tripulación</option>
<option value="4">Abarz&uacute;a Gonz&aacute;lez Catalina Alejandra</option>
<option value="8">Acevedo Ossa Jos&eacute; Ignacio</option>
<option value="12">Adasme Alemparte Maria Dolores</option>
<option value="16">Aguero Trivelli Nuvia Del Carmen</option>
<option value="20">Aguilera Goycoolea Pilar</option>
<option value="24">Alamos Castro Erika Jaqueline</option>
<option value="28">Alarc&oacute;n Jir&oacute;n Luis Miguel</option>
<option value="32">Albornoz Diaz Del R&iacute;o Ruben Marcos</option>
<option value="36">Aldrete Ibacache Ver&oacute;nica Mar&iacute;a</option>
<option value="40">Alliende Vilugron Ana Gabriela</option>
<option value="44">Alvarado Uribe Manuela</option>
<option value="48">Alvarez S&aacute;nchez Luz Mar&iacute;a</option>
<option value="52">Amengual Cerda Maria Jose Laura</option>
<option value="56">Ancapi Devia Maria Catalina</option>
<option value="60">Aninat Arriagada Mar&iacute;a Luisa</option>
<option value="64">Aranguiz Maturana Maria Magdalena</option>
<option value="68">Arenas Iba&ntilde;ez Antonio Enrique</option>
<option value="72">Arriaza Escobar Erika</option>
<option value="76">Arteaga Wielandt Angelica</option>
<option value="80">Aspillaga Vergara Mar&iacute;a Trinidad</option>
<option value="84">Avenda&ntilde;o Godoy Alberto</option>
<option value="88">Avil&eacute;s Ramirez Elizabeth Margarita</option>
<option value="92">Baboun Larenas Mar&iacute;a Pilar</option>
<option value="96">Baeza Ponce Mar&iacute;a Francisca</option>
<option value="100">Barahona Widow Ana Elisa</option>
<option value="104">Barrera Bottinelli Jos&eacute; Antonio</option>
<option value="108">Barrios Correa Alejandra Del Rosari</option>
<option value="112">Barros Salas Rosario</option>
<option value="116">Bengolea Torres Ingrid Lucila</option>
<option value="120">Berguecio Bennett Mar&iacute;a Paz</option>
<option value="124">Besa Ballestero Bernardo Patricio</option>
<option value="128">Biggs Zenteno Olga De Las Mercedes</option>
<option value="132">Borquez Benavides Mario Enr&iacute;que</option>
<option value="136">Bralic Fuenzalida Jimena</option>
<option value="140">Bravo Braun Ximena Del Carmen</option>
<option value="144">Browne Valenzuela Francisco Javier</option>
<option value="148">Bugue&ntilde;o Tobar Daniela</option>
<option value="152">Bustamante Naranjo Sandra Jimena</option>
<option value="156">Bustos Vald&eacute;s Victoria</option>
<option value="160">C&aacute;ceres Benavides Madelheyn Patricia</option>
<option value="164">Calvert Benavides Luis Hernan</option>
<option value="168">Canessa Salvatore Maria Teresa</option>
<option value="172">Caris Sorich Carolina Del Carmen</option>
<option value="176">Carvajal Lillo Francisco Alejandro</option>
<option value="180">Carvajal Ovalle Mar&iacute;a Florencia</option>
<option value="184">Castillo Gaete Rodrigo Jos&eacute;</option>
<option value="188">Castro Jarpa Mar&iacute;a Jos&eacute;</option>
<option value="192">Celis Soto Macarena Eugenia</option>
<option value="196">Cerda Segovia Mar&iacute;a Victoria</option>
<option value="200">Ch&aacute;vez Ciudad C&eacute;sar Rodrigo</option>
<option value="204">Claro De Landa Luz Mar&iacute;a</option>
<option value="208">Colipe Cunliffe Maria Adela</option>
<option value="212">Concha Alessandri Carol Judith</option>
<option value="216">Contreras Mart&iacute;nez Mariana</option>
<option value="224">Correa Johnson Osvaldo Antonio</option>
<option value="220">Correa Morales Catalina</option>
<option value="228">Cort&eacute;s Cortes Maria Luisa</option>
<option value="232">Costa Miranda N&eacute;lson William</option>
<option value="236">Cox Garcia Maria Del Pilar</option>
<option value="240">Cruzat Hurtado Mar&iacute;a Teresa</option>
<option value="244">Cuadra Alvarez Isabel Margarita</option>
<option value="248">De Castro D&iacute;ez Mar&iacute;a Gabriela</option>
<option value="252">De La Cerda Diaz Alfredo Ignacio</option>
<option value="256">De La Lastra Gallardo Manuel Andr&eacute;s</option>
<option value="260">Del R&iacute;o Ruz Mar&iacute;a Te</option>
<option value="264">Delgado Navarro Maria Laura</option>
<option value="272">D&iacute;az C&oacute;rdova Vicente Octavio</option>
<option value="268">Diaz Garcia-huidobro Taimis</option>
<option value="276">Diez Benavides Josefina</option>
<option value="284">Dom&iacute;nguez Damm Mar&iacute;a Josefina</option>
<option value="280">Dominguez Vergara Paulo Cesar</option>
<option value="288">Donoso D&iacute;az Jose Ignacio</option>
<option value="292">Duhart Vergara Francisco Javier</option>
<option value="296">Echeverria Wilckens Maria Jose</option>
<option value="300">Edwards D&iacute;az Magdalena</option>
<option value="304">Eguiguren De La Lastra Gonz&aacute;lo An&iacute;bal</option>
<option value="308">Eluani Capdevila Ana Mar&iacute;a</option>
<option value="312">Errazuriz Aspillaga Macarena Mar&iacute;a</option>
<option value="316">Err&aacute;zuriz Palma Paul Jimmy</option>
<option value="320">Escobar Knight Luis Alejandro</option>
<option value="324">Espinosa Mateluna Felipe Ignacio</option>
<option value="328">Estay Bustamante Gracia</option>
<option value="332">Feller M&eacute;ndez Maria Jes&uacute;s</option>
<option value="336">Fern&aacute;ndez Costabal Isabel Margarita</option>
<option value="340">Fern&aacute;ndez Iba&ntilde;ez Florencia</option>
<option value="344">Fern&aacute;ndez Del R&iacute;o Tarud Bernardita</option>
<option value="348">Figueroa Gil Mar&iacute;a Francisca</option>
<option value="352">Fontanet Jorquera Ismael</option>
<option value="356">Fuenzalida Ekelund Mauricio De Jes&uacute;s</option>
<option value="360">Fuenzalida V&aacute;squez Vicente Antonio</option>
<option value="364">Gaete Matte Mar&iacute;a Consuelo</option>
<option value="368">Gallardo Araya Juan Eduardo</option>
<option value="372">Gamboa Valenzuela MARIA BERNARDITA</option>
<option value="376">Ganzur Balmaceda Iv&aacute;n Alejandro</option>
<option value="384">Garc&iacute;a Basilio Trinidad</option>
<option value="380">Garc&iacute;a Ortuzar Cecilia</option>
<option value="388">Garc&iacute;a-huidobro Kruse Maria Teresa</option>
<option value="392">Gazmuri Serani Magdalena Maria</option>
<option value="396">Goldenberg Bacarreza Catalina</option>
<option value="400">G&oacute;mez Guzman Matias Eduardo</option>
<option value="416">Gonz&aacute;lez Dom&iacute;nguez Javiera Alejandra</option>
<option value="412">Gonz&aacute;lez Dur&aacute;n Mar&iacute;a Jos&eacute;</option>
<option value="404">Gonzalez Musso Sof&iacute;a</option>
<option value="408">Gonzalez Rios Cristina Mar&iacute;a</option>
<option value="420">Gonz&aacute;lez Simonetti Magdalena Mar&iacute;a</option>
<option value="424">Guajardo Zapico Paula</option>
<option value="428">Guerrero Arraztoa Constanza</option>
<option value="432">Guti&eacute;rrez Milnes Camila</option>
<option value="436">Guzman Oehninger Isabel</option>
<option value="440">Halty Escobar Ariel Antonio</option>
<option value="448">Herrera Gastellu Leyla Katherine</option>
<option value="444">Herrera Huneeus Francisco Jose</option>
<option value="452">Hojas Mart&iacute;nez B&aacute;rbara</option>
<option value="456">Honour Lorca Donald Benjamin</option>
<option value="460">Hurtado Araya Mar&iacute;a Teresa</option>
<option value="468">Ib&aacute;&ntilde;ez Arancibia Carlos Nicolas</option>
<option value="464">Iba&ntilde;ez Fernadez Rocio Belen</option>
<option value="472">Infante Ayestaran Maria Del Pilar</option>
<option value="476">Irarr&aacute;zaval Aravena Valentina Paz</option>
<option value="480">Izcue Sep&uacute;lveda Francisca Pilar</option>
<option value="484">Izquierdo Quezada Manuel Alejandro</option>
<option value="488">Jara Valenzuela Francisco Javier</option>
<option value="492">Joannon Rodr&iacute;guez Trinidad</option>
<option value="496">Jofr&eacute; Correa Nicol&aacute;s Jos&eacute;</option>
<option value="500">Julbe Monge Carolina Paz</option>
<option value="504">Kayser Morande Alejandro Alberto</option>
<option value="508">Labarca Vergara Marco Antonio</option>
<option value="516">Lagos Cruz Maria Josefina</option>
<option value="512">Lagos Viacava Miguel Jos&eacute;</option>
<option value="520">Lara Nieto Magdalena</option>
<option value="532">Larra&iacute;n Camus Catalina Paz</option>
<option value="528">Larra&iacute;n Castillo Bernardita</option>
<option value="524">Larrain Wood Rodrigo Andr&eacute;s</option>
<option value="536">Lavin Caviedes Mar&iacute;a Rosario</option>
<option value="540">Lecaros Rastinoff Jose Manuel</option>
<option value="544">Leiva Duval Maria Isabel</option>
<option value="548">Le&oacute;n Latife Luis Andres</option>
<option value="552">Letelier Gonz&aacute;lez Jos&eacute; Ignacio</option>
<option value="556">Leyton Vargas Maria Ignacia</option>
<option value="560">Lira P&eacute;rez Maria Jesus</option>
<option value="564">Llona Rios Maria Angelica</option>
<option value="568">Lopez Bacarreza Maria Ignacia</option>
<option value="572">Lorca Cruz Mar&iacute;a Paz</option>
<option value="576">Lucero Montt Maria Paz</option>
<option value="580">Maffei Bezanilla Mat&iacute;as Ignacio</option>
<option value="584">Maldonado Morales Mar&iacute;a Gabriela</option>
<option value="588">Mar&iacute;n Moz&oacute; Sofia Maria</option>
<option value="592">Martinez De La Carrera Luis Alberto</option>
<option value="600">Mart&iacute;nez Manzanares Margarita Maria</option>
<option value="596">Mart&iacute;nez Valdes Mar&iacute;a Jes&uacute;s</option>
<option value="604">Matte Irarrazaval Ignacio Andres</option>
<option value="608">Medina Vergara Macarena</option>
<option value="612">Melendez Iglesias Magdalena</option>
<option value="616">Mella Cano Maria Fernanda</option>
<option value="620">M&eacute;ndez Allende Consuelo Maria</option>
<option value="624">Meyer Montero Mar&iacute;a Ignacia</option>
<option value="628">Miranda Araya Mar&iacute;a Alejandra</option>
<option value="632">Mol Lira Maria Elisa</option>
<option value="636">Montaldo Hargous Bernardita</option>
<option value="640">Montero Echenique Francisca Javiera</option>
<option value="644">Montes Rivas Mar&iacute;a Teresa</option>
<option value="648">Montt Saavedra Constanza De Lourdes</option>
<option value="652">Morales Bitterncourt Maria Trinidad Ines</option>
<option value="656">Moreno Z&uacute;&ntilde;iga Sebastian Luis</option>
<option value="660">Moretti Rufin Susanne Nicole</option>
<option value="664">Moya Valenzuela Jos&eacute; Agust&iacute;n</option>
<option value="672">Mu&ntilde;oz Parodi Javiera Antonia</option>
<option value="668">Mu&ntilde;oz Vial Catalina</option>
<option value="676">Nahuelpi Beizan Consuelo</option>
<option value="680">Navarro Iturriaga Maria Jesus</option>
<option value="684">Nu&ntilde;ez Echeverr&iacute;a Connie Gabriela</option>
<option value="688">O reilly Von Wussow Pilar</option>
<option value="692">Olea Achurra Rebeca</option>
<option value="696">Olivares Caro Valentina Paz</option>
<option value="700">Olivares Ugarte CLEMENTE JOS&Eacute;</option>
<option value="704">Olivos Letelier Daniel Eduardo</option>
<option value="708">Orellana M&eacute;ndez Daniela Ignacia</option>
<option value="712">Orozco P&eacute;rez Maria Agustina</option>
<option value="716">Ortiz Salinas Vicente</option>
<option value="720">Ort&uacute;zar Covarrubias Andrea</option>
<option value="724">Ossa Montero Sebastian</option>
<option value="728">Ovalle Barros Elisa</option>
<option value="732">Oviedo Segovia Maria Josefina</option>
<option value="736">Pardo Bascur Maria Paz</option>
<option value="740">Paredes Pizarro Mar&iacute;a Catalina</option>
<option value="744">Parraguez Garcia Beatriz</option>
<option value="748">Pavez Von Appen Bernardita</option>
<option value="752">Pe&ntilde;afiel Klein Maria Paz</option>
<option value="760">P&eacute;rez Benites Bernardita Maria</option>
<option value="756">Perez Carrero Maria Jesus</option>
<option value="764">P&eacute;rez Pinto Nicolas</option>
<option value="768">P&eacute;rez Ramirez Mar&iacute;a Catalina</option>
<option value="772">P&eacute;rez De Arce Luque Ramiro</option>
<option value="776">Pimentel Lopez Andr&eacute;s Eduardo</option>
<option value="780">Pino Rondon Gerardo Andr&eacute;s</option>
<option value="784">Pizarro Acu&ntilde;a Macarena</option>
<option value="788">Poblete Rocuant Eugenia Guadalupe</option>
<option value="792">Pradenas Cueto Marta</option>
<option value="800">Prieto Eche&ntilde;ique N&ouml;el</option>
<option value="796">Prieto Zapico Erika Josefina</option>
<option value="804">Pulido Santa Cruz Yuri</option>
<option value="808">QUINTERO Hevia Antonia</option>
<option value="812">Raggi Vial Lindor Patricio</option>
<option value="816">Rauld Ossa Margarita Rosa</option>
<option value="820">Reyes De&nbsp;La&nbsp;Cortina Mar&iacute;a Lu</option>
<option value="824">Reyes Infante Jos&eacute;</option>
<option value="828">Ricalde Guerra Claudio Antonio</option>
<option value="832">Ringeling Mart&iacute;nez Patricia</option>
<option value="836">Rivas P&eacute;rez Mar&iacute;a In&eacute;s Del Pilar</option>
<option value="840">Rocha Garc&iacute;a Mar&iacute;a Ines</option>
<option value="844">Rodriguez Faur&eacute; Waldemar</option>
<option value="848">Rodr&iacute;guez Fern&aacute;ndez Nancy Bernardita</option>
<option value="852">Rodr&iacute;guez Lecaros Humberto</option>
<option value="856">Rojas Mingo Maria Asuncion</option>
<option value="860">Romero Vial Patricio</option>
<option value="864">Ruff Troncoso Mar&iacute;a Jos&eacute;</option>
<option value="868">Ruiz Celis Mar&iacute;a Jos&eacute;</option>
<option value="872">Ruiz-tagle Mery Francisca</option>
<option value="876">Saavedra Talavera Marcela Paz</option>
<option value="880">Saitua Brahm Francisca</option>
<option value="884">Salbach Rojas Mar&iacute;a Paz</option>
<option value="888">Salinas Galleguillos Vesna Paula</option>
<option value="892">Salvestrini Johnson Mar&iacute;a Soledad</option>
<option value="896">Sandoval Palacios Ana Mari</option>
<option value="900">Santana Bolados M&oacute;nica</option>
<option value="904">Schmidt Cardenas Jorge Arturo</option>
<option value="908">Sep&uacute;lveda Jeria Loreto</option>
<option value="912">Sharp Madrid Constanza Mar&iacute;a</option>
<option value="916">Silva Mu&ntilde;oz Elizabeth</option>
<option value="920">Silva Perez Blanca Marcela</option>
<option value="924">Simonetti Mellas Miguel</option>
<option value="928">Soler Jofr&eacute; Marcelo</option>
<option value="932">Soto Rodriguez Domingo Antonio</option>
<option value="936">Sotomayor Rivadeneira Alejandra</option>
<option value="940">Stevenson Molina Mar&iacute;a Jos&eacute;</option>
<option value="944">Swett Altamirano Jos&eacute; Germ&aacute;n</option>
<option value="948">Tagle Vald&eacute;s Mariella Gemma</option>
<option value="952">Taulis Torres Maria Alejandra</option>
<option value="956">Thieme Correa Jose Luis</option>
<option value="960">Tornero Van Der Valk Bernardo</option>
<option value="964">Toro Torres Mar&iacute;a Ang&eacute;lica</option>
<option value="968">Troncoso Eguiguren Adriana</option>
<option value="972">Ugarte Illanes Alicia Lorena</option>
<option value="976">Ureta Cubillos Josefina</option>
<option value="980">Urquidi Carvajal Mar&iacute;a Lo</option>
<option value="984">Urrutia S&aacute;ez Daniel Orlando</option>
<option value="992">Vald&eacute;s Espinoza Marcela Teresita</option>
<option value="988">Valdes Ort&iacute;z Nelly Patricia</option>
<option value="996">Vald&eacute;s Vidal Marcela</option>
<option value="1000">Valdivieso Perez Margarita Del Carmen</option>
<option value="1012">Valenzuela Donoso Mario</option>
<option value="1004">Valenzuela Gonz&aacute;lez Maria Jose Carmela</option>
<option value="1008">Valenzuela Troemel Roberto Marcelino</option>
<option value="1016">Varela Err&aacute;zuriz Marcela</option>
<option value="1020">V&aacute;squez Soto Ar&iacute;stides Antonio</option>
<option value="1024">Vera Trujeda Mar&igrave;a Is</option>
<option value="1028">Vergara Barraza Luis</option>
<option value="1032">Vergara Villavicencio Juan Carlos</option>
<option value="1040">Vial Etchevers Patricio</option>
<option value="1036">Vial Infante Jaime Eduardo</option>
<option value="1044">Vial Rojas Carlos Enrique</option>
<option value="1048">Vidal De La Cerda Gonzalo</option>
<option value="1052">Viollier Romero Blanca Luz</option>
<option value="1056">Walker Riveros Elia Del Carmen</option>
<option value="1060">Ya&ntilde;ez Gonz&aacute;lez Mar&iacute;a</option>
<option value="1064">Zanolli Portales Leonel Abd&oacute;n</option>
<option value="1068">Zavala Mar&iacute;n Soledad Francisca</option>
<option value="1072">Zu&ntilde;iga Ancacura H&eacute;ctor Francisco</option>
<option value="1076">Zurita Musalem Cecilia Del Carmen</option>
					</select>
				</td>
			</tr>
			<tr>
				<td>
					Ida/Vuelta<br/>
					<select name="ida_vuelta" style="width: 150px;">
<option value="2">Ida y Vuelta</option>
<option value="1" selected="selected" >Solo Ida</option>
					</select>
				</td>
				<td>
					Tiempo Espera<br/>
					<select name="espera" id="espera" style="width: 100px;" onChange="cambio_espera()">
<option value="18">0 Hora</option>
<option value="1">0&comma;5 Hora</option>
<option value="2">1&comma;5 hora</option>
<option value="3">2 hora</option>
<option value="4">2&comma;5 hora</option>
<option value="5">3 hora</option>
<option value="6">3&comma;5 hora</option>
<option value="7">4 hora</option>
<option value="8">4&comma;5 hora</option>
<option value="9">5 hora</option>
<option value="10">5&comma;5 hora</option>
<option value="11">6 hora</option>
<option value="12">6&comma;5 hora</option>
<option value="13">7 hora</option>
<option value="14">7&comma;5 hora</option>
<option value="15">8 hora</option>
<option value="16">8&comma;5 hora</option>
<option value="17">Otro</option>
					</select>
					<input type="text" name="espera_otro" id="espera_otro" value="" maxlength="5"  style="width: 100px;" onkeypress="return ingdecimal(event,this)"/>
				</td>
				<td>
					Condiciones de Pago<br/>
					<select name="pago_condicion" style="width: 150px;">
<option value="5">Cr&eacute;dito</option>
<option value="1" selected="selected" >Efectivo</option>
<option value="3">Tarjeta Credito</option>
<option value="4">Tarjeta Debito</option>
<option value="2">Transferencia</option>
					</select>
				</td>
				<td>
					Forma de pago - Número de documento<br/>
					<select name="pago_forma" style="width: 100px;">
<option value="1" selected="selected" >Boleta</option>
<option value="2">Factura</option>
					</select>
					<input type="text" name="num_documento" id="num_documento" value="" maxlength="8"  style="width: 100px;" />
				</td>
			</tr>
			<tr>
				<td colspan="3">
					<span class="txtcampo" id="txt_diagnostico">Diagnostico Paciente</span><br/>
					<textarea name="diagnostico" id="diagnostico" cols="140" rows="3"></textarea>
				</td>
				<td>
					Folio<br/>
					<input type="text" name="folio" id="folio" value="" maxlength="8"  style="width: 100px;"  onkeypress="return ingentero(event,this)"/>
				</td>
			</tr>
			<tr>
				<td>
				Requerimiento<br/>
<input type="checkbox" name="req1" id="req1" value="1"/><label for="req1">Oxigeno</label><input type="checkbox" name="req2" id="req2" value="2"/><label for="req2">Aspiraci&oacute;n</label><input type="checkbox" name="req3" id="req3" value="3"/><label for="req3">Monitorizaci&oacute;n</label>				</td>
				<td>
					Aislamiento<br/>
<input type="checkbox" name="ais1" id="ais1" value="1"/><label for="ais1">Sin Aislamiento</label><input type="checkbox" name="ais2" id="ais2" value="2"/><label for="ais2">Contacto</label><input type="checkbox" name="ais3" id="ais3" value="3"/><label for="ais3">Gotita</label><input type="checkbox" name="ais4" id="ais4" value="4"/><label for="ais4">A&eacute;reo</label>				</td>
				<td>
					Condición de traslado<br/>
<input type="checkbox" name="cod1" id="cod1" value="1"/><label for="cod1">Camilla</label><input type="checkbox" name="cod2" id="cod2" value="2"/><label for="cod2">Silla Ruedas</label><input type="checkbox" name="cod3" id="cod3" value="3"/><label for="cod3">Incubadora</label><input type="checkbox" name="cod4" id="cod4" value="4"/><label for="cod4">Ambulatorio</label>				</td>
				<td>
					<span class="txtcampo" id="txt_precio">
					Valor en Pesos ($)</span><br/>
					<input type="text" name="precio" id="precio" style="width: 150px;" value="" maxlength="10" onkeypress="return ingentero(event,this)"/>
					
				</td>
			</tr>
			<tr>
				<td colspan="4">
					Observaciones<br/>
					<textarea name="obs" cols="140" rows="3"></textarea>
				</td>
			</tr>
		</table>
		
		<input type="button" style="margin: 10px 0px; padding: 7px" onClick="validar()" value="Guardar Traslado"/>
		</p>
		<input type="hidden" name="id_cliente" id="id_cliente" value=""/>
		</form>
	</section>
	
	<script type="text/javascript">
		cambio_hora();
		hora_termino();
		cambio_espera();
		cambio_desde();
		cambio_hasta();
		cambio_intermedio();
		paciente(2);
	</script>
	

</body>
</html>
<!---
james334334/james334334 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
