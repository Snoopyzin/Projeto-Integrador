//TABULEIRO 
import java.util.Scanner;
public class lig4 {


    public static void main(String[] args){
		Scanner sc = new Scanner(System.in);
        //SAUDACOES INICIAIS
        System.out.println("           !! *** BEM VINDOS AO LIG 4!! *** ");
        System.out.println(" > Digite o nome do jogador 1");
        String jogador1 = sc.nextLine();//RECEBE O NOME DO JOGADOR 1
        System.out.println(" > Digite o nome do jogador 2");
        System.out.println();//PULAR LINHA
        String jogador2 = sc.nextLine();//RECEBE O NOME DO JOGADOR 2
        /**
         * CRIANDO O TABULEIRO 8X8
         * ESPAÇO VAZIO = " "
         * PARTE INICIAL DO JOGO 
         */
            String[][] tabuleiro = new String[8][8];
            for(int i = 0; i < tabuleiro.length; i++){
            for(int j = 0; j < tabuleiro[i].length; j++){
                tabuleiro[i][j] = " ";
            }
        }
             //IMPRESSAO DO TABULEIRO
            for(int i = 0; i < tabuleiro.length; i++){
            for(int j = 0; j < tabuleiro[i].length; j++){
            System.out.print("## " + tabuleiro[i][j] + " ##");
            }
            System.out.println();
        } //FIM DA IMPRESSAO DO TABULEIRO
         System.out.println(" **************************************** ");
         int jogadas = 0;
            while (jogadas < 7){
            //JOGADOR 1
          System.out.println("        ************************************  ");
          System.out.println("                   ''!''!'!" + jogador1+ "''!''!'!");
          System.out.println("        _________________________________________ ");
          System.out.println(" > Digite a coluna que deseja jogar");
          System.out.println("        *************************************  ");
          System.out.println(" _____________________________________________");
          System.out.println(); // PULAR LINHA
            int coluna = sc.nextInt();
           while(coluna < 0 || coluna > 7){
            System.out.println(" ***************************************************** ");
            System.out.println();//PULAR LINHA
            System.out.println("       ''!''!'! Coluna invalida! Digite novamente ''!''!'!");
            System.out.println(); // PULAR LINHA
            System.out.println(" ________________________________________________________ ");
            System.out.println("                   ''!''!'!" + jogador1+ "''!''!'!");
            System.out.println(" ********************************************************* ");
            System.out.println(); // PULAR LINHA
            System.out.println(" > Digite a coluna que deseja jogar");
            System.out.println();//PULAR LINHA
            System.out.println("         _________________________________________________   ");
            coluna = sc.nextInt();
           } //FIM DO WHILE DE VERIFICACAO DA COLUNA DO JOGADOR 1
            //VERIFICANDO SE A COLUNA ESTA CHEIA
                if(tabuleiro[0][coluna] != " "){
                    System.out.println(" Coluna cheia");
                    System.out.println();
                }
            else
            {
            //DESCENDO A PECA NA COLUNA VERIFICANDO SE A POSICAO ESTA VAZIA
                for(int i = 7; i >= 0; i--){
                    if(tabuleiro[i][coluna] == " "){
                        tabuleiro[i][coluna] = "X";
                        break;
                    }
                }
            }
             //MATRIZ COM A POSICAO DAS PEÇAS DO JOGADOR 1
            for(int i = 0; i < tabuleiro.length; i++){
            for(int j = 0; j < tabuleiro[i].length; j++){
            System.out.print("## " + tabuleiro[i][j] + " ##");
            }
            System.out.println();
        }  
        System.out.println("         **********************************************   ");
          //       -----------------------------JOGADOR 2 -----------------------------      \\         
            System.out.println("> PROXIMO JOGADOR");
            System.out.println("        ____________________________________________   ");
            System.out.println("                   ''!''!'!'" +  jogador2 + "'!''!'!");
            System.out.println("         ********************************************    ");
            System.out.println("> Digite a coluna que deseja jogar");
            System.out.println("         _____________________________________________   ");
            System.out.println(" **********************************************************");
            int coluna2 = sc.nextInt();//VARIAVEL QUE RECEBE A COLUNA DO JOGADOR 2
            while(coluna2 < 0 || coluna2 > 7){ // VERIFICANDO SE A COLUNA É VALIDA 
                System.out.println("         _______________________________________________   ");
                System.out.println(" > Coluna invalida! Digite novamente!");
                System.out.println("         ***********************************************   ");
                System.out.println("                   ''!''!'!'" +  jogador2 + "'!''!'!");
                System.out.println("         ________________________________________________   ");
                System.out.println(" > Digite a coluna que deseja jogar");
                coluna2 = sc.nextInt();
            } // FIM DO WHILE DE VERIFICACAO DA COLUNA DO JOGADOR 2
                //VERIFICAR SE A COLUNA ESTA CHEIA
                if(tabuleiro[0][coluna2] != " "){
                    System.out.println("         **********************************************   ");
                    System.out.println();//PULAR LINHA
                    System.out.println(" > Coluna cheia");
                    System.out.println();//PULAR LINHA
                    System.out.println("         ______________________________________________   ");
                }
                else
                {
                    System.out.println(" __________________________________________________________ ");

                   //DESCENDO ATE A ULTIMA POSICAO VAZIA DA COLUNA
                    for(int i = 7; i >= 0; i--){
                        if(tabuleiro[i][coluna2] == " "){
                            tabuleiro[i][coluna2] = "O";
                            break;
                        }
                    }
    
                //MATRIZ COM A COLUNA ESCOLHIDA PELO JOGADOR 2
                for(int i = 0; i < tabuleiro.length; i++){
                    for(int j = 0; j < tabuleiro[i].length; j++){
                        System.out.print("## " + tabuleiro[i][j] + " ##");
                    }
                    System.out.println();
                }
                System.out.println(" ****************************************************** ");
           //CONDICOES DE VITORIA PARA O JOGADOR 1
           //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA HORIZONTAL
              for(int i = 0; i < tabuleiro.length; i++){
              for(int j = 0; j < tabuleiro[i].length - 4; j++){
                   if(tabuleiro[i][j] == "X" && tabuleiro[i][j + 1] == "X" && tabuleiro[i][j + 2] == "X" && tabuleiro[i][j + 3] == "X"){
                       System.out.println(""+jogador1+ " VENCEU !!");
                       System.out.println(" ");
                       System.out.println(" *********************** ");
                       System.out.println("     JOGADOR  " + jogador1 + " VENCEU!!! ");
                       System.out.println(" *                   * ");
                       System.out.println("     *  \\0/    *       ");
                       System.out.println(" *    *  |   *     *  ");
                       System.out.println("   *    / \\     *       ");
                       System.out.println(" *                   * ");
                       System.out.println(" *********************** ");
                       System.exit(0);
                   }
               }
           }      
           //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA VERTICAL
              for(int i = 0; i < tabuleiro.length - 3; i++){
                for(int j = 0; j < tabuleiro[i].length; j++){
                     if(tabuleiro[i][j] == "X" && tabuleiro[i + 1 ][j] == "X" && tabuleiro[i + 2 ][j] == "X" && tabuleiro[i + 3][j] == "X"){
                          System.out.println(""+jogador1+ " VENCEU !!");
                          
                          System.out.println(" ");
                          System.out.println(" *********************** ");
                          System.out.println("     JOGADOR  " + jogador1 + " VENCEU!!! ");
                          System.out.println(" *                   * ");
                          System.out.println("     *  \\0/    *       ");
                          System.out.println(" *    *  |   *     *  ");
                          System.out.println("   *    / \\     *       ");
                          System.out.println(" *                   * ");
                          System.out.println(" *********************** ");
                          System.exit(0);
                     }
                }
              }
             //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA DIAGONAL DIREITA
                for(int i = 0; i < tabuleiro.length - 3; i++){
                    for(int j = 0; j < tabuleiro[i].length; j++){
                        if(tabuleiro[i][j] == "X" && tabuleiro[i + 1 ][j + 1] == "X" && tabuleiro[i + 2][j + 2 ] == "X" && tabuleiro[i + 3][j + 3 ] == "X"){
                            System.out.println(""+jogador1+ "venceu");
                            System.exit(0);
                            System.out.println(" ");
                            System.out.println(" *********************** ");
                            System.out.println("     JOGADOR  " + jogador1 + " VENCEU!!! ");
                            System.out.println(" *                   * ");
                            System.out.println("     *  \\0/    *       ");
                            System.out.println(" *    *  |   *     *  ");
                            System.out.println("   *    / \\     *       ");
                            System.out.println(" *                   * ");
                            System.out.println(" *********************** ");
                        }
                    }
                }
                //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA DIAGONAL ESQUERDA
                for(int i = 0; i < tabuleiro.length - 3; i++){
                    for(int j = 3; j < tabuleiro[i].length; j++){
                        if(tabuleiro[i][j] == "X" && tabuleiro[i + 1][j - 1] == "X" && tabuleiro[i + 2][j - 2] == "X" && tabuleiro[i + 3][j - 3] == "X"){
                            System.out.println(""+jogador1+ "venceu");
                            System.out.println(" ");
                            System.out.println(" *********************** ");
                            System.out.println("     JOGADOR  " + jogador1 + " VENCEU!!! ");
                            System.out.println(" *                   * ");
                            System.out.println("     *  \\0/    *       ");
                            System.out.println(" *    *  |   *     *  ");
                            System.out.println("   *    / \\     *       ");
                            System.out.println(" *                   * ");
                            System.out.println(" *********************** ");
                            System.exit(0);
                        }
                    }
                }
                 //CONDICOES DE VITORIA PARA O JOGADOR 2
                //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA HORIZONTAL
                for(int i = 0; i < tabuleiro.length; i++){
                    for(int j = 0; j < tabuleiro[i].length - 4; j++){
                        if(tabuleiro[i][j] == "O" && tabuleiro[i][j + 1] == "O" && tabuleiro[i][j + 2] == "O" && tabuleiro[i][j + 3] == "O"){
                            System.out.println(""+jogador2+" VENCEU !!");
                            System.out.println(" ");
                            System.out.println(" *********************** ");
                            System.out.println("     JOGADOR  " + jogador2 + " VENCEU!!! ");
                            System.out.println(" *                   * ");
                            System.out.println("     *  \\0/    *       ");
                            System.out.println(" *    *  |   *     *  ");
                            System.out.println("   *    / \\     *       ");
                            System.out.println(" *                   * ");
                            System.out.println(" *********************** ");
                            System.exit(0);
                        }
                    }
                }
                //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA VERTICAL
                for(int i = 0; i < tabuleiro.length - 3; i++){
                    for(int j = 0; j < tabuleiro[i].length; j++){
                        if(tabuleiro[i][j] == "O" && tabuleiro[i + 1 ][j] == "O" && tabuleiro[i + 2 ][j] == "O" && tabuleiro[i + 3 ][j] == "O"){
                            System.out.println(""+jogador2+" VENCEU !!");
                            System.out.println(" ");
                            System.out.println(" *********************** ");
                            System.out.println("     JOGADOR  " + jogador2 + " VENCEU!!! ");
                            System.out.println(" *                   * ");
                            System.out.println("     *  \\0/    *       ");
                            System.out.println(" *    *  |   *     *  ");
                            System.out.println("   *    / \\     *       ");
                            System.out.println(" *                   * ");
                            System.out.println(" *********************** ");
                            System.exit(0);
                        }
                    }
                }
                //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA DIAGONAL DIREITA
                for(int i = 0; i < tabuleiro.length - 3; i++){
                    for(int j = 0; j < tabuleiro[i].length - 3; j++){
                        if(tabuleiro[i][j] == "O" && tabuleiro[i + 1][j + 1] == "O" && tabuleiro[i + 2][j + 2] == "O" && tabuleiro[i + 3][j + 3] == "O"){
                            System.out.println(""+jogador2+" VENCEU !!");
                            System.out.println(" ");
                            System.out.println(" *********************** ");
                            System.out.println("     JOGADOR  " + jogador2 + " VENCEU!!! ");
                            System.out.println(" *                   * ");
                            System.out.println("     *  \\0/    *       ");
                            System.out.println(" *    *  |   *     *  ");
                            System.out.println("   *    / \\     *       ");
                            System.out.println(" *                   * ");
                            System.out.println(" *********************** ");
                            System.exit(0);
                        }
                    }
                }
                //VERIFICANDO SE TEM 4 PEÇAS IGUAIS NA DIAGONAL ESQUERDA
                for(int i = 0; i < tabuleiro.length - 3; i++){
                    for(int j = 3; j < tabuleiro[i].length; j++){
                        if(tabuleiro[i][j] == "O" && tabuleiro[i + 1][j - 1] == "O" && tabuleiro[i + 2][j - 2] == "O" && tabuleiro[i + 3][j - 3] == "O"){
                            System.out.println(""+jogador2+"venceu");
                            System.out.println(" ");
                            System.out.println(" *********************** ");
                            System.out.println("     JOGADOR  " + jogador2 + " VENCEU!!! ");
                            System.out.println(" *                   * ");
                            System.out.println("     *  \\0/    *       ");
                            System.out.println(" *    *  |   *     *  ");
                            System.out.println("   *    / \\     *       ");
                            System.out.println(" *                   * ");
                            System.out.println(" *********************** ");
                            System.exit(0);
                        }
                    }
                }
               //VERIFICANDO SE O JOGO EMPATOU
                int cont = 0;
                for(int i = 0; i < tabuleiro.length; i++){
                    for(int j = 0; j < tabuleiro[i].length; j++){
                        if(tabuleiro[i][j] != " "){
                            cont++;
                        }
                    }
                }
                 if(cont == 64){
                    System.out.println("JOGO EMPATADO");
                    System.exit(0);
                           }          
        }                   
                        
        
    }
    
 


         
}
}        





            
       
      
    

    

    
