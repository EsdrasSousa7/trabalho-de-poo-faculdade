<h1 align="center">Trabalho de Programação Orientada a  Objetos</h1>

<h2>⚡1º : Considerando os conceitos básicos de Orientação a Objetos, explique o significado dos conceitos abaixo:</h2>

<h3> 1. Encapsulamento: É A forma de dividir as tarefas no codigo de uma forma organizada para que seja evitado repetição de codigos. </h3>
<h5> EXEMPLO: </h5>
##### Em um programa que adiciona nomes em uma lista sem uso de encapsulamento, toda vez q quiser digitar o nome e armazenar
##### terá que reescrever o mesmo codigo, se for necessario adicionar 100 nomes, o mesmo codigo será reescrito 100 vezes.
#### EXEMPLO:    
     public class Exemplo {
	
	public static void main(String[] args){
		Scanner lerNome = new Scanner(System.in);
		ArrayList<String> ListaDeNomes = new ArrayList<String>();
		
		System.out.println
		("Qual nome quer adicionar na Lista?"); //mostra na tela uma pergunta
		String nome1 = lerNome.next();          //armazena a resposta em uma variavel                   
		ListaDeNomes.add(nome1);                //adiciona na lista
		
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
     
     

 Com o encapsulamento, evita-se linhas de codigos repetidos com a seguinte logica:
     
     Para adicionar um nome em uma lista temos 2 tarefas principais:
         -> 1- saber qual o livro que deve ser armazenado.
         -> 2- armazenar o livro em questão.

     Todas as vezes que tiver que fazer algo repetitivo,podemos criar "metodos" que cada tarefa separadamente no codigo:
      
     metodo 1: ver qual o livro
     
     metodo 2: armazenar o livro

  
 Assim, em vez de ter longas linhas de codigos repetidos, pode simplesmente chamar o respectivo metodo que faz a função que está sendo necessaria
    
    
    2. Herança
    
    
    3. Polimorfismo
    
    4. Atributos e Métodos
    
    5. Atributos e Métodos Estáticos





