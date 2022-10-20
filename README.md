# JS exercises review
1. Realizar un programa para una tienda de coches. Si el coche a la venta es un ford fiesta, el descuento es de un 5%. Si el coche a la venta es un ford focus, el descuento es del 10%. 
	El usuario introduce el artículo y el programa saca el descuento correspondiente por pantalla. (prompt)

```javascript
let marca, modelo, descuento = 0;
marca = prompt("Marca?", "0");
modelo = prompt("Modelo?", "0");

if((marca == "ford") $$ (modelo == "fiesta")){
descuento = 5;
}
if((marca == "ford") && (modelo == "focus")){
descuento = 10;
}
documento.write(`<h3>Su descuento es ${descuento} </h3>`);
```

2. Escriba una función JavaScript que devuelva una cadena pasada con letras en orden alfabético. Cadena de ejemplo : 'webmaster' 
	Resultado esperado : 'abeemrstw' 
	Nota: Asuma que los símbolos de puntuación y números no están incluidos en la cadena pasada.
```javascript
function alphabet_order(str){  
	return str.split('').sort().join('');
} 
document.write(alphabet_order("webmaster"));</script>
```

3. Escriba una función de JavaScript que acepte una cadena como parámetro y cuente el número de vocales dentro de la cadena. 
	Nota: Como la letra "y" puede considerarse tanto una vocal como una consonante, aquí no contamos "y" como vocal. 
	Datos de ejemplo y salida: Cadena de ejemplo : '' The quick brown fox"
	Resultado esperado: 5
```javascript
function vowel_count(str1){

	var vowel_list = 'aeiouAEIOU';
	
	var vcount = 0;

	for(var x = 0; x < str1.length ; x++){
	
		if (vowel_list.indexOf(str1[x]) !== -1){
	
		vcount += 1;
	
		}
	}

return vcount;
}
Document.write(vowel_count("The quick brown fox"));
```

4. Escribe un programa en JavaScript para calcular la multiplicación y la división de dos números (input del usuario). Ejemplo:
![[Captura de Pantalla 2022-10-20 a las 9.57.52.png]]
