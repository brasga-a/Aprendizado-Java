É uma [[Classe|classe]] do java que permite criar listas de um determinado tipo de variável e utilizar os métodos de um determinado elemento ao chama-lo. Podemos usa-lo da seguinte maneira **`ArrayList<Tipo> nomeDoArray = new ArrayList<>()`**.
```
			public class App{
				public static void main(String[] args){
					Filme meuFilme = new Filme();
					ArrayList<Filme> meusFilmes = new ArrayList();
				}
			}
```
.                         *Criamos uma instancia da [[Classe|classe]] filme e logo em seguida criamos uma lista para armazenar nossos filmes*

**Nota:** Existe outra maneira de fazer um Array, que é utilizando `tipo nomeDoArray[]`, porem ele é bastante limitado em relação as suas funções, por isso é sempre recomendado usar o **ArrayList**

#### .add()
- Serve para adicionar um novo item a nossa lista

#### .size()
- Retorna o número de itens existentes dentro da lista

#### .get(index)
- Retorna o item referente ao valor fornecido (index), a posição no java começa a partir do valor 0

#### Outros métodos
[ArrayList Java Documentation](https://docs.oracle.com/javase/8/docs/api/java/util/ArrayList.html)