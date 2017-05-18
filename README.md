# FaculTrab
Trabalho da calculadora de algoritmos

package trabalhoalgoritmos;

import java.util.Scanner;

public class TrabalhoAlgoritmos 
{
    //Scanner
    public Scanner ler = new Scanner(System.in);
    
    //BOOLS
    public boolean running;
    
    //INTS
    public int menuValor;
    public int vectorSize1, vectorSize2;
    
    //VETORES
     public int[] vector1 = new int[vectorSize1];
     public int[] vector2 = new int[vectorSize2];
    
    

    public void printMenu()
    {
         System.out.printf("======== MENU DE OPÇÕES ======== \n"
                    + "–\n"
                    + "1 - Preencher vetores \n"
                    + "–\n"
                    + "2 - Imprimir vetores \n"
                    + "–\n"
                    + "3 - Eliminar elemento do vetor \n"
                    + "–\n"
                    + "4 - Pesquisar elemento nos vetores \n"
                    + "–\n"
                    + "5 - Ordenar os vetores \n"
                    + "–\n"
                    + "6 - Calcular operações matemáticas \n"
                    + "–\n"
                    + "7 - Calcular métodos estatísticos \n"
                    + "–\n"
                    + "8 - Total de elementos válidos \n"
                    + "-\n"
                    + "9 - Sair"
                    + "\n ==================================="
                    + "\n Escolha sua opção : ");
         
         menuValor = ler.nextInt();
         
         options();
    }
    
    public void options()
    {
         switch(menuValor)
         {
             case 1:
                 fillVector();
                 break;
             case 2:    
             case 3:
             case 4:
             case 5:
             case 6:
             case 7:
             case 8:
             case 9:
                 System.out.println("Bye bye");
                 running = false;
             default:
                 System.out.printf("ERROR... Oh não!!!"
                         + "\nPor favor insira um valor valido!!!");   
                 printMenu();
         }
    }
    
    //menuValor == 1
    public void fillVector()
    {
        int choice;
        
         System.out.printf("1- Preenchimento Automatico"
                            + "\n2- preenchimento manual"
                            + "\nEscolha sua opção: ");
         
         choice = ler.nextInt();
         
         if(choice == 1)
         {
             
         }
         else if (choice == 2)
         {
             
         }
         else
         {
             System.out.printf("ERROR... Oh não!!!" 
             +"\nVocê será redirecionado para o Menu.");
             printMenu();                   
         }    
    }
    
    //menuValor == 2
    public void printVector()
    {
        
    }
    
    //menuValor == 3
    public void editVector()
    {
        
    }
    
    //menuValor == 4
    public void browseVector()
    {
        
    }
    
    //menuValor == 5
    public void orderVector()
    {
        
    }
    
    //menuValor == 6
    public void doMath()
    {
        
    }
    
    //menuValor == 7
    public void doStatistic()
    {
        
    }
    
    //menuValor == 8
    public void elementsValid()
    {
        
    }
    
    
    public static void main(String[] args) 
    {
        //Declaração de variaveis
        int ValorMenu = 0;
        int Menu, vetorSize;
        //determinação do tamanho do vetor
        Scanner ler = new Scanner(System.in);
        System.out.println("Inserir tamanho do vetor: ");
        vetorSize = ler.nextInt();//tem que fazer metodo pra checar se o vetor tem mais de 10000 caracteres

        //declaração dos vetores
        int[] vetor;
        vetor = new int[vetorSize];
        int[] vetor2;
        vetor2 = new int[vetorSize];

        //enquanto o valor não for 9(sair) ele vai repetir o menu
        while (ValorMenu != 9) {
            //Menu de opções
            System.out.printf("======== MENU DE OPÇÕES ======== \n"
                    + "–\n"
                    + "1 - Preencher vetores \n"
                    + "–\n"
                    + "2 - Imprimir vetores \n"
                    + "–\n"
                    + "3 - Eliminar elemento do vetor \n"
                    + "–\n"
                    + "4 - Pesquisar elemento nos vetores \n"
                    + "–\n"
                    + "5 - Ordenar os vetores \n"
                    + "–\n"
                    + "6 - Calcular operações matemáticas \n"
                    + "–\n"
                    + "7 - Calcular métodos estatísticos \n"
                    + "–\n"
                    + "8 - Total de elementos válidos \n"
                    + "-\n"
                    + "9 - Sair"
                    + "\n ==================================="
                    + "\n Escolha sua opção : ");
            ValorMenu = ler.nextInt();
            switch (ValorMenu) {
                case 1:
                    //preenchimento dos vetores
                    System.out.printf("1- Preenchimento Automatico"
                            + "\n2- preenchimento manual"
                            + "\nEscolha sua opção: ");
                    ValorMenu = ler.nextInt();
                    //não precisa fazer o preenchimento automatico, deixa que eu faço depois
                    if (2 == ValorMenu) {
                        //inserir valores dos vetores
                        for (int i = 0; i < vetorSize; i++) {
                            System.out.println("Vetor 1 = Inserir " + (i + 1) + "º vetor");
                            vetor[i] = ler.nextInt();

                        }
                        for (int i = 0; i < vetorSize; i++) {
                            System.out.println("Vetor 2 = Inserir " + (i + 1) + "º vetor");
                            vetor2[i] = ler.nextInt();

                        }
                        //tem que fazer metodo pra checar se o vetor tem menos de 3000 itens

                    }

                case 2:
                    //imprimir vetores
                    System.out.print("Vetor 1 \n [");
                    for (int i = 0; i < vetorSize; i++) {
                        System.out.print(vetor[i] + "-");

                    }
                    System.out.print("]");
                    System.out.print("\n Vetor 2 \n [");
                    for (int i = 0; i < vetorSize; i++) {
                        System.out.print(vetor2[i] + "-");

                    }
                    System.out.print("]\n");
                //ele vai diretamente pro menu depois disso, tem que subir
                //coloca algum sleep seila comando pra pausar, eu to no linux e parece que esse
                //sleep n funciona no meu OS
                case 3:
                    //eliminar elemento dos vetores
                    break;
                case 4:
                    //pesquisar elemento nos vetores
                    break;
                case 5:
                    //ordenar vetores
                    break;
                case 6:
                    //calcular operações matematicas
                    break;
                case 7:
                    //calcular metodos estatisticos
                    break;
                case 8:
                    //total dos elementos validos
                    break;
                default:
                    System.out.println("Valor inválido");
                //colocar um sleep aqui tbm

            }
        }

    }
}
