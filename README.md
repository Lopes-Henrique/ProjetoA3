# ProjetoA3
package proja3;
import java.util.Scanner;
import java.util.Random;
public class ProjA3 {

    public static void main(String[] args) {
        //abertura de scanner
        Scanner tc = new Scanner (System.in);
        Random aleatorio = new Random();
        //declaracao de variaveis
        int escolha, ponto = 0, i, contador;
        String R;
        //saida e entrada de dados
        
        System.out.println("Digite o seu nome:\n");
        String nome = tc.next();
        
        System.out.println("\nOla, " + nome + " qual quizz voce deseja jogar? 1 - Mat,"
                + " 2 - Geografia, 3 - Conhecimentos gerais, 4 - Esportes, 5 - Todo juntos");
        escolha= tc.nextInt(); 
        
        //abertura de switch case para escolha de quizz
         switch(escolha){
             case(1) -> { 
                 System.out.println("Voce escolheu o quizz de mat! \n");
                 System.out.println("Voce ganhara 1 ponto para acerto e -1 para erro");
              
                    for(contador = 0; contador < 7; contador++){ 
                    i = aleatorio.nextInt(7);
                    
                     switch (i) {
                         case (0): System.out.println("Qual a raiz quadrada de 9?\n");
                             System.out.println("============");
                             System.out.println("A - 5");
                             System.out.println("B - 6");
                             System.out.println("C - 3");
                             System.out.println("D - 2");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;  
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto ++;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\n\nResposta errada");
                                 ponto--;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }
                             break;
                             
                         case (1): System.out.println("\nQuanto e 12^2\n");
                             System.out.println("============");
                             System.out.println("A - 240");
                             System.out.println("B - 144");
                             System.out.println("C - 320");
                             System.out.println("D - 102");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto ++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (2): System.out.println("\nQuanto e 10% de 1500\n");
                             System.out.println("============");
                             System.out.println("A - 150");
                             System.out.println("B - 50");
                             System.out.println("C - 1500");
                             System.out.println("D - 500");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta certa");
                                  ponto++;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\n\nResposta errada");
                                 ponto--;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                          case (3): System.out.println("Quanto é 8 ao cubo?\n");
                             System.out.println("============");
                             System.out.println("A - 512");
                             System.out.println("B - 600");
                             System.out.println("C - 358");
                             System.out.println("D - 64");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta correta");
                                 ponto++;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\n\nResposta errada");
                                 ponto--;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }
                             break;
                             
                         case (4): System.out.println("Qual a raiz de 121?\n");
                             System.out.println("============");
                             System.out.println("A - 5");
                             System.out.println("B - 21");
                             System.out.println("C - 7");
                             System.out.println("D - 11");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                  ponto ++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }
                             break; 
                         case (5): System.out.println("Qual a raiz de 81?\n");
                             System.out.println("============");
                             System.out.println("A - 5");
                             System.out.println("B - 6");
                             System.out.println("C - 7");
                             System.out.println("D - 9");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                  ponto ++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }
                             break; 
                         case (6): System.out.println("Resolva: 2*(15+15)?\n");
                             System.out.println("============");
                             System.out.println("A - 60");
                             System.out.println("B - 30");
                             System.out.println("C - 90");
                             System.out.println("D - 50");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta certa");
                                    ponto ++;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }
                             break; 
                        }     
                     }//switch        
            }
              case(2) -> {
                  System.out.println("Voce escolheu o quizz de geo\n"); 
                  System.out.println("Voce ganhara 1 ponto para acerto e -1 para erro");
                  for( i = 0; i < 3; i++){
                      switch (i) {
                         case (0): System.out.println("Qual a capital do Chile\n");
                             System.out.println("============");
                             System.out.println("A - Caracas");
                             System.out.println("B - Santiago");
                             System.out.println("C - Foz do iguaçu");
                             System.out.println("D - Machu Picho");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (1): System.out.println("\nQual continente fica a Australia\n");
                             System.out.println("============");
                             System.out.println("A - Europa");
                             System.out.println("B - America do Norte");
                             System.out.println("C - Asia");
                             System.out.println("D - Oceania");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (2): System.out.println("\nEm qual America a Jamaica se localiza\n");
                             System.out.println("============");
                             System.out.println("A - America do Sul");
                             System.out.println("B - America do Norte");
                             System.out.println("C - Africa");
                             System.out.println("D - America Central");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                           case (3): System.out.println("Qual a capital do Chile\n");
                             System.out.println("============");
                             System.out.println("A - Caracas");
                             System.out.println("B - Santiago");
                             System.out.println("C - Foz do iguaçu");
                             System.out.println("D - Machu Picho");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                        
                             case (4): System.out.println("Qual a capital do Chile\n");
                             System.out.println("============");
                             System.out.println("A - Caracas");
                             System.out.println("B - Santiago");
                             System.out.println("C - Foz do iguaçu");
                             System.out.println("D - Machu Picho");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                        case (5): System.out.println("Qual a capital do Chile\n");
                             System.out.println("============");
                             System.out.println("A - Caracas");
                             System.out.println("B - Santiago");
                             System.out.println("C - Foz do iguaçu");
                             System.out.println("D - Machu Picho");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                        case (6): System.out.println("Qual a capital do Chile\n");
                             System.out.println("============");
                             System.out.println("A - Caracas");
                             System.out.println("B - Santiago");
                             System.out.println("C - Foz do iguaçu");
                             System.out.println("D - Machu Picho");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                                 ponto--; 
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                     }        
                 }
               }
            
               case(3) -> {
                   System.out.println("Voce escolheu o quizz de Conhecimentos gerais\n");
                   System.out.println("Voce ganhara 1 ponto para acerto e -1 para erro");
                   for( i = 0; i < 3; i++){
                    switch (i) {
                         case (0): System.out.println("Qual é a moeda da Inglaterra\n");
                             System.out.println("============");
                             System.out.println("A - Libra Esterlina");
                             System.out.println("B - Dollar Europeu");
                             System.out.println("C - Dollar");
                             System.out.println("D - Euro");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++; 
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (1): System.out.println("\nQual pintou cortou sua propria orelha\n");
                             System.out.println("============");
                             System.out.println("A - Pablo Picasso");
                             System.out.println("B - Leonardo da Vinci");
                             System.out.println("C - Claudio Monet");
                             System.out.println("D - Vincent Van Gogh");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (2): System.out.println("\nQual filme ganhou o oscar de melhor filme deste ano?\n");
                             System.out.println("============");
                             System.out.println("A - Gato de botas 2");
                             System.out.println("B - A Fera do Mar");
                             System.out.println("C - Pinoquio por Guillermo del Toro");
                             System.out.println("D - Tudo em todo lugar ao mesmo tempo");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                     }        
                
                }
            }
                  case(4) -> {
                      System.out.println("Voce escolheu o quizz de esportes\n");
                      System.out.println("Voce ganhara 1 ponto para acerto e -1 para erro");
                for ( i = 0; i < 3; i++) {
                    switch (i) {
                         case (0): System.out.println("Quem ganhou a copa de 2018?\n");
                             System.out.println("============");
                             System.out.println("A - Croacia");
                             System.out.println("B - Franca");
                             System.out.println("C - Inglaterra");
                             System.out.println("D - Brasil");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada"); 
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (1): System.out.println("\nQuem e intitulado o Rei do Futsal\n");
                             System.out.println("============");
                             System.out.println("A - Falcao");
                             System.out.println("B - Cristiano Ronaldo");
                             System.out.println("C - Lionel Messi");
                             System.out.println("D - Pele");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (2): System.out.println("\n Qual o jogador mais alto que já participou da NBA\n");
                             System.out.println("============");
                             System.out.println("A - Ish Smith");
                             System.out.println("B - Koby Briant");
                             System.out.println("C - Shack O'neil");
                             System.out.println("D - Tack Fall");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                     }      
                }
               
            }
                case(5) -> { 
                 System.out.println("Voce escolheu o quizz de tudo junto! \n");
                 System.out.println("Voce ganhara 1 ponto para acerto e -1 para erro");
                 
                 for( i = 0; i < 12; i++){
                     switch (i) {
                         case (0): System.out.println("Qual a raiz quadrada de 9?\n");
                             System.out.println("============");
                             System.out.println("A - 5");
                             System.out.println("B - 6");
                             System.out.println("C - 3");
                             System.out.println("D - 2");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto ++;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\n\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }
                             break;
                             
                         case (1): System.out.println("\nQuanto e 12^2?\n");
                             System.out.println("============");
                             System.out.println("A - 144");
                             System.out.println("B - 102");
                             System.out.println("C - 320");
                             System.out.println("D - 200");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (2): System.out.println("\nQuanto e 10% de 1500?\n");
                             System.out.println("============");
                             System.out.println("A - 500");
                             System.out.println("B - 50");
                             System.out.println("C - 150");
                             System.out.println("D - 1500");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\n\nResposta certa");
                                 ponto++;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                        case (3): System.out.println("Qual a capital do Chile?\n");
                             System.out.println("============");
                             System.out.println("A - Caracas");
                             System.out.println("B - Foz do Iguacu");
                             System.out.println("C - Santiago");
                             System.out.println("D - Machu Picho");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (4): System.out.println("\nQual continente fica a Australia?\n");
                             System.out.println("============");
                             System.out.println("A - Europa");
                             System.out.println("B - America do Norte");
                             System.out.println("C - Asia");
                             System.out.println("D - Oceania");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (5): System.out.println("\nEm qual America a Jamaica se localiza?\n");
                             System.out.println("============");
                             System.out.println("A - America do Sul");
                             System.out.println("B - America do Norte");
                             System.out.println("C - Africa");
                             System.out.println("D - America Central");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (6): System.out.println("Qual é a moeda da Inglaterra?\n");
                             System.out.println("============");
                             System.out.println("A - Dollar");
                             System.out.println("B - Dollar Europeu");
                             System.out.println("C - Libra Esterlina");
                             System.out.println("D - Euro");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (7): System.out.println("\nQual pintou cortou sua propria orelha?\n");
                             System.out.println("============");
                             System.out.println("A - Pablo Picasso");
                             System.out.println("B - Leonardo da Vinci");
                             System.out.println("C - Claudio Monet");
                             System.out.println("D - Vincent Van Gogh");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (8): System.out.println("\nQual filme ganhou o oscar de melhor filme deste ano?\n");
                             System.out.println("============");
                             System.out.println("A - Gato de botas 2");
                             System.out.println("B - A Fera do Mar");
                             System.out.println("C - Pinoquio por Guillermo del Toro");
                             System.out.println("D - Tudo em todo lugar ao mesmo tempo");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (9): System.out.println("Quem ganhou a copa de 2018?\n");
                             System.out.println("============");
                             System.out.println("A - Croacia");
                             System.out.println("B - Iglaterra");
                             System.out.println("C - Franca");
                             System.out.println("D - Brasil");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                             
                         case (10): System.out.println("\nQuem e intitulado o Rei do Futsal?\n");
                             System.out.println("============");
                             System.out.println("A - Pele");
                             System.out.println("B - Cristiano Ronaldo");
                             System.out.println("C - Lionel Messi");
                             System.out.println("D - Falcao");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                             R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;
                         case (11): System.out.println("\n Qual o jogador mais alto que ja participou da NBA?\n");
                             System.out.println("============");
                             System.out.println("A - Ish Smith");
                             System.out.println("B - Koby Briant");
                             System.out.println("C - Shack O'neil");
                             System.out.println("D - Tack Fall");
                             System.out.println("Pular");
                             System.out.println("============");
                             
                            R = tc.next();
                             
                             if("A".equals(R) || "a".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("B".equals(R) || "b".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("C".equals(R) || "c".equals(R)){
                                 System.out.println("\nResposta errada");
                             }else if("D".equals(R) || "d".equals(R)){
                                 System.out.println("\nResposta certa");
                                 ponto++;
                             }else if("Pular".equals(R) || "pular".equals(R) || "PULAR".equals(R)){
                                 System.out.println("Voce pulou a pergunta");
                             }else{
                                 System.out.println("Resposta invalida");
                             }break;    
                     }//switch5        
                 }
            }//case 5   
                 
                  default -> {
                      System.out.println("Opcao invalida");
                  }
                  
                
         }//switch
        System.out.println("Parabens, voce fez: " + ponto + " pontos");             
 }//main
           
}//public class
    

//Aumentar numero de questoes 
//Terminar trabalho
//Pontuação diferente 
//Se possivel, deixar aleatorio
