Variáveis, são características que damos ao nosso código, sendo estes manipuláveis ao longo do código ou estáticos, ou seja, possuem um valor único e imutável.
		**Exemplo:**
```
			public class App{
				private int minhaVariavel = 0;
				private static int minhaVariavelEstatica = 1;
				
				public static void main(String[] args){
					minhaVariavel = 1;
					minhaVariavelEstatica = 2; //Isto ira dar erro
				}	
			}
```
.                         *Criamos duas variáveis do tipo inteiro, sendo uma mutável e outra estática ou seja imutável, caso tentes mudar o valor da **minhaVariavel**, o programa ira rodar tranquilamente, mas se tentarmos mudar o valor da **minhaVariavelEstatica**, iremos receber um erro no terminal*