#include <stdio.h>
#include <string.h>

int main() {
    int opc, opc1, opc2;
    
    printf("1 --- Conversao de temperatura\n");
    printf("2 --- Conversao de distancia\n");
    printf("3 --- misterio\n");
    printf("escolha: ");
    scanf("%d", &opc);
    
        switch(opc){
        
            case 1:
                printf("\n1 --- Conversao de celcius para fahrenheit\n");
                printf("2 --- Conversao de fahrenheit para celsius\n");
                printf("3 --- Conversao de celsius para kelvin\n");
                printf("escolha: ");
                scanf("%d", &opc1);
                
                    switch(opc1){
                        case 1:
                            int aux, C;
                                printf("\nqual a temperatura em celcius: ");
                                scanf("%d", &C);
                                
                                aux = ((9 * C / 5) + 32);
                                printf("\nA temperatura em fahrenheit é: %d", aux);
                            break;
                        case 2:
                            int aux1, F;
                                printf("\nqual a temperatura em fahrenheit: ");
                                scanf("%d", &F);
                                
                                aux1 = (5 * (F - 32) / 9 );
                                printf("\nA temperatura em celcius é: %d", aux1);
                            
                            break;
                        case 3:
                            int aux2, Celsius;
                                printf("\nqual a temperatura em celcius: ");
                                scanf("%d", &Celsius);
                                
                                aux2 = (Celsius + 273);
                                printf("\nA temperatura em kelvin é: %d", aux2);
                                
                            break;
                        default:
                            printf("\nescolha uma opçao valida!");
                            
                            break;
                    }
            
                break;
                
            case 2:
                printf("\n1 --- Conversao de Km para Milhas\n");
                printf("2 --- Conversao de Milhas para Km\n");
                printf("escolha: \n");
                scanf("%d", &opc2);
                
                    switch(opc2){
                        
                        case 1:
                            int milha, km;
                                printf("\nquantos km de distancia: ");
                                scanf("%d", &km);
                                    
                                milha = km * 0.62137;
                                printf("\nA distancia em Milhas é: %d", milha);
                        
                            break;
                        
                        case 2:
                            int milha1, km1;
                                printf("\nquantas Milhas de distancia: ");
                                scanf("%d", &milha1);
                                    
                                km1 = milha1 / 0.62137 ;
                                printf("\nA distancia em Km é: %d", km1);
                        
                            break;
                            
                        default:
                            printf("\nescolha uma opçao valida!");
                                
                            break;
                                
                    }
                    
                break; 
                
            case 3:
                char sla[5], sla1[5];
                
                int res;
                    
                    do{
                        printf("\n   quer saber o tanto eu Te Amo? (sim ou sim)\n");
                        printf("   resposta: ");
                        
                        scanf("%s", sla);
                        
                    }while(strcmp(sla, "sim") != 0);
                    
                    
                    do{ 
                        
                        if(strcmp(sla, "sim") == 0){
                            printf("\n   tem certeza que quer saber msm?\n");
                            printf("   resposta: ");
                            
                            scanf("%s", sla1);
                            
                            if(strcmp(sla1, "sim") == 0){
                                printf("\n   Entao quanto é 10 vezes 7 dividido por 2 menos 34\n");
                                printf("   resposta: ");
                                
                                scanf("%d", &res);
                                
                                if(res == 1){
                                    printf("\n\n\n\n\n\n   1 né, foi o dia em que me tornei um homem mais feliz ao ter vc ao meu lado. ");
                                    getchar();
                                    getchar();
                                    
                                    printf("\n   Eu quero que vc saiba que eu Te Amo tanto meu amor, que tem um calculo para te mostrar");
                                    getchar(); 
                            
                                    printf("\n   Meu amor por vc é: \n\n");
                                    getchar();
                                    printf("\n                          ♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥");
                                    printf("                                                      ");
                                    printf("\n                          ♥♥♥    lim x→0+ 1/x    ♥♥♥");
                                    printf("                                                      ");
                                    printf("\n                          ♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥♥");
                                    getchar();
                                    
                                    printf("\n\n   Nao entendeu nada né kkkkk");
                                    getchar();
                                    printf("\n   Mas fica em paz amor, eu explico!");
                                    getchar();
                                    printf("\n   Esse calculo se chama limite e a gente estuda em calculo 1 (materia que estou tendo agr)");
                                    getchar();
                                    printf("\n   Ai pensando eu achei um calculo matematico que resume meu amor por vc ♥");
                                    getchar();
                                    printf("\n   Portanto, nessa limete que te mostrei o limite não resulta em um valor numérico finito, mas indica um comportamento assintótico da função em direção ao infinito positivo.");
                                    getchar();
                                    printf("\n   Resumindo o role, meu amor por vc nao tem limites, ele tende ao infinito e alem!");
                                    getchar();
                                    printf("\n   Te amo meu amor ♥");
                                    
                                    break;
                                }else{
                                    printf("\nvai ter que fazer de novo hihihi");
                                }
                            }else{
                                printf("\ndigita sim ai muie");
                            }
                        }else{
                            printf("\ndigita sim ai muie");
                        }
                        
                    }while(strcmp(sla, "sim") == 0);
                    
                    break;
                
            default:
                printf("\nescolha uma opçao valida!");
                            
                break;
        }

    return 0;
}



