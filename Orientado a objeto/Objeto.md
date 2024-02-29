Objeto é uma instancia de uma determinada [[Classe]], assim podemos instanciar vários objetos que possuem os mesmos atributos, mas com parâmetros diferentes, por exemplo:
.
		Exemplo:
```
			public class Carro{
				String marca;
				int anoDeLancamento;
				String cor;
				String modelo;	
				int velocidadeMaxima;
			}
```
```
			public class App{
				public static void main(String[] args){
					Carro meuCarro = new Carro();
					meuCarro.marca = "Ford";
					meuCarro.anoDeLancamento = 2020;
					meuCarro.cor = "Preto";
					meuCarro.modelo = "Focus";
					meuCarro.velocidadeMaxima = 200;
				}
			}
```
.                     *O exemplo a seguir é constituído pela [[Classe]] **Carro** e o [[Objeto]] **meuCarro** que é uma instancia da [[Classe]] **Carro**, dessa forma é possível criar várias instancias desta classe com os mesmos atributos, mas com valores diferentes como velocidade máximo indo até o 180 por exemplo.*

Import