<h1 align="center">Trabalho de Programação Orientada a  Objetos</h1>

<h2>⚡1º- Considerando os conceitos básicos de Orientação a Objetos, explique o significado dos conceitos abaixo:</h2>
</br>
<h3>Encapsulamento:  💥</h3>
      
       ⠀⠀
      💠Tem o princípo de dividir tarefas em um codigo de maneira organizada.
      
      💠Evita de ter muitos codigo repetidos.
      
      💠Por ter tarefas divididas, a manutenção do codigo é mais eficiente.
      
      ➡️O encapsulamento consiste em separar as tarefas em "metodos".
      
      ➡️Com isso sempre que for realizar uma tarefa, será necessário apenas chamar o metodo.
      ⠀⠀
      
</br>
<h1></h1>
</br>

<h3>Herança:  💫</h3>

      ⠀⠀
      ➡️A herança permite que Classes compartilhem características e ações com outras.

       💠Classe que vai compartilhar: Se chama base;
       💠Classe que vai receber: Se chama derivada;
      
      ❓exemplo:
      
          💠Uma Classe com nome Pessoa que possui:
          💠características: nome e sobrenome;
          💠ações: andar e falar;
	     
      ➡️A Classe que recebe herança de Pessoa também vai ter nome e sobrenome,andar e falar.
      ⠀⠀

</br>
<h1></h1>
</br>

<h3>Polimorfismo  🐸</h3>
     
      ⠀⠀
      🟢Poli = muitas;  
      🟢morfo = formas
      
      ➡️Poliformifismo é quando algo pode fazer a mesma coisa de formas diferentes.
      
      ❓exemplo:
      
           💠Fazer um trabalho de faculdade tem varias formas de fazer essa ação:
           💠Estudando pra saber resolver.
           💠Pedindo ajuda.
           💠Copiando de outra pessoa.
           💠Fazer de forma errada
	 
      🟢Temos o mesmo nome pra um comportamento ( Fazer um trabalho de faculdade ) e varías formas de fazer.
      ⠀⠀

</br>
<h1></h1>
</br>

<h3>Atributos e Métodos 🍀</h3>

      ⠀⠀
      🟢Atributos são características de objetos como por exemplo:
      
         💠Carro -> tem roda,volante,banco.
         💠Porta -> tem cor,material,espessura.
	  
	     ❓ roda, volante, banco, cor, material eespessura são atributos.
	 
      🟢Métodos são ações que o objeto pode fazer:
      
         💠Carro -> acelerar,frear,ligar,desligar.
         💠Porta -> abrir,fechar.
    
               ❓acelerar,frear,ligar,desligar,abrir e fechar são métodos
	       ⠀⠀

</br>
<h1></h1>
</br>
		      
<h3>Atributos e Métodos Estáticos 🍁</h3>

 
      ⠀⠀
      ➡️Atributos e Métodos Estáticos são ações e características de uso exclusivo da Classe.
      ⠀⠀

</br>
<h1></h1>
</br>


<h2>🔅2º- Diferencie os mecanismos de sobrescrita e sobrecarga, demonstrando cenário de uso de cada um desses.</h2>
</br>
<h4 align="center">⭕Sobrescrita⭕</h4>


       ⠀⠀
      ➡️Sobrescrita é quando se tem métodos com a mesma assinatura em classes diferentes.
      ➡️Quando não se quer herdar o método do jeito da outra classe, se "sobrescreve" o mesmo.
      
        🟢Mesma assinatura: quando tem a mesma quantidade de parametros e sãp do mesmo tipo.
      
      ❓exemplo pratico:
      
        💠Classe1 com uma método "mensagem" que mostra uma string:
      
            🔸public class Classe1 {
            🔸   public void mensagem() {
            🔸       System.out.println("mensagem");
            🔸  }
            🔸}
       
        💠Classe2 derivada de Classe1:
      
            🔸 public class Classe2 extends Classe1{
            🔸 }
      
      💠Como a Classe2 herda de classe1, ela tambem possui o método mensagem().
      
      🟢Então se tentar imprimir mensagem() em ambas,ambas vão retornar a mesma coisa!
      
      ➡️Agora com Sobrescrita:
      
        💠Classe1 com uma método "mensagem" que mostra uma string:
      
            🔸public class Classe1 {
            🔸   public void mensagem() {
            🔸       System.out.println("mensagem");
            🔸  }
            🔸}
	
        💠Classe2 derivada de Classe1:
      
            🔸public class Classe2 extends Classe1{
            🔸
            🔸   @Override
            🔸   public void mensagem() {
            🔸	System.out.println("outra mensagem");
            🔸   }
            🔸}
      

      💠Agora dessa forma o método mensagem() em Classe2 está sendo sobreescrito no de Classe1
      
      🟢Então se tentar imprimir mensagem() em ambas:
      
        🔺Classe1 mostrará "mensagem"
	🔺Classe2 mostrará "outra mensagem"
	⠀⠀

</br>
<h1></h1>
</br>

<h4 align="center">❌Sobrecarga❌</h4>


     ⠀⠀
     ➡️Sobrecarga é quando se tem métodos com assinaturas diferentes em classes iguais.
     
       🟢Mesma assinatura: quando tem a mesma quantidade de parametros e sãp do mesmo tipo.
     
     ❓exemplo pratico:
      
            🔸public class Classe {
            🔸
            🔹🔹Atributos:
            🔸   public String nome,sobrenome,estadoCivil;
            🔸   public int idade,cpf;
            🔸
            🔹🔹método que recebe 2 string:
            🔸   public Classe(String nome,String sobrenome) {
            🔸      this.nome = nome;
            🔸      this.sobrenome = sobrenome;
            🔸   }
            🔸
            🔹🔹método que recebe 2 inteiros:
            🔸   public Classe(int idade,int cpf) {
            🔸      this.idade = idade;
            🔸      this.cpf = cpf;
            🔸   }
            🔸
            🔹🔹método que recebe 1 String
            🔸   public Classe(String estadoCivil) {
            🔸      this.estadoCivil = estadoCivil;
            🔸   }
            🔸
            🔸}
      
      💠No codigo acima tem 3 métodos com o mesmo nome, porém, cada um recebe parâmetros diferentes.
        
      ❓Exemplo da utilização:
      
            🔸public class Principal {
            🔸
            🔸   public static void main(String[] args) {
            🔸
            🔹🔹🔹Chama o construtor Classe pra criar um novo objeto com os parâmetros: 18 e 06592349222.
            🔸      Classe teste = new Classe(18,06592349222);
            🔸         System.out.println(teste);
            🔸   }
            🔸}
	 
      💠Quando se cria um novo objeto, a Classe prorcura um construtor compatível.
      
        🟢Ele verifica o primeiro metodo disponível:
	
	    🔹🔹metodo que recebe 2 string:
            🔸   public Classe(String nome,String sobrenome) {
            🔸      this.nome = nome;
            🔸      this.sobrenome = sobrenome;
            🔸   }
	 
	🟢Como ele recebe 2 strings e o construtor foi chamado com 2 inteiros ele tenta o próximo método:
	
	    🔹🔹metodo que recebe 2 inteiros:
            🔸   public Classe(int idade,int cpf) {
            🔸      this.idade = idade;
            🔸      this.cpf = cpf;
            🔸   }
	 
	🟢Esse método em questão aceita 2 inteiros, então é esse que vai ser usado.
	
      ➡️Quando se chama um construtor ele verifica os metodos disponível em sequência.
      
      ➡️Quando um método não é compativel ele fica "sobrecarregado",então verifica o próximo.
      ⠀⠀
</br>
<h1></h1>
</br>   

<h2>⚡3º-A partir do diagrama abaixo, implemente a estrutura de classes.:</h2>
</br>
<p align="center">
<img src="https://github.com/isonhar/trabalho-de-poo-faculdade/blob/main/extra/img%203%20questao.png">
</p>
      
 ➡️Pessoa:
	 
    🔸public class Pessoa {
    🔸   protected String nome;
    🔸   public Pessoa(String nome) {
    🔸      this.nome = nome;
    🔸   }
    🔸   public void setNome(String nome) {
    🔸	this.nome = nome;
    🔸   }
    🔸   public String getNome() {
    🔸	return nome;
    🔸   }
    🔸   public String toString() {
    🔸	return "\n" + nome;
    🔸   }
}
	
➡️Pessoa Física:

    🔸public class PessoaFisica extends Pessoa {
    🔸   protected String cpf,sobrenome;
    🔸   protected String tipo = "Pessoa tipo Fisica";
    🔸   public PessoaFisica(String nome, String sobrenome, String cpf) {
    🔸      super(nome);
    🔸	this.cpf = cpf;
    🔸	this.sobrenome = sobrenome;
    🔸   }
    🔸   public String getSobrenome() {
    🔸	return sobrenome;
    🔸   }
    🔸   public void setSobrenome(String sobrenome) {
    🔸	this.sobrenome = sobrenome;
    🔸   }
    🔸   public String getCpf() {
    🔸	return cpf;
    🔸   }
    🔸   public void setCpf(String cpf) {
    🔸	this.cpf = cpf;
    🔸   }
    🔸   public String toString() {
    🔸	return  "\n"
    🔸             + tipo 
    🔸             +"\nNome: " + this.getNome()
    🔸             +"\nSobrenome: " + this.getSobrenome()
    🔸             +"\nCpf: " + this.getCpf();
    🔸   }
    🔸}

➡️Pessoa Jurídica:

    🔸public class PessoaJuridica extends Pessoa {
    🔸   private String cnpj,razaoSocial;
    🔸   private String tipo = "Pessoa tipo juridica";
    🔸   public PessoaJuridica(String nome, String cnpj, String razaoSocial) {
    🔸      super(nome);
    🔸	this.cnpj = cnpj;
    🔸	this.razaoSocial = razaoSocial;
    🔸   }
    🔸   public String getRazaoSocial() {
    🔸	return razaoSocial;
    🔸   }
    🔸   public void setRazaoSocial(String razaoSocial) {
    🔸	this.razaoSocial = razaoSocial;
    🔸   }
    🔸   public String getCnpj() {
    🔸	return cnpj;
    🔸   }
    🔸   public void setCnpj(String cnpj) {
    🔸	this.cnpj = cnpj;
    🔸   }
    🔸   public String toString() {
    🔸	return  "\n"
    🔸	       + tipo 
    🔸	       +"\nNome: " + this.getNome()
    🔸	       +"\nSobrenome: " + this.getCnpj()
    🔸	       +"\nCpf: " + this.getRazaoSocial();
    🔸   }
    🔸}
       
</br>
<h1></h1>
</br>

<h2>💲4º-Modifique a o projeto banco (abordado em sala de aula) para que o cliente usado seja um tipo PessoaFisica ou PessoaJuridica.</h2>
</br>

➡️[Link para 4º questão](https://github.com/isonhar/trabalho-de-poo-faculdade/tree/main/quest%C3%A3o%204/banco/src/banco)

</br>
<h1 align="center">〰️〰️〰️〰️〰️〰️〰️〰️〰️〰️</h1>
</br>


 
