<h1 align="center">Trabalho de Programação Orientada a  Objetos</h1>

<h2>⚡1º : Considerando os conceitos básicos de Orientação a Objetos, explique o significado dos conceitos abaixo:</h2>

- <h3> 1. Encapsulamento:  💥</h3>
> <p> É a forma de dividir tarefas no codigo de uma forma organizada para evitar repetição de codigos.</p>

> <p>   Em um programa que adiciona nomes em uma lista sem uso de encapsulamento, toda vez q quiser digitar o nome e armazenar
terá que reescrever o mesmo codigo, se for necessario adicionar 100 nomes, o mesmo codigo será reescrito 100 vezes. </p>

     public class Exemplo {	
	public static void main(String[] args){
		Scanner lerNome = new Scanner(System.in);
		ArrayList<String> ListaDeNomes = new ArrayList<String>();
		
		System.out.println
		("Qual nome quer adicionar na Lista?");     //mostra na tela uma pergunta
		String nome1 = lerNome.next();              //armazena a resposta em uma variavel                   
		ListaDeNomes.add(nome1);                    //adiciona na lista
		
		System.out.println("Qual nome quer adicionar na Lista?");
		String nome2 = lerNome.next();
		ListaDeNomes.add(nome2);
		
		System.out.println("Qual nome quer adicionar na Lista?");
		String nome3 = lerNome.next();
		ListaDeNomes.add(nome3);
		
		System.out.println("Qual nome quer adicionar na Lista?");
		String nome4 = lerNome.next();
		ListaDeNomes.add(nome4);
		
		lerNome.close();
	}
    }
> <p>Podemos ver acima,que está se repetindo os mesmos codigos várias,agora veja como seria com metodos(encapsulamento) <p>
	
	public static void main(String[] args) {
		while( ListaDeNomes.size() < = 10 )
		adicionaConta();                                          //chamando metodo adicionarConta
	}
	
________________________________________________________________________________________________________________
					       
	public static void adicionaConta() {                              //metodo pra adicionar nome na lista
		System.out.println("Qual nome quer adicionar na Lista?");
		String nome2 = lerNome.next();
		ListaDeNomes.add(nome2);
	}
					       
> <p>Com o encapsulamento, evita-se linhas de codigos repetidos com a seguinte logica:</p>
     
> <p>Para adicionar um nome em uma lista temos 2 tarefas principais:</p>
	
> <p> -> 1- saber qual o livro que deve ser armazenado.</p>
	
> <p> -> 2- armazenar o livro em questão.</p>

> <p>Todas as vezes que tiver que fazer algo repetitivo,podemos criar "metodos" para cada tarefa separadamente</p>
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





