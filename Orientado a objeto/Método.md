Método é um bloco de código que um objeto ira realizar como se fosse uma tarefa, como por exemplo em uma classe chamada Filme, podemos ter o método chamado **exibirFichaTecnica** que será responsável por retornar para nós os dados da ficha técnica do filme em questão.
			**Exemplo:**
```
Classe pai
			public class "Titulo"{
				private String nome;
				private String diretor;
				private int anoDeLancamento;
				private String estudioDeProducao;
				private int duracaoEmMinutos;
				
				public int getDuracaoEmMinutos(){
					return duracaoEmMinutos;
				}
				
				//nosso método
				public void exibirFichaTecnica(){
					System.out.println("Nome do filme: " + nomeDoFilme);
					System.out.println("Diretor do filme: " + diretor)
					System.out.println("Estudio produtor: " + estudioDeProducao)
					System.out.println("Ano de lançamento: " + anoDeLancamento)
				}
			}
```
.                            *O método **exibirFichaTecnica** será responsável por executar a tarefa de exibir os dados sobre o objeto (filme) que iremos instanciar*

# Sobrescrever um método

Quando uma [[Classe|classe]] [[Herança|herda]] [[Atributos|atributos]] e métodos de outra [[Classe|classe]] é possível sobrescrever um método para que ele altere o comportamento do método da classe pai. Para fazermos isso, basta reescrever o método na classe filho e adicionar **@override** antes do método.
			**Exemplo:**
```
Classe filho
			public class Serie extends Titulo{
				private int temporadas;
				private int episodiosPorTemporada;
				private int duracaoPorEpisodio;
				
				@override
				public int getDuracaoEmMinutos(){
					return temporadas * episodiosPorTemporada * duracaoPorEpisodio;
				}
			}
```
.                         *Como nossa classe filho é uma série, a duração é calculada de uma maneira diferente do que um filme, assim, sobrescrevemos a função **getDuracaoEmMinutos** mudando o seu valor de retorno para se adequar ao novo formato.*

# Sobrecarga de método

Há uma sobrecarga de método quando copiamos um método e alteramos seu funcionamento, mas preservamos seu nome.
			**Exemplo:**
```
			public class Calculadora{
				private int tempoTotal;
				
				public void incluir(Filme filme){
					tempoTotal += filme.getDuracaoEmMinutos;
				}
				
				public void incluir(Serie serie){
					tempoTotal += serie.getDuracaoEmMinutos;
				}
			}
```
.                         *Neste caso estamos pegando o método **incluir** que possui o parâmetro **[[Classe|Filme]]** e fazendo uma sobrecarga, criando um outro método de mesmo nome que executa a mesma função, porem este possui o parâmetro **[[Classe|Série]]**.*