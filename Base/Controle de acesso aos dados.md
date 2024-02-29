Modificadores de acesso:
- **Private** (torna restrito apenas a [[Classe]] de origem)
			**exemplo:** 
```
	Numero.java
					public class Numero{
						private int x = 0;
						// acesso cutorizado!
						x = 3;
						}

	App.java
					public class App {
						public static void main(String[] args){
							Numero meuNumero = new Numero();
							//Acesso negado!
							meuNumero.x = 10;
							}
						}
```

- **Public** (Pode ser acessado de qualquer [[Classe]])

- **Protected** mantém o acesso restrito, mas deixa livre o acesso direto para as [[Herança|classes filhas]].

- **Default** (Mantém o acesso restrito apenas as [[Classe|Classes]] que se encontram no mesmo projeto)
			**exemplo:**
```
	Dados.java
					package br.com.skelware.server;
					
					public class Dados {
						String nome;
						String senha;
						String CPF;
					}
	
	App.java - (Acesso autorizado!)
					package br.com.skelware.server;
					
					public class App {
						public static void main(String[] args){
							Dados userJoao = new Dados();
							userJoao.nome = "João Victor";
							userJoao.senha = "123joao";
							userJoao.CPF = "123.456.789-10";
						}				
					}```
	
	App.java - (Acesso negado!)
					package br.com.skelware.backend;
					
					public class App {
						public static void main(String[] args){
							Dados userJoao = new Dados();
							userJoao.nome = "João Victor";
							userJoao.senha = "123joao";
							userJoao.CPF = "123.456.789-10";
						}				
					}
```