# desenvolvimento-de-sistemas

# SISTEMA PARA FILMES E CINEMA :
# FALTANDO UMA LIMPA DE TELA, E QUE O PROGRAMA PARE QUANDO ESGOTE
#include <locale.h> 
int main() 
{ 
//permite o programa a ficar em português 
setlocale(LC_ALL, "Portuguese"); 
printf("Utilizando acentuação da língua portuguesa! \n\n"); 
//Variáveis 
int filmes, salas, comidas, bebidas, valor, valor2, pagamento, posicao, ingresso, total, linha, contador, matrizK1[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0} , matrizK2[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0} , matrizK3[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0} , matrizG1[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0}, matrizG2[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0}, matrizG3[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0},matrizP1[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0}, matrizP2[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0}, matrizP3[49]={1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,0}; 
contador=49; 
valor=1; 
    //Mostra as opções de filmes e o usuário escolhe 
    while(valor !=0) { 
    printf("Olá senhor[a]"); 
    printf("\n Bem-vindo ao cinema CINEPOLIS"); 
    printf("\n Nós não temos mais opções de horario, pois já são 10h e o cinema ira fechar após o filme"); 
    printf("\n Os filmes disponiveis estão abaixo"); 
    printf("\n1 ------------Kung fu panda 4------------"); 
    printf("\n2 ------------Garfield fora de casa------------"); 
    printf("\n3 ------------Planeta dos macacos: O reinado------------"); 
    printf("\n digite o número do filme desejado:"); 
    scanf("%d", &filmes); 
      //mostra as opções de sala e o usuário escolhe 
    printf("\n ok qual o tipo da sala do filme?"); 
    printf("\n pressione 1 para legendado - 2 para dublado - 3 para normal:"); 
    scanf("%d", &salas); 
if(matrizK1==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
    if(matrizK2==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizK3==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizG1==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizG2==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizG3==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizP1==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizP2==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){ 
printf("esgotado"); 
valor=0; 
} 
if(matrizP3==0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0){
printf("esgotado"); 
valor=0; 
} 
    //removedor de cadeiras 
    if(filmes ==1 && salas ==1) { 
    printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    printf("\n-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizK1[linha]); 
    printf("\n-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------\n"); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
printf("\n-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizK1[linha]=matrizK1[linha+1]; 
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizK1[linha]); 
printf("\n-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------\n"); 
} 
//removedor de cadeiras2 
    if(filmes ==1 && salas ==2) { 
    printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizK2[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizK2[linha]=matrizK2[linha+1]; 
for(linha=0; linha<contador-1; linha++)
printf("%d  ", matrizK2[linha]); 
} 
//removedor de cadeiras3 
    if(filmes ==1 && salas ==3){ 
printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizK3[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizK3[linha]=matrizK3[linha+1]; 
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizK3[linha]); 
} 
   //removedor de cadeiras4 
    if(filmes ==2 && salas ==1) { 
    printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\nabaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizG1[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizG1[linha]=matrizG1[linha+1];
for(linha=0; linha<contador-1; linha++)
printf("%d  ", matrizG1[linha]); 
} 
//removedor de cadeiras5 
    if(filmes ==2 && salas ==2) { 
    printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizG2[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizG2[linha]=matrizG2[linha+1]; 
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizG2[linha]); 
} 
//removedor de cadeiras6 
    if(filmes ==2 && salas ==3){ 
printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizG3[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizG3[linha]=matrizG3[linha+1];
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizG3[linha]); 
} 
//removedor de cadeiras7 
    if(filmes ==3 && salas ==1) { 
    printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\nabaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizP1[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizP1[linha]=matrizP1[linha+1]; 
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizP1[linha]); 
} 
//removedor de cadeiras8 
    if(filmes ==3 && salas ==2) { 
    printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizP2[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizP2[linha]=matrizP2[linha+1]; 
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizP2[linha]); 
} 
//removedor de cadeiras9 
    if(filmes ==3 && salas ==3){ 
printf("\n nos possuimos cerca de 49 cadeiras"); 
    printf("\n para escolher a cadeira desejada voce deve digitar o numero da posição da cadeira"); 
    printf("\n abaixo estão as cadeiras\n"); 
    for(linha=0; linha<contador; linha++) 
    printf("%d  ", matrizP3[linha]); 
    printf("\n se a cadeira estiver livre aparecera o numero dela, senão aparecera um 0"); 
    printf("\n a 49 por exemplo já foi comprada por isso ela é um 0, todas as cadeiras compradas ficarão do lado da 49"); 
    printf("\n EX: quero a cadeira 2 então digito 2, logo a cadeira 3 passa a ser cadeira 2 e a cadeira 4 a ser a cadeira 3 e assim por diante"); 
    printf("\n digite a cadeira que deseja"); 
scanf("%d", &posicao); 
if (posicao>=contador+1) 
printf("nao eh possivel"); 
else 
printf("\n cadeiras\n"); 
for(linha= posicao -1; linha<contador-1; linha++) 
matrizP3[linha]=matrizP3[linha+1]; 
for(linha=0; linha<contador-1; linha++) 
printf("%d  ", matrizP3[linha]); 
} 
    //Mostra as opções de comida e o usuário escolhe a comida 
    printf("\n veja as comidas do nosso cardápio abaixo "); 
    printf("\n 1 - pipoca PP "); 
    printf("\n 2 - pipoca P "); 
    printf("\n 3 - pipoca M "); 
    printf("\n 4 - pipoca G "); 
    printf("\n 5 - pipoca GG "); 
    printf("\n 6 - Nada "); 
    printf("\n digite o número da comida "); 
    scanf("%d", &comidas); 
  //mostra as opções de bebida e o usuário escolhe a bebida 
    printf("\n veja as bebidas do nosso cardápio abaixo "); 
    printf("\n 1 - Coca-Cola 500ml"); 
    printf("\n 2 - Chá mate leão 500ml"); 
    printf("\n 3 - Água com gás 500ml"); 
    printf("\n 4 - Água sem gás 500ml"); 
    prirtf("\n 5 - Guaraná antártica 500ml"); 
    printf("\n 6 - Nada"); 
    printf("\n digite o número da bebida "); 
    scanf("%d", &bebidas); 
     //mostra as opções de ingresso e o usuário escolhe 
    printf("\n veja as opções de ingresso abaixo "); 
    printf("\n 1 - inteira"); 
    printf("\n 2 - meia"); 
    printf("\n digite o número da ingresso "); 
    scanf("%d", &ingresso); 
    //SWITCH CASE DOS DADOS 
   printf("\n  você escolheu o filme:"); 
    switch(filmes){ 
case 1: 
    printf("\n Kung fu Panda 4"); 
    break; 
case 2:
    printf("\n Garfiel fora de casa"); 
    break; 
case 3: 
    printf("\n Planeta dos macacos: O reinado"); 
    break; 
    } 
      printf("\n a sala "); 
    switch(salas){ 
case 1: 
    printf("\n Legendado"); 
    break; 
case 2: 
    printf("\n Dublado"); 
    break; 
case 3: 
    printf("\n Normal"); 
    break; 
    } 
    printf("\n a comida:"); 
    switch(comidas){ 
case 1:
    printf("\n Pipoca PP"); 
    comidas=20; 
    break; 
case 2: 
    printf("\n Pipoca P"); 
    comidas=26; 
    break; 
case 3: 
    printf("\n Pipoca M"); 
    comidas=30; 
    break; 
case 4: 
    printf("\n Pipoca G"); 
    comidas=37; 
    break; 
case 5: 
    printf("\n Pipoca GG"); 
    comidas=43; 
    break; 
case 6: 
    printf("\n não quis"); 
    comidas=0; 
    break; 
    } 
    printf("\n a bebida:"); 
    switch(bebidas){ 
case 1: 
    printf("\n Coca-Cola"); 
    bebidas=12; 
    break; 
case 2: 
    printf("\n Chá mate"); 
    bebidas=12; 
    break; 
case 3: 
    printf("\n Guaraná Antártica"); 
    bebidas=12; 
    break; 
case 4: 
    printf("\n Água sem gás"); 
    bebidas=5; 
    break; 
case 5 :
    printf("\n Água com gás"); 
    bebidas=7; 
    break; 
case 6: 
    printf("\n não quis");
    bebidas=0; 
    break; 
}
    printf("\n e o tipo de ingresso foi " ); 
switch(ingresso){ 
case 1: 
    printf("\n inteiro"); 
    ingresso=50;
    break; 
case 2: 
    printf("\n meia"); 
    ingresso=25; 
    break; 
    } 
    //IMPRESSÃO DOS DADOS 
    total = ingresso+comidas+bebidas; 
    printf("\n o total foi de R$%d", total); 
    printf("\n os pagamentos disponiveis são"); 
    printf("\n cartão = 1"); 
    printf("\n dinheiro = 2"); 
    printf("\n qual o metodo de pagamento?"); 
    scanf("%d", &pagamento); 
    //parar ou continuar o programa 
    printf("obrigado"); 
    printf("\n fim da compra, se desejar sair digite 0 senão digite 1"); 
    scanf("%d", &valor2); 
    if(valor2 != 1) { 
        valor =0; 
    } 
    } 
return 0; 
} 
