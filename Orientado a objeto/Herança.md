Herança é quando uma [[Classe|classe]] filho herda características de uma classe pai, assim adquirindo métodos e [[Atributos|atributos]] desta classe, como por exemplo: [[Classe]] cachorro herda da classe Animal os seguintes [[Atributos|atributos]] **expectativaDeVida**, **especie**, **filo**, **tipoDeAmbiente** e **tipoDeHabitat**, desta forma, não precisamos recriar estes [[Atributos|atributos]] caso fossemos criar outra classe de animal, pois estes compartilham destes mesmos [[Atributos|atributos]].
		**Como usar:**
```
classe Animal (pai)
			public class Animal{
				private int expectativaDeVida;
				private String especie;
				private String filo
				private String tipoDeAnimal
				private String tipoDeHabitat;
			}
```
```
classe Cachorro (filho)
			public class Cachorro extends Animal{
				private String nome;
				private String cor;
			
				public void latir(){
					//reproduzir som do latido
				}
			}
```
 .                        *Para uma [[Classe|classe]] herdar a outra, devesse adicionar **extends** e depois o nome da [[Classe|classe]] como no exemplo acima!*

# Polimorfismo

Quando uma [[Classe|classe]] é uma subclasse (classe filha), ela pode ser considerado o mesmo tipo da superclasse (classe mãe), por exemplo caso tenhamos duas classes filhas que herdam da classe pai **Animal**, caso queiramos utilizar como um parâmetro, basta apenar usar a classe pai que ela poderá receber ambas as classes filhas.
			**Exemplo:**
```
			public class MinhaClasse{
			
				public void meuMetodo(Animal animal){
					//código omitido
				}
			}
```
.                         *No nosso [[Método|método]] **meuMetodo** pede-se um parâmetro do tipo **Animal**, se possuirmos duas classes chamadas respectivamente de **Cachorro** e **Gato** e ambas herdarem a classe **Animal**, elas podem ser passadas como parâmetro dentro do **meuMetodo**.*
```
			public class App{
				public static void main(String[] args){
					MinhaClasse classeDeTeste = new MinhaClasse();
					Cachorro golden = new Cachorro();
					Gato gatoPreto = new Gato();
					
					classeDeTeste.meuMetodo(golden);
					classeDeTeste.meuMetodo(gatoPreto);
				}
			}
```