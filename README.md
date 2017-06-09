# CalculadoraJQ

CalculatorJQ es una calculadora básica en linea en la que puedes sumar, restar, multiplicar y dividir.

Puedes ver la calculadora y jugar con ella en [CalculadoraJQ](https://fiorellaqa.github.io/Calculadora/)

## Desarrollado con:

* HTML
* CSS
* JavaScript
* jQuery

```javascript
$(function (){
	var screenVal=$("input:text");
	$("input:button").on("click", function(){
		var eachNumber=$(this).val();
		var currentScreen= screenVal.val();
		currentScreen+=eachNumber;
		screenVal.val(currentScreen);
		if($(this).val()=="C"){
			screenVal.val("");
		}
	});
	$("button").click(function(event){
		event.preventDefault();
		screenVal.val(eval(screenVal.val()));
	});
});
```
