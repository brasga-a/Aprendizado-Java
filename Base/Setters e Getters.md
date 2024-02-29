- **Setter:** Serve para atribuir um valor a um [[Controle de acesso aos dados|parâmetro protegido]].
		Exemplo:
```
			public class Filme{
				Private String nomeDoFilme;
			
				public void setNome(String nomeDoFilme){
					this.nomeDoFilme = nomeDoFilme;
				}			
			}
```
.                    *Criamos um [[Método|método]] chamado **setNome** onde o [[Controle de acesso aos dados|atributo protegido]] **nomeDoFilme** recebe o valor do parâmetro **nome** tipo String que iremos fornecer.* 

***this** serve para referir o [[Atributos|atributo]] ao qual está conectado, isto serve para quando temos [[Atributos|atributos]] que possuem o mesmo nome que nosso parâmetro*

- **Getter:** Serve para pegar o valor de um [[Controle de acesso aos dados|parâmetro protegido]].
```
			public class Filme{
				Private String nomeDoFilme;
						
				public String getNome(){
					return nomeDoFilme;
				}			
			}
```
.                     *Criamos um [[Método|método]] do tipo String chamado **getNome** que retorna o valor do [[Atributos|atributo]] **nomeDoFilme***.