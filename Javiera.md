<section>

 

## Resolución ejercicios de desarrollo

 

- Pon tu nombre al atributo value del campo first name
- Pon el valor a la pregunta Favorite Day of Week a Monday
- Cambia la etiqueta de First name a 'Tu nombre'
- Obtén el valor del atributo 'name' del campo Favorite Day of The Week
- Escoge la opción Female de la pregunta de género.
- Encuentra la primera form del documento y pon el atributo name = personal_info
- Encuentra la primera form del documento y pon el atributo name = job_info
- Agrega un título h1 a cada una de las formas que diga 'Entrevista personal', 'Entrevista de trabajo' respectivamente
- Agrega un título a la pregunta Male/Female 'Gender'
- Agrega una pregunta Email: con un input de tipo texto después de last name
- Agrega la clase form a ambas for- </section>


	~~~js
	$('[name = "firstname"]').attr("value"); //recupera el valor

	    $('[name = "firstname"]').attr("value", "javiera"); //cambia valor por otro 
 
	  	jQuery("select[name = 'fav_day'] option[value='Monday']").attr("selected", "selected");
		  //cambia la opción por defecto a 'Monday' 

	  	$('[name = "first_name_label"]').text('Tu nombre'); 
		  //cambia el label de 'First name' a 'Tu nombre' 
		   
	  	$('[name = "fav_day"]').attr('name');
		  //Obtiene el valor del atibuto "name" del campo Favorite Day Of The Week

 	    $('[value = "female"]').attr('checked', true);
		  //Escoge la opción Female de la pregunta de género

	 	$("form:eq(0)").attr('name', 'personal_info');
		  /*Encuentra la primera etiqueta form del documento y pone el atributo name=personal_info*/

		$("form:eq(1)").attr('name', 'job_info'); 
		  /*Encuentra la segunda etiqueta form del documento y pon el 
		  atributo name = job_info */

		$( ".tit1").append('<h1>Entrevista personal</h1>'); 
		$( ".tit2").append('<h1>Entrevista de trabajo</h1>');  
		  /* Agrega un título h1 a cada una de las formas que diga 'Entrevista personal', 'Entrevista de trabajo' respectivamente */

		
		$( ".genName").append('<label>Tu genero:</label>'); 
		  // Agrega un título a la pregunta Male/Female 'Gender' 


		$( ".mail" ).append('<input >'); 
		$('.mail').children().attr('name', 'email');
		$('.mail').children().attr('type', 'email');  
		 /* Agrega una pregunta Email: con un input de tipo email con name email, después de last name. */

		 $("form:eq(0)").attr('class', 'formu1');
		 $("form:eq(1)").attr('class', 'formu2'); 
		 //Agrega la clase form a ambas etiquetas de form	~~~