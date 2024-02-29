Classe é um conjunto de atributos e métodos que criamos quando queremos criar vários [[Objeto|Objetos]] que compartilham de certas funcionalidades básica, como por exemplo um carro. Um carro possui [[Atributos|atributos]] básicos e comuns entre si, como cor, velocidade, nome e etc..., sendo assim podemos criar uma classe chamada carro que ira compartilhar essas informações e assim instanciamos um [[Objeto|objeto]] desta classe. 
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
.                     *O exemplo a seguir é constituído pela [[Classe]] **Carro** e o [[Objeto]] **meuCarro** que é uma instancia da [[Classe]] **Carro**, dessa forma é possível criar várias instancias desta classe com os mesmos [[Atributos|atributos]], mas com valores diferentes como velocidade máximo indo até o 180 por exemplo*
