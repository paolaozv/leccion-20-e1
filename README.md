# leccion-20-e1

###Código inicial

``` javascript

1. var num2 = 0;
2. function suma(num1) {
3. 	  return function(num2) {
4. 	  return num1 + num2;
5.	  }
6. }
7. 
8. var suma2 = suma(2);
9. console.log(suma2(5)); // Debería mostrar 7 de resultado
10. 
11. var suma12 = suma(12);
12. console.log(suma12(76)) // Debería mostrar 88 de resultado.
```

###Código final

``` javascript
1. function suma(num1) {
2.	  return function(num2) {
3.	  return num1 + num2;
4.	  }
5. }
6.
7. var suma2 = suma(2);
8. console.log(suma2(5)); // Debería mostrar 7 de resultado
9. 
10. var suma12 = suma(12);
11. console.log(suma12(76)) // Debería mostrar 88 de resultado.
```

###Solución

En la línea 1 del código inicial la variable num2 se define e inicializa en cero, pero en el código final se omite ese línea 1 porque al inicializarla de manera global, en la función anónima ya no la usa y sería innecesario colocarla.
