<section>

 
## Desarrollo de ejercicio de repaso de javascript y jquery

 

	~~~js
	 
	  var calcularIMC = function(peso, estatura){
		 	return peso / (estatura * estatura);
		 }(60,1.60)

		  function interpretarIMC (varimc){
		 	var imc = varimc 
		 	if (imc => 25){
		 		return "sobrepeso";
		 	} else if (imc > 19) {
		 		return "ok";
		 	} else {
		 		return "bajo peso";
		 	}
		 }

		 resultado = interpretarIMC(calcularIMC);  
		 console.log(resultado);

	 
	 
	~~~


 