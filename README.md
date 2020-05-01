# waitForGlobal
Javascript para aguardar pelas globais serem instanciadas

##Exemplo de Uso
```JS
waitForGlobal("jQuery", function() {
	waitForGlobal("PagarMeCheckout", function() {
		waitForGlobal("PagarMeCheckoutLoadedRetail", function() {
			console.log("Carregado esse item após PagarMeCheckoutLoadedRetail, PagarMeCheckout e jQuery prontos nessa ordem");
		});
	});
});
```
