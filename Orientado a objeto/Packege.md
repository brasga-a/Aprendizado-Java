- **Package**: Para melhor organização das [[classe|classes]], é possível criar um package, uma biblioteca que serve para agrupar [[classe|classes]] que estão relacionadas a alguma funcionalidade. Para adicionar uma [[classe]] ao nosso package criado basta inserir no topo do nosso arquivo o atributo **package br.com.nomedaempresa.nomedoprojeto**
		**Exemplo**: 
```
	Arquivo da nossa Classe User
			
			Package br.com.skelware.account
			
			public class User{
				String nomeDoUsuario;
				int idadeDoUsuario;
				String cpfDoUsuario;
			}
```
.
			*Neste caso estamos inserindo a [[classe]] **user** dentro do nosso package que criamos*

- **Import:** Serve para importar um package (biblioteca) contendo [[Classe|classes]] relacionadas a uma especialidade. Para importar um package devesse colocar no topo do arquivo o seguinte atributo **import br.com.nomedaempresa.nomedoprojeto.nomedaclasse**
		**Exemplo**: 
```
	Arquivo principal do nosso App
			
			import br.com.skelware.account.user
			
			public class App{
				public static void main(String[] args){
					User novoUsuario = new User();
					novoUsuario.nomeDoUsuario = "João Victor";
					novoUsuario.idadeDoUsuario = 20;
					novoUsuario.cpfDoUsuario = "123.456.789.10";
				}
			}
```
.
			*Este import serve para importar a [[Classe]] **user** presente em nosso package dentro de nosso arquivo.*

