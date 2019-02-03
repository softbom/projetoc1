import java.util.Scanner;


public class AtividadeC1 {
	
	static Scanner s = new Scanner(System.in);
    static int inteiros, idade, valor;
    static char caract;

//sub1
static void Entrada() {
	//sub1
	    Scanner s = new Scanner(System.in);
        System.out.println("--  Olá seja bem-vindo!");
		System.out.println("DIgite seu nome: ");
	    String nome = s.nextLine();
		System.out.println("Digite sua idade: ");
	    idade = s.nextInt();
	    if(idade < 18 ) {
			System.out.println( nome + " Você não pode acessar essa atividade por ser menor que a idade permitida!");
		}else {
			System.out.println("Acesso liberado!");
            System.out.println();
	        System.out.println("---- " + nome + " Seja bem vindo ao MENU do programa ! ---");
	        System.out.println();
            System.out.println("----- " + nome + " Você irá se surpreender ---- ");
            System.out.println();
         // Opções de ecolha
    	    OpçõesEscolha();
		}
	    
}
//sub2
static void Atividade4() {
	Scanner s = new Scanner(System.in);
	float numero1, numero2;
	char operacao;
	    //saídas de dados
	System.out.print("Olá seja bem-vindo a calculadora virtual !");
	System.out.println();
	
	System.out.print("Escolha sua operação:  [+, -, *, ])");
	operacao = s.nextLine().charAt(0);
	
	System.out.print("Escolha o primeiro numero: ");
	numero1 = s.nextFloat();
	System.out.print("Escolha o segundo numero: ");
	numero2 = s.nextFloat();
	System.out.println();
	
	   switch(operacao) {
		case '+':
			System.out.printf("O resultado da soma e: " + (numero1 + numero2));
			break; 
			
		case '-':
			System.out.printf("O resultado da subtração e: " + (numero1 - numero2));
			break;
			
		case '*':
			System.out.printf("O resultado da multiplicação e: " + (numero1 * numero2));
			break;
			
		case '/':
			System.out.printf("O resultado da divisão e: " + (numero1 / numero2));
			break;
			
		default:
			System.out.printf("Opção inválida!");
	   }
}
//sub3
static void A3() {
    Scanner s = new Scanner(System.in);
	System.out.println("DIgite seu nome completo");
    String nome = s.nextLine();
    System.out.println();
    System.out.println("DIgite sua idade: ");
    idade = s.nextInt();
    System.out.println(" " + nome + " você tem " + idade + " anos");
	
	
				
}
//sub4
static void Atividade5() {
  Scanner s  = new Scanner(System.in);
  System.out.println("Olá seja bem-vindo!: ");
  System.out.println();
  System.out.println("Escreva seu nome: ");
  String nome = s.nextLine();
  System.out.println();
  System.out.println("Escreva seu sobrenome: ");
  String sobrenome = s.nextLine();
  System.out.println();
  System.out.println("Escreva sua idade: ");
  int idade = s.nextInt();
  System.out.println();
  System.out.println("Escreva sua altura: ");
  double altura = s.nextDouble();
  System.out.println();
  System.out.println(nome + " " + sobrenome + " você tem " + idade + " anos e mede " + altura + " de altura!");
  
} 
//sub5
static void Atividade6Ex3() {
	Scanner s  = new Scanner(System.in);
	double nota1, nota2, nota3, nota4, media;
	System.out.println("Olá seja bem-vindo ao Programa de calculo média!");
	System.out.println("Insira a primeira nota: ");
	nota1 = s.nextDouble();
	System.out.println("Insira a segunda nota: ");
	nota2 = s.nextDouble();
	System.out.println("Insira a terceira nota: ");
	nota3 = s.nextDouble();
	System.out.println("Insira a quarta nota: ");
	nota4 = s.nextDouble();
	
    media = (nota1  + nota2 + nota3 + nota4) / 4;
    
    System.out.println("O resultado da média do aluno é: " + media);
	
}
//sub6
static void Atividade6Ex4() {
	
  for(int numero = 100; numero <= 200; numero++ ) {
  System.out.println("Bilhete Nº " + numero); 
	 
  }
  
	
}
//sub7
static void OpçõesEscolha() {
	Scanner s  = new Scanner(System.in);
	System.out.println("Escolha uma das opções abaixo: " );
    System.out.println();
    System.out.println("-Opção 1- Atividade 3");
    System.out.println();
    System.out.println("-Opção 2- Atividade 4");
    System.out.println();
    System.out.println("-Opção 3- Atividade 5");
    System.out.println();
    System.out.println("-Opção 4- Atividade 6 Ex: 3");
    System.out.println();
    System.out.println("-Opção 5- Atividade 6 Ex: 4");
    System.out.println();
    System.out.println("-Opção 6- Atividade 7");
    System.out.println();
    System.out.println("-Opção 7- Atividade 8");
    System.out.println();
    System.out.println("-Opção 8- Atividade 9");
    System.out.println();
    System.out.println("Escreva aqui sua escolha: ");
    valor = s.nextInt();
    
	
}
//sub8
static void Atividade7() {
	Scanner s  = new Scanner(System.in);
	System.out.println("seja be vindo ao menu do cliente!");
	System.out.println();
	System.out.println("Escolha uma das opções abaixo: " );
    System.out.println();
    System.out.println("-Opção 1- Cadastrar Cliente: ");
    System.out.println();
    System.out.println("-Opção 2- Alterar Cliente: ");
    System.out.println();
    System.out.println("-Opção 3- Excluir Cliente: ");
    System.out.println();
    System.out.println("-Opção 4- Sair ");
    System.out.println("Escreva sua escolha: ");
    valor = s.nextInt();
    
    switch(valor) {
    
    case 1:
    	System.out.println("Você escolheu a opção Cadastrar Cliente!");
    	break;
    case 2:
    	System.out.println("Você escolheu a opção Alterar Cliente!");
    	break;
    case 3:
    	System.out.println("Você escolheu a opção Excluir Cliente!");
    	break;
    case 4:
    	System.out.println("Você escolheu a opção  Sair!");
        break;
    default:
    	System.out.println("Opção Inválida!");
    }
}
//sub9
static void Atividade8() {
	Scanner s  = new Scanner(System.in);
	int[] vetor = new int[10];
	System.out.println("Digite um numero: ");
	for(int i = 0; i < 10; i++) {
		System.out.println("vetor["+i+"]: ");
		vetor[i] = s.nextInt();
	}
	for(int i = 0; i < 10; i++) {
		System.out.println(vetor[i]);
	}

}
//sub10
static void Atividade9() {
	System.out.println("------ Empresa 123 ------");
	System.out.println("------ Data: 13/12/2018 ------");
	System.out.println("------ Fincionário: José ------");
	System.out.println();
	System.out.println("CUPOM FISCAL");
	System.out.println();
	System.out.println("TOTAL R$: R$ 3000,00");
	System.out.println("Dinheiro: R$ 2600,00");
	System.out.println("Troco:    R$  400,00");
	
}
//sub11
static void CorpoPrograma() {
	
	switch( valor) {
	
	case 1:
		 System.out.println("-Opção 1 - Programa Atividade 3 ");
		 System.out.println();
         A3();
	break;
	
	case 2:
		System.out.println("-Opção 2 - Programa Atividade 4 ");
		System.out.println();
		Atividade4();
		   
	 break;
	 
	 case 3:
		 System.out.println("-Opção 3 - Programa Atividade 5 ");
		 System.out.println();
	     Atividade5();
	 break;
	 
	 case 4:
		 
		 System.out.println("-Opção 4 - Programa Atividade 6 Exercício 3"); 
		 System.out.println();
		 Atividade6Ex3();
		 break;
		 
	 case 5:
		 System.out.println("-OPção 5 - Programa Atividade 6 Exercício 4");
		 Atividade6Ex4();
		 break;
		 
	 case 6:
		 System.out.println("-Opção 6 - Programa Atividade 7");
		 Atividade7();
		 break;
		 
	 case 7:
		 System.out.println("- Opção 7 - Programa Atividade 8");
		 Atividade8();
		 break;
		 
	 case 8:
		 System.out.println("-Opção 8 - Programa Atividade 9");
		 Atividade9();
		 break;
		
     default:
	     System.out.println("OPÇÃO INVÁLIDA!");
	
	}
		 
}
//sub12
static void Chamada() {
	Entrada();
}

  public static void main(String[] args) {
    	
     Chamada();
    if(idade < 18 ) {
		System.out.println();
	}else {
    
     CorpoPrograma();
	}
    	
    }
  }
 
