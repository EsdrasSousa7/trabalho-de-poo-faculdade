<h1 align="center">Trabalho de Programação Orientada a  Objetos</h1>

<h2>⚡1º- Considerando os conceitos básicos de Orientação a Objetos, explique o significado dos conceitos abaixo:</h2>

- <h3>1. Encapsulamento:  💥</h3>
      
      💠Tem o princípo de dividir tarefas em um codigo de maneira organizada.
      
      💠Evita de ter muitos codigo repetidos.
      
      💠Por ter tarefas divididas, a manutenção do codigo é mais eficiente.
      
      ➡️O encapsulamento consiste em separar as tarefas em "metodos".
      
      ➡️Com isso sempre que for realizar uma tarefa, será necessário apenas chamar o metodo.
</br>
________________________________________________________________________________________________________________
</br>

- <h3>2. Herança:  💫</h3>

      ➡️A herança permite que Classes compartilhem características e ações com outras.

       💠Classe que vai compartilhar: Se chama base;
       💠Classe que vai receber: Se chama derivada;
      
      ❓exemplo:
         💠 Uma Classe com nome Pessoa que possui:
	     💠características: nome e sobrenome;
	     💠ações: andar e falar;
	     
      ➡️A Classe que recebe herança de Pessoa também vai ter nome e sobrenome,andar e falar.
</br>
________________________________________________________________________________________________________________
</br>

- <h3>3. Polimorfismo  🐸</h3>
     
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
</br>
________________________________________________________________________________________________________________
</br>

- <h3>4. Atributos e Métodos 🍀</h3>

      🟢Atributos são características de objetos como por exemplo:
         💠Carro -> tem roda,volante,banco.
         💠Porta -> tem cor,material,espessura.
	  
	     ❓ roda, volante, banco, cor, material eespessura são atributos.
	 
      🟢Métodos são ações que o objeto pode fazer:
         💠Carro -> acelerar,frear,ligar,desligar.
         💠Porta -> abrir,fechar.
    
               ❓acelerar,frear,ligar,desligar,abrir e fechar são métodos
</br>
________________________________________________________________________________________________________________
</br>
		      
- <h3>5. Atributos e Métodos Estáticos 🍁</h3>

       Atributos e Métodos Estáticos são ações e características de uso exclusivo da Classe.
</br>
________________________________________________________________________________________________________________
</br>


<h2>🔅2º- Diferencie os mecanismos de sobrescrita e sobrecarga, demonstrando cenário de uso de cada um desses.</h2>

<h4 align="center">⭕Sobrescrita⭕</h4>

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
      
        🔸 public class Classe2 extends Classe1{
	🔸
	🔸   @Override
	🔸   public void mensagem() {
	🔸	System.out.println("outra mensagem");
	🔸   }
	🔸
        🔸}
      

      💠Agora dessa forma o método mensagem() em Classe2 está sendo sobreescrito no de Classe1
      
      🟢Então se tentar imprimir mensagem() em ambas:
        🔺Classe1 mostrará "mensagem"
	🔺Classe2 mostrará "outra mensagem"
           

