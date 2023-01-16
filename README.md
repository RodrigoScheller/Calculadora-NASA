# Calculadora-NASA -> HTML

<!DOCTYPE html>
  <html>
    <head>


	    <title>CALCULADORA</title>

        <!-- CSS only -->
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">
        <!-- JavaScript Bundle with Popper -->
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3" crossorigin="anonymous"></script>
        <script src="https://code.jquery.com/jquery-3.6.1.js" integrity="sha256-3zlB5s2uwoUzrXK3BT7AX3FyvojsraNFxCc2vC/7pNI=" crossorigin="anonymous"></script>
        <link href="style.css" rel="stylesheet">
  
    </head>

        <body>
        
          <div class="fundo_h1"><h1>CALCULADORA </h1></div>
            <div class="container"></div>
              <div id="conteudo_calculadora">
                <div class="calculadora" >
                
                  <div class="conteudo_visor">
                    <input type="text" id="visor">
                    </input>
                  </div>
          
                    <div id="conteudo_numero">
                        <div>
                          <div class="button_numeros"><button onclick="adicionaValorVisor(7);">7</button></div>
                          <div class="button_numeros"><button onclick="adicionaValorVisor(8);">8</button></div>
                          <div class="button_numeros"><button onclick="adicionaValorVisor(9);">9</button></div>
                        </div>

                          <div >
                            <div class="button_numeros"> <button onclick="adicionaValorVisor(4);">4</button></div>
                            <div class="button_numeros"><button onclick="adicionaValorVisor(5);">5</button></div>
                            <div class="button_numeros"><button onclick="adicionaValorVisor(6);">6</button></div>
                          </div>
                        
                            <div >
                              <div class="button_numeros"> <button onclick="adicionaValorVisor(1);">1</button></div>
                              <div class="button_numeros"> <button onclick="adicionaValorVisor(2);">2</button></div>
                              <div class="button_numeros"><button onclick="adicionaValorVisor(3);">3</button></div>
                            </div>
                  
                                <div class="button_numeros"><button onclick="adicionaValorVisor('.');">.</button></div>
                                <div class="button_numeros"><button onclick="adicionaValorVisor(0);">0</button></div>
                                <div class="button_numeros"><button onclick="calcular();">=</button></div>
                    </div>
                


                      <div class="conteudo_operacao">
                          <div ><button onclick="adicionaValorVisor('+');">+</button></div>
                          <div ><button onclick="adicionaValorVisor('-');">-</button></div>
                          <div ><button onclick="adicionaValorVisor('*');">*</button></div>
                          <div ><button onclick="adicionaValorVisor('/');">/</button></div>
                      </div>
                    

                    <div>
                      <div id=conteudo_acoes>
                        <button  class="limpar" onclick="limparValorVisor();">Limpar</button>
                      </div>
                    </div>
                </div>    
              </div>

                  <p class="resultado2"><div id="conteudo_logs"></div></p>
        
        </body>

    <script src="calculadora.js"></script>
  </html>
  
  
  # Calculadora-NASA -> CSS
  
  html {
	text-align: center;
}

h1{
	padding: 35px;
	margin-left: 0px;
	z-index: +1	;
	letter-spacing: 2.5px;
	text-transform: capitalize bold	italic;
	text-shadow: #fff;
	font-size: 40px;
}

.fundo_h1 {
	z-index: -1	;
	width: 400px;
	height: 120px;
	margin-right: 600px;
	background-color: aqua;
	opacity: 50%;
	margin-top: 30px;
	margin-left: 478px;
}

.fundo_h1 :hover {
	background-color: red;
}

.conteudo_visor {
	align-items: center;
	padding: 50px;
}

.container {
display: flex;
flex-direction: row;
align-items: center;
max-width: 100px;
text-align: center;
}

#conteudo_numero {
	float: left;
	padding: 15px;
}

.conteudo_visor {
	background-color: rgba(84, 87, 87, 0.308);
	border-bottom: double #000;
}

#visor {
	width: 350px;
	height: 95px;
	background-color: rgb(207, 218, 218);
	font-size: 30px;
	font-family: Arial, Helvetica, sans-serif;
}

#numero_centro {
	float: left;
	padding: 15px;
}

.conteudo_operacoes {
	float: left;
}

#conteudo_acoes {
	margin-top: 30px	;
}

button {
  padding: 25px;
	margin: 5px;
	color: #000;
	
}

.button_numeros{
	float: left;
}

.limpar {
	text-align: center;
}

#resultado {
	margin-top: 70px;
	width: 350px;
	height: 150px;
}

.calculadora {
	border: solid #000;
	background-color: rgba(84, 87, 87, 0.308);
	float: left;
	
}


body {
  background-image: url("https://th.bing.com/th/id/R.2abbc33ac220efebebdb2b347afbcf47?rik=qkPo55ca1kEwug&riu=http%3a%2f%2fwallup.net%2fwp-content%2fuploads%2f2016%2f01%2f297996-space-Earth.jpg&ehk=LPVTPSuaysfspV3FWZYhRZiI6r1MuhDnjZGde%2fmsF54%3d&risl=&pid=ImgRaw&r=0");
	background-repeat: no-repeat;
	background-size: cover;
}

#conteudo_logs {
	position: absolute;
	margin-top: 730px;
	border: solid #000;
	width: 420px;
	height: 200px;
	margin-left: 467px;
	margin-bottom: 500px;
	padding: 20px 160px;
}

#conteudo_calculadora {
	position: absolute;
	margin-top: 800px;
	margin-left: -150px;
}

.calculadora {
margin-left: 600px;
margin-top: -750px;
}
  
  
  
   # Calculadora-NASA -> JavaScript
   
   
   
 function adicionaValorVisor(valor){
	console.log("Adicionou o texto " + valor + " no visor.");
	document.getElementById("visor").value += valor;

}

function limparValorVisor(){
document.getElementById("visor").value = "";
}

function calcular(){
	console.log("Função calcular.");
	var resultado = "";
	var operacao = "";
	var valor1 = "";
	var valor2 = "";

	var conteudoVisor = document.getElementById("visor").value;
	
	for (var indice = 0; indice < conteudoVisor.length; indice++){

		var valorIndice = conteudoVisor[indice];
                if((isNaN(valorIndice)) && (valorIndice != ".")){
			if(valorIndice == "+"){
				operacao = valorIndice;
			}else
			if(valorIndice == "-"){
				operacao = valorIndice;
			}else
			if(valorIndice == "*"){
				operacao = valorIndice;
			}else	
			if(valorIndice == "/"){
				operacao = valorIndice;
			}
		}else{
						
			if(operacao==""){
				valor1 += valorIndice;
			}else{
                                valor2 += valorIndice;                
			}
		} 
		
		if(isNaN(conteudoVisor[indice+1])){
			if((valor1 != "") && (valor2 !="") && (operacao != "")){
				if(operacao == "+"){
					resultado = somar(parseFloat(valor1),parseFloat(valor2));
				}else
				if(operacao == "-"){
					resultado = subtrair(parseFloat(valor1),parseFloat(valor2));
				}else
				if(operacao == "*"){
					resultado = multiplicar(parseFloat(valor1),parseFloat(valor2));
				}else
				if(operacao == "/"){
					resultado = dividir(parseFloat(valor1),parseFloat(valor2));
				}
				
				valor1 = resultado;
                                valor2 = "";
			}
		}
				
			

	}  
	console.log("executou o calculo");
	if(resultado){
		exibirResultado(resultado);
		log(conteudoVisor + "=" + resultado);
	}
            

			
}

function somar(val1,val2){
	console.log("Somou os valores " + val1 + " e " + val2 + " no visor.");
	return val1 + val2;
}
 
function subtrair(val1,val2){
	console.log("Subtraiu os valores " + val1 + " e " + val2 + " no visor.");
return val1 - val2;
}

function multiplicar(val1,val2){
	console.log("Multiplicou os valores " + val1 + " e " + val2 + " no visor.");
return val1 * val2;
}

function dividir(val1,val2){
	console.log("Dividiu os valores " + val1 + " e " + val2 + " no visor.");
return val1 / val2;
}

function exibirResultado(valor){
	console.log("Atribuiu o valor " + valor + " no visor.");
}

function log(valor){
	console.log("Adicinou o log " + valor + ".");
if(valor!=""){
var textoLog = "<p>" + valor + "</p>" + document.getElementById("conteudo_logs").innerHTML;
document.getElementById("conteudo_logs").innerHTML = textoLog;

conteudo_logs.style.background = '#fff';
conteudo_logs.style.opacity = '50%';

}
}

function exibirResultado(valor){
    console.log("Atribuiu o valor " + valor + " no visor.");
    document.getElementById("visor").value = valor;



}
  
