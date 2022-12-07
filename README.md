<h1 align="center">Trabalho de Programação Orientada a  Objetos</h1>

<h2>⚡1º : Considerando os conceitos básicos de Orientação a Objetos, explique o significado dos conceitos abaixo:</h2>

- <h3> 1. Encapsulamento:  💥</h3>

``
Tem o princípo de dividir tarefas em um codigo de maneira organizada de forma que evite repetição de codigos.
      
      Exemplo :
      Temos um programa que adiciona nomes em uma lista.
        Nesse programa temos o seguinte algoritmo:
	                                        ->Saber qual nome tem que adicionar;
						->Adicionar o nome
      
      Sem uso de encapsulamento, todas as vezes q for preciso fazer o uso desse algoritmo será necessário repetir o mesmo codigo. 
      Se for necessario adicionar 100 nomes, o mesmo codigo será reescrito 100 vezes.
      
      Mas caso você faça uso da prática de encapsulamento, o algoritmo em questão se tornará um "método", com isso sempre que for necessário o uso desse algoritmo em vez de repetir codigo, será preciso apenas "chamar o método".
      
</br>
________________________________________________________________________________________________________________
</br>

- <h3>2. Herança:  💫</h3>
> <p>É a forma de classes compartilharem atributos e metodos entre si de uma forma hierarquica:</p>

> <p>Classe que vai compartilhar : base </p>

> <p>Classe que vai receber : derivada </p>
  
      public class Base {    //classe Base
	
	int numero  = 1;                                 //2 variaveis na classe Base
	String nome = "arroz";   
	
     }
     
________________________________________________________________________________________________________________
     
     public class Derivada extends Base{                //classe Derivada herda Base
	public void derivada() {
		
		System.out.println(numero + nome);      //pode fazer o uso das variaveis declaradas em Base
		
	}
    }
- <h3>3. Polimorfismo  🐸</h3>
     
    
    
    
    
    4. Atributos e Métodos
    
    5. Atributos e Métodos Estáticos





