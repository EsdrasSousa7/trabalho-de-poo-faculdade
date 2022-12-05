<h1 align="center">Trabalho de Programação Orientada a  Objetos</h1>

<h2>⚡1º : Considerando os conceitos básicos de Orientação a Objetos, explique o significado dos conceitos abaixo:</h2>

- <h3> 1. Encapsulamento:</h3>
> <p> É A forma de dividir tarefas no codigo de uma forma organizada para evitar repetição de codigos.</p>

<p>   Em um programa que adiciona nomes em uma lista sem uso de encapsulamento, toda vez q quiser digitar o nome e armazenar
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
<p>Podemos ver acima, q as mesmas linhas de codigos estão se repetindo várias vezes, agora veja como seria com metodos ( encapsulament ) <p>
	
	public static void main(String[] args) {
		while( ListaDeNomes.size() < = 10 )
		adicionaConta();                                          //chamando metodo adicionarConta
	}
	
					       
	public static void adicionaConta() {                              //metodo pra adicionar nome na lista
		System.out.println("Qual nome quer adicionar na Lista?");
		String nome2 = lerNome.next();
		ListaDeNomes.add(nome2);
	}
					       
<p>Com o encapsulamento, evita-se linhas de codigos repetidos com a seguinte logica:</p>
     
<p>Para adicionar um nome em uma lista temos 2 tarefas principais:</p>
<p> -> 1- saber qual o livro que deve ser armazenado.</p>
<p> -> 2- armazenar o livro em questão.</p>

<p>Todas as vezes que tiver que fazer algo repetitivo,podemos criar "metodos" para cada tarefa separadamente</p>
    2. Herança
    
    
    3. Polimorfismo
    
    4. Atributos e Métodos
    
    5. Atributos e Métodos Estáticos





