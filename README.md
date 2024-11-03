# DESENVOLVIMENTO DE SISTEMAS

# EXERCICIO 32
void setup() {
  // put your setup code here, to run once:
pinMode (8, OUTPUT);
pinMode (12, OUTPUT);
pinMode (11, OUTPUT);
pinMode (10, OUTPUT);
pinMode (9, OUTPUT);
}


void loop() {
  // put your main code here, to run repeatedly:
digitalWrite (8, HIGH);
digitalWrite (12, HIGH);
delay (20000);
digitalWrite (8, LOW);
digitalWrite (12, LOW);
digitalWrite (9, HIGH);
digitalWrite (10, HIGH);
delay (15000);
digitalWrite (10, LOW);
digitalWrite (9, HIGH);
digitalWrite (11, HIGH);
delay (3000);
digitalWrite (11, LOW);
digitalWrite (9, LOW);
}

# EXERCICIO 33
void setup() {
  // put your setup code here, to run once:
pinMode (8, OUTPUT); // VERDE PEDESTRE
pinMode (12, OUTPUT); // VERMELHA CARRO
pinMode (11, OUTPUT); // AMARELA
pinMode (10, OUTPUT); // VERDE CARRO
pinMode (9, OUTPUT); // VERMELHA PEDESTRE
}


void loop() {
  manhafunc();
  tardefunc();
  madrufunc();
}
// CONTADOR MANHÃ
void manhafunc(){
  int contador, manha, tarde, madru;
  contador=0;
  manha=0;
do{ manha++;
digitalWrite (8, HIGH);
digitalWrite (12, HIGH);
delay (20000);
do{
  contador++;
digitalWrite (8, LOW);
digitalWrite (9, HIGH);
delay (500);
// PISCA LUZ VERMELHA PEDESTRE
digitalWrite (9, LOW);
delay (500);
digitalWrite (9, HIGH);
delay (500);
}while(contador<4);
contador=0;
// FIM PISCA
// LIGA VERDE CARRO E LIGA VERMEHO PEDESTRE
digitalWrite (12, LOW);
digitalWrite (9, HIGH);
digitalWrite (10, HIGH);
delay (15000);
digitalWrite (10, LOW);
digitalWrite (9, HIGH);
digitalWrite (11, HIGH);
delay (3000);
digitalWrite (11, LOW);
digitalWrite (9, LOW);
  }while(manha<2);
}
// CONTADOR TARDE
void tardefunc(){
  int contador, manha, tarde, madru;
  contador=0;
  tarde=0;
 do{ tarde++;
digitalWrite (8, HIGH);
digitalWrite (12, HIGH);
delay (8000);
do{
  contador++;
digitalWrite (8, LOW);
digitalWrite (9, HIGH);
delay (300);
// PISCA LUZ VERMELHA PEDESTRE
digitalWrite (9, LOW);
delay (300);
digitalWrite (9, HIGH);
delay (300);
}while(contador<4);
contador=0;
// FIM PISCA
// LIGA VERDE CARRO E LIGA VERMEHO PEDESTRE
digitalWrite (12, LOW);
digitalWrite (9, HIGH);
digitalWrite (10, HIGH);
delay (8000);
digitalWrite (10, LOW);
digitalWrite (9, HIGH);
digitalWrite (11, HIGH);
delay (2000);
digitalWrite (11, LOW);
digitalWrite (9, LOW);
  }while(tarde<2);
}
// CONTADOR MADRUGADA
void madrufunc(){
  int contador, manha, tarde, madru;
  contador=0;
  madru=0;
do{ madru++;
  digitalWrite (11, HIGH);
  digitalWrite (9, HIGH);
  delay (2000);
  digitalWrite (11, LOW);
  digitalWrite (9, LOW);
  delay (1000);
  }while(madru<10);
}

# EXERCICIO 34
int counter;

void setup()
{
  pinMode(5, OUTPUT);
  pinMode(6, OUTPUT);
  pinMode(7, OUTPUT);
  pinMode(8, OUTPUT);
  pinMode(9, OUTPUT);
}

void loop()
{
  
   digitalWrite(8, HIGH);
   digitalWrite(6, LOW);
   digitalWrite(7, HIGH);
   
 
    delay(5000); // Wait for 1000 millisecond(s)
    digitalWrite(6, HIGH);
    digitalWrite(7, LOW);
    delay(5000); // Wait for 100 millisecond(s)
    digitalWrite(5, HIGH);
    digitalWrite(9, HIGH);
    digitalWrite(8, LOW);
    digitalWrite(6, LOW);
  	 delay(5000); // Wait for 100 millisecond(s)
    digitalWrite(5, LOW);
    digitalWrite(9, LOW);
    digitalWrite(8, LOW);
}

# EXERCICIO 35
void setup() {
  // put your setup code here, to run once:
pinMode (8, OUTPUT); // VERDE PEDESTRE
pinMode (12, OUTPUT); // VERMELHA CARRO
pinMode (11, OUTPUT); // AMARELA
pinMode (10, OUTPUT); // VERDE CARRO
pinMode (9, OUTPUT); // VERMELHA PEDESTRE
}


void loop() {
  manhafunc();
  tardefunc();
  madrufunc();
}
// CONTADOR MANHÃ
void manhafunc(){
  int contador, manha;
  contador=0;
  manha=0;
do{ manha++;
digitalWrite (8, HIGH);
digitalWrite (12, HIGH);
delay (25000);
do{
  contador++;
digitalWrite (8, LOW);
digitalWrite (9, HIGH);
delay (500);
// PISCA LUZ VERMELHA PEDESTRE
digitalWrite (9, LOW);
delay (500);
}while(contador<5);
contador=0;
// FIM PISCA
// LIGA VERDE CARRO E LIGA VERMEHO PEDESTRE
digitalWrite (12, LOW);
digitalWrite (9, HIGH);
digitalWrite (10, HIGH);
delay (40000);
digitalWrite (10, LOW);
digitalWrite (9, HIGH);
digitalWrite (11, HIGH);
delay (5000);
digitalWrite (11, LOW);
digitalWrite (9, LOW);
  }while(manha<6);
}
// CONTADOR TARDE
void tardefunc(){
  int contador, tarde;
  contador=0;
  tarde=0;
 do{ tarde++;
digitalWrite (8, HIGH);
digitalWrite (12, HIGH);
delay (45000);
do{
  contador++;
digitalWrite (8, LOW);
digitalWrite (9, HIGH);
delay (500);
// PISCA LUZ VERMELHA PEDESTRE
digitalWrite (9, LOW);
delay (500);
}while(contador<5);
contador=0;
// FIM PISCA
// LIGA VERDE CARRO E LIGA VERMEHO PEDESTRE
digitalWrite (12, LOW);
digitalWrite (9, HIGH);
digitalWrite (10, HIGH);
delay (60000);
digitalWrite (10, LOW);
digitalWrite (9, HIGH);
digitalWrite (11, HIGH);
delay (10000);
digitalWrite (11, LOW);
digitalWrite (9, LOW);
  }while(tarde<6);
}
// CONTADOR MADRUGADA
void madrufunc(){
  int contador, madru;
  contador=0;
  madru=0;
do{ madru++;
  digitalWrite (11, HIGH);
  digitalWrite (9, HIGH);
  delay (2000);
  digitalWrite (11, LOW);
  digitalWrite (9, LOW);
  delay (1000);
  }while(madru<6);
}


# EXERCICIO 38

# A) Desenvolver um programa que faça a contagem de 0 até 100 e imprima na tela,
na horizontal.
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int valor, peso, contadorpeso, contador4, contador, contadorpeso2;
    float altura , contador5, somadaaltura;
for(contador=0;contador<=100;contador++)
printf("%d ",contador);
return (0);
}
# B) 
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=10;contador<=50;contador++)
printf("%d ",contador);
return (0);
}
# C) 
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=10;contador<=100;contador++)
printf("%d \n",contador);
return (0);
}
# D) 
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=20;contador<=40;contador++)
if(contador %2 ==0)
printf("%d ",contador);
return (0);
}
# E)
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=10;contador<=60;contador++)
if(contador %2 !=0)
printf("%d \n",contador);
return (0);
}
# F)
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=39;contador<=100;contador++)
if(contador %3 ==0)
printf("%d ",contador);
return (0);
}
# G)
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=0;contador<=100;contador++)
if(contador %5 ==0)
printf("%d ",contador);
return (0);
}
# H)
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=100;contador>=0;contador--)
printf("%d ",contador);
return (0);
}
# I)
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int contador;
for(contador=50;contador>=0;contador--)
if(contador%2 ==0)
printf("%d ",contador);
return (0);
}
# J)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int contador, contadorsoma, contador2;
contadorsoma =0;
contador2=0;
for(contador=1;contador<=200;contador++)
if (contador%2 !=0 && contador%3 ==0)
contador2++;
printf("%f ", 105.0909090909*contador2);
}
# K)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int contador;
for(contador=1;contador<=100;contador++)
if(contador%2 !=0)
printf("%d ",contador);
for(contador=100;contador>=1;contador--)
if(contador%2 !=0)
printf("%d ",contador);
return (0);
}
# L)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int contador;
for(contador=10;contador<=50;contador++)
if(contador%2 ==0)
printf("%d par",contador);
else
    printf("%d impar", contador);
}
# M)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int contador, contadorsoma;
contadorsoma =0;
for(contador=1;contador<=50;contador++)
contadorsoma+=contador;
printf("%d", contadorsoma);
}

# EXERCICIO 39
# A)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int valor;
printf("\nescolha o lanche do cardapio abaixo");
printf("\nOpcao1 - Big Mac:14,50");
printf("\nOpcao2 - Quarterao com Queijo:15,50");
printf("\nOpcao3 - Hamburguer:10,90");
printf("\nOpcao4 - Cheeseburger:9,90");
printf("\nOpcao5 - McFritas Pequena:6,70");
printf("\nOpcao6 - Chicken McNuggets:7,80");
printf("\nqual a opcao desejada? para escolher simplesmente digite o numero da opcao");
scanf("%d", &valor);

switch ( valor )
{
case 1:
printf("Opcao 1 - Big Mac: 14,50");
break;
case 2:
printf("Opcao 2 - Quarterao com Queijo: 15,50");
break;
case 3:
printf("Opcao 3 - Hamburguer: 10,90");
break;
case 4:
printf("Opcao4 - Cheeseburger:9,90");
break;
case 5:
printf("Opcao 5 - McFritas Pequena: 6,70");
break;
case 6:
printf("Opcao 6 - Chicken McNuggets: 7,80");
break;
default:
    printf("essa opcao nao existe");
}

}
# B)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int valor;
printf("se voce deseja votar veja a tabela de idades abaixo");
printf("\n0 a 15 digite 1");
printf("\n16 a 18 digite 2");
printf("\n19 a 65 digite 3");
printf("\n66 a 99 digite 4");
printf("\ndigite o seu valor para descobrir");
scanf("%d", &valor);
switch ( valor )
{
case 1:
printf("nao eh possivel votar");
break;
case 2:
printf("voto facultativo");
break;
case 3:
printf("voto obrigatorio");
break;
case 4:
printf("voto nao obrigatorio");
break;
default:
    printf("essa opcao nao existe");
}

}
# C)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int valor;
printf("qual sobremesa deseja?");
printf("\n para Mousse digite 1");
printf("\n para Sorvete digite 2");
printf("\n para MilkShake digite 3");
printf("\n para Sunday digite 4");
scanf("%d", &valor);
switch ( valor )
{
case 1:
printf("Mousse");
break;
case 2:
printf("Sorvete");
break;
case 3:
printf("MilkShake");
break;
case 4:
printf("Sunday");
break;
default:
    printf("Essa opcao nao existe");
}

}
# D)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int valor, salario, s, z;
printf("digite o valor do seu salario");
scanf("%d", &salario);
printf("agora olhe as opcoes abaixo e digite o valor para saber o valor do seu auxilio mensal");
printf("\n casada e sem filhos digite 1");
printf("\n casada ou nao e com filhos digite 2");
printf("\n solteira e sem filhos digite 3");
scanf("%d", &valor);
s=salario*0.15;
z=salario*0.35;
switch ( valor )
{
case 1:
printf("%d", s+salario);
break;
case 2:
printf("%d", z+salario);
break;
case 3:
printf("Nao possui auxilio mensal");
break;
default:
    printf("Essa opcao nao existe");
}

}
# E)
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()
{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int padaria, bebidas, congelados, acougue, verduras, contador, filmes, padaria2, bebidas2, congelados2, acougue2, verduras2;


printf("\nbem vindo ao supermercado condor");
printf("\ntemos 5 setores de compra abaixo");
printf("\n 1 Padaria");
printf("\n 2 Bebida");
printf("\n 3 Congelados");
printf("\n 4 Açougue");
printf("\n 5 Verdura");
printf("qual o setor desejado?");
scanf("%d", &filmes);


switch(filmes)
{
case 1:
printf("\n no setor da padaria possuimos 5 itens");
printf("\n 1 Pão francês R$1,25");
printf("\n 2 Pão de queijo R$2,00");
printf("\n 3 Chipa   R$2,50");
printf("\n 4 Empada de frango 8 unidades R$14,99");
printf("\n 5 Doguinho 8 unidades R$14,99");
printf("\noque deseja comprar ?");
scanf("%d", &padaria);
printf("\nquantas unidades?");
scanf("%d", &padaria2);
if (padaria==1)
    printf("%f R$", 1.25*padaria2);
if (padaria==2)
    printf("%d R$", 2*padaria2);
if (padaria==3)
    printf("%f R$", 2.5*padaria2);
if (padaria==4)
    printf("%d R$", 15*padaria2);
if (padaria==5)
    printf("%d R$", 15*padaria2);
break;


case 2:
printf("\n no setor das bebidas possuimos 5 itens");
printf("\n 1 Coca-Cola 1,5L R$7,50 R$");
printf("\n 2 Chá mate 1,5L R$8,00 R$");
printf("\n 3 Água-sem-gas 500ml R$3,00 R$");
printf("\n 4 Pepsi 250ml R$3,00 R$");
printf("\n 5 Suco de laranja 1L R$9,00 R$");
printf("oque deseja comprar?");
scanf("%d", &bebidas);
printf("\nquantas unidades?");
scanf("%d", &bebidas2);
if (bebidas==1)
    printf("%f R$", 7.5*bebidas2);
if (bebidas==2)
    printf("%d R$", 8*bebidas2);
if (bebidas==3)
    printf("%d R$", 3*bebidas2);
if (bebidas==4)
    printf("%d R$", 3*bebidas2);
if (bebidas==5)
    printf("%d R$", 9*bebidas2);
break;


case 3:
printf("\n no setor dos congelados possuimos 5 itens");
printf("\n 1 Batata frita 2kg R$25,00");
printf("\n 2 Frango inteiro 1kg R$12,00");
printf("\n 3 Hamburguer 500g R$20,99");
printf("\n 4 Pizza de frango e catupiri 500g R$17,00");
printf("\n 5 Postas de tilapia 1kg R$30,99");
printf("oque deseja comprar?");
scanf("%d", &congelados);
printf("\nquantas unidades?");
scanf("%d", &congelados2);
if (congelados==1)
    printf("%f R$", 25*congelados2);
if (congelados==2)
    printf("%d R$", 12*congelados2);
if (congelados==3)
    printf("%d R$", 21*congelados2);
if (congelados==4)
    printf("%d R$", 17*congelados2);
if (congelados==5)
    printf("%d R$", 31*congelados2);
break;


case 4:
printf("\n no setor do açougue possuimos 5 itens");
printf("\n 1 Picanha 1kg R$110,00");
printf("\n 2 Linguiça 500g R$25,00");
printf("\n 3 File mignon 500g R$30,00");
printf("\n 4 Coração de galinha 1kg R$30,00");
printf("\n 5 Peito de frango 1kg R$18,00");
printf("oque deseja comprar?");
scanf("%d", &acougue);
printf("\nquantas unidades?");
scanf("%d", &acougue2);
if (acougue==1)
    printf("%f R$", 110*acougue2);
if (acougue==2)
    printf("%d R$", 25*acougue2);
if (acougue==3)
    printf("%d R$", 30*acougue2);
if (acougue==4)
    printf("%d R$", 30*acougue2);
if (acougue==5)
    printf("%d R$", 18*acougue2);
break;


case 5:
printf("\n no setor das verduras possuimos 5 itens");
printf("\n 1 Alface 200g R$15,00");
printf("\n 2 Abóbora cabotia 2,25kg R$15,99");
printf("\n 3 Repolho verde 500g R$9,00");
printf("\n 4 Couve 200g R$9,00");
printf("\n 5 Rucula 200g R$10,00");
printf("oque deseja comprar e quantas unidades?");
scanf("%d", &verduras);
printf("\nquantas unidades?");
scanf("%d", &verduras2);
if (verduras==1)
    printf("%f R$", 15*verduras2);
if (verduras==2)
    printf("%d R$", 16*verduras2);
if (verduras==3)
    printf("%d R$", 9*verduras2);
if (verduras==4)
    printf("%d R$", 9*verduras2);
if (verduras==5)
    printf("%d R$", 10*verduras2);
break;
}
}
# F)
#include<stdlib.h>
#include<stdio.h>
int main()
{
int valor, salario, s, z, t;
printf("digite o valor do seu salario");
scanf("%d", &salario);
printf("agora digite o seu cargo para ver qual o aumento do salario");
printf("\n supervisor digite 1");
printf("\n tecnico digite 2");
printf("\n outros cargos digite 3");
scanf("%d", &valor);
s=salario*0.3;
z=salario*0.2;
t=salario*0.1;
switch ( valor )
{
case 1:
printf("supervisor %d", s+salario);
break;
case 2:
printf("tecnico %d", z+salario);
break;
case 3:
printf("outros cargos %d", t+salario);
break;
default:
    printf("Essa opcao nao existe");
}

}
# G)
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes;

printf("\nbem vindo ao restaurante xy");
printf("\naqui nos temos 5 pratos diferentes");
printf("\n 1 - Bacalhau");
printf("\n 2 - Risoto");
printf("\n 3 - Peixe");
printf("\n 4 - Feijoada");
printf("\n 5 - Carne Assada");
printf("digite o número do prato desejado");
scanf("%d", &filmes);

switch(filmes)
{

case 1:
printf("a escolha é o bacalhau");
break;

case 2:
printf("a escolha é o Risoto");
break;

case 3:
printf("a escolha é o Peixe");
break;

case 4:
printf("a escolha é a Feijoada");
break;

case 5:
printf("a escolha é a Carne Assada");
break;
}
}

# H)
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes;

printf("a sua compra deu um total de 500,00 reais");
printf("opções de pagamento");
printf(" 1 cartão debito");
printf(" 2 cartão credito");
printf(" 3 dinheiro");
printf(" 4 vale refeição");
printf(" 5 vale alimentação");
printf("qual o pagamento desejado?");
scanf("%d", &filmes);

switch(filmes)
{
case 1:
printf("\n 10 por cento de acrescimo");
printf("\n R$505,00");
break;

case 2:
printf("\n 10 por cento de acrecsimo");
printf("\n R$505,00");
break;

case 3:
printf("\n 10 por cento de decrecsimo");
printf("\n R$495,00");
break;

case 4:
printf("\n anula o valor total");
printf("\n R$00,00");
break;

case 5:
printf("\n sem mudanças");
printf("\n R$500,00");
break;
}
}
# I)
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes;

printf("\nbem vindo ao lanches xy");
printf("\n 1 - Big Mac - R$ 26,90 e Suco de Laranja – R$ 12,30 ");
printf("\n 2 - Cheddar McMelt - R$ 26,50 e Coca Cola – R$ 7,90");
printf("\n 3 - Duplo Big Mac - R$ 28,90 e Suco de Laranja – R$ 12,30");
printf("\n 4 - Quarterão com queijo - R$ 26,50 e Coca Cola – R$ 7,90");
printf("\n 5 - McNífico Bacon - R$ 29,90 e Suco de Laranja – R$ 12,30");
printf("\n 6 - McChicken - R$ 25,90 e Coca Cola – R$ 7,90");
printf("\n 7 - Chicken Supreme Crispy - R$ 29,90 e Suco de Laranja – R$ 12,30");
printf("\n 8 - 10 Chicken McNuggets - R$ 22,50 e Coca Cola – R$ 7,90");
printf("\n 9 - Big Tasty Turbo Queijo - R$ 33,90 e Suco de Laranja – R$ 12,30");
printf("\n 10 - Big Tasty - R$ 31,90 e Coca Cola – R$ 7,90");
printf("\n 11 - Picanha Club House (1 carne) - R$ 34,90 e Suco de Laranja – R$ 12,30");
printf("\ndigite o número do prato desejado");
scanf("%d", &filmes);

switch(filmes)
{

case 1:
printf("\na escolha é Big Mac e Suco de Laranja");
printf("\ntotal: R$39,20");
break;

case 2:
printf("\na escolha é Cheddar McMelt e Coca Cola");
printf("\ntotal: R$34,40");
break;

case 3:
printf("\na escolha é Duplo Big Mac e Suco de Laranja");
printf("\ntotal: R$41,20");
break;

case 4:
printf("\na escolha é Quarterão com queijo e Coca Cola");
printf("\ntotal: R$34,40");
break;

case 5:
printf("\na escolha é McNífico Bacon e Suco de Laranja");
printf("\ntotal: R$42,20");
break;

case 6:
printf("\na escolha é McChicken e Coca Cola");
printf("\ntotal: R$33,80");
break;

case 7:
printf("\na escolha é Chicken Supreme Crispy e Suco de Laranja");
printf("\ntotal: R$42,20");
break;

case 8:
printf("\na escolha é 10 Chicken McNuggets e Coca Cola");
printf("\ntotal: R$30,40");
break;

case 9:
printf("\na escolha é Big Tasty Turbo Queijo e Suco de Laranja");
printf("\ntotal: R$46,20");
break;

case 10:
printf("\na escolha é  Big Tasty e Coca Cola");
printf("\ntotal: R$39,80");
break;

case 11:
printf("\na escolha é  Picanha Club House e Suco de Laranja");
printf("\ntotal: R$47,20");
break;
}
}
# J)
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes, filmes2, filmes3;
do{
filmes3 =1;
printf("no nosso livro possuimos 3 bolos");
printf("\n 1 bolo de fubá");
printf("\n 2 bolo de laranja");
printf("\n 3 bolo de cenoura");
printf("\nqual a receita de bolo desejada?");
scanf("%d", &filmes);

switch(filmes)
{
case 1:
printf("\n ingredientes: 3 ovos, 2 xícaras (chá) de açúcar, 2 xícaras (chá) de fubá, 3 colheres (sopa) rasas de farinha de trigo, 1/2 copo (americano) de óleo, 1 copo de leite, 1 colher (sopa) de fermento em pó");
printf("\n passo1: Bata todos os ingredientes no liquidificador.");
printf("\n passo2: Coloque em uma forma untada e enfarinhada.");
printf("\n passo3: Leve ao forno preaquecido e deixe assar, por cerca de 40 minutos.");
printf("fim");
break;

case 2:
printf("\n ingredientes: 3 ovos, Suco de 2 laranjas, 1 xícara (chá) de óleo, 2 xícaras (chá) de açúcar, 3 xícaras (chá) de farinha de trigo, 1 colher (sopa) de fermento em pó, Suco de 1 laranja, 2 colheres de sopa de açúcar");
printf("\n passo1: Bata no Liquidificador ou na batedeira os ovos, o suco da laranja, o óleo, e o açúcar.");
printf("\n passo2: Depois despeje em uma tigela e junte com a farinha e o fermento, bata tudo junto até a massa ficar homogênea.");
printf("\n passo3: Depois colocar em uma assadeira com furo untada com manteiga e farinha e levar para o forno.");
printf("\n passo4: Asse em forno médio, preaquecido, por cerca de 40 minutos, ou até dourar.");
printf("\n passo5: Calda: Fervente o suco da laranja com o açúcar em uma panela pequena, depois e só derramar em cima do bolo desenformado.");
printf("fim");
break;

case 3:
printf("\n ingredientes: 1 xícara de cenoura picada, 3 ovos, 1 xícara de açúcar, 1 xícara (chá) de óleo, 1 colher (sopa) de fermento em pó, 1 e 1/2 xícara de farinha de trigo, 1 lata de leite condensado, 4 colheres (sopa) de chocolate em pó, 1 colher (sopa) de margarina");
printf("\n passo1: Junte no liquidificador a cenoura, os ovos, o açúcar e o óleo e bata por uns 5 minutos.");
printf("\n passo2: Despeje este conteúdo em um recipiente, acrescente a farinha e o fermento e misture bem.");
printf("\n passo3: Unte com óleo uma forma de buraco central.");
printf("\n passo4: Leve ao forno em temperatura baixa, por mais ou menos, 40 minutos.");
printf("\n passo5: Para fazer a cobertura, utilize 1 lata de leite condensado, junte 4 colheres de sopa de chocolate em pó e uma colher de margarina.");
printf("\n passo6: Quando engrossar (mas um pouco antes de começar a aparecer o fundo da panela) está pronto.");
printf("fim");
break;

}
}while(filmes3);


return 0;
}
# K) 
# 1
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes, filmes2, filmes3;

printf("\num palhaço chega em você e diz assim:");
printf("\n vamos jogar um jogo!");
printf("\n em uma mão eu tenho uma moeda, se você acertar eu dou a moeda, senão você me da uma moeda");
printf("\n em qual mão o palhaço está com a moeda? 1 ou 2?");
scanf("%d", &filmes);
switch(filmes)
{
case 1:
printf("correto! + R$1,00");
break;
case 2:
printf("incorreto! - R$1,00");
break;
}
}
# 2
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes, filmes2, filmes3;

printf("\o seu pai pergunta a você o que você deseja no aniversario");
printf("\n você diz que quer jogos e uma bicileta");
printf("\n mas seu pai diz que ou um ou outro");
printf("\n 1 jogos  ou 2 bicicleta?");
scanf("%d", &filmes);
switch(filmes)
{
case 1:
printf("presente = Serie Batman Arkam");
break;
case 2:
printf("presente = Bicicleta");
break;
}
}
# 3
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()

{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int filmes, filmes2, filmes3;

printf("\n bem vindo ao restaurante xyz");
printf("\n cardapio:");
printf("\n 1 Feijoada");
printf("\n 2 Baião de 2");
scanf("%d", &filmes);
switch(filmes)
{
case 1:
printf("Feijoada");
break;
case 2:
printf("Baião de 2");
break;
}
}

# L)
#include<stdlib.h>
#include<stdio.h>
#include <locale.h>
int main()
{
//Permite o programa a ficar em português
setlocale(LC_ALL, "Portuguese");
printf("Utilizando acentuação da língua portuguesa! \n\n");


//Variáveis
int tamanhoM3, idade, tamanhoM2, tamanhoF2, tamanhoF3, contador, genero, tamanhoM, tamanhoF, acougue2, contador2, opcao, opcao2, opcao3, opcao4, opcao5, opcao6;

//introdução
printf("\nbem vindo ao Rei dos sapatos");
//escreve a idade
printf("\n qual a sua idade?");
printf("\n 1 infantil");
printf("\n 2 jovem");
printf("\n 3 adulto");
scanf("%d", &idade);
if (idade==1)
contador=1;
if (idade==2)
contador=2;
if(idade==3)
contador=3;

//escreve o gênero
printf("\n qual o seu genêro?");
printf("\n 1 Masculino");
printf("\n 2 Feminino");
scanf("%d", &genero);
if (genero==1)
contador2=1;
if (genero==2)
contador2=2;
if (genero==3)
contador2=3;

//separa os sapatos por idade, gênero e tamanho
if (contador==1 && contador2==1){
printf("\n qual o seu tamanho?");
printf("\n 1 13 a 20");
printf("\n 2 21 a 28");
printf("\n 3 29 a 35");
printf("\n 4 maior que 36");
scanf("%d", &tamanhoM);

switch(tamanhoM)
{
case 1:
    printf("escolha o tenis");
    printf("\n 1 Tenis bb canvas rn azul R$149,00");
    printf("\n 2 Tenis rmi rio knit R$349,00");
    printf("\n 3 Tenis infaltil calça-facil R$71,16");
    scanf("%d", &opcao);
    break;

case 2:
    printf("escolha o tenis");
    printf("\n 1 Tenis bb canvas rn azul R$149,00");
    printf("\n 2 Tenis rmi rio knit R$349,00");
    printf("\n 3 Tenis infaltil calça-facil R$71,16");
    scanf("%d", &opcao);
    break;

case 3:
    printf("escolha o tenis");
    printf("\n 1 Tenis bb canvas rn azul R$149,00");
    printf("\n 2 Tenis rmi rio knit R$349,00");
    printf("\n 3 Tenis infaltil calça-facil R$71,16");
    scanf("%d", &opcao);
    break;

case 4:
    printf("escolha o tenis");
    printf("\n 1 Tenis bb canvas rn azul R$149,00");
    printf("\n 2 Tenis rmi rio knit R$349,00");
    printf("\n 3 Tenis infaltil calça-facil R$71,16");
    scanf("%d", &opcao);
    break;
}
}

if (contador==2 && contador2==1){
printf("\n qual o seu tamanho?");
printf("\n 1 20 a 27");
printf("\n 2 28 a 35");
printf("\n 3 42 a 49");
printf("\n 4 maior que 50");
scanf("%d", &tamanhoM2);

switch(tamanhoM2)
{
case 1:
    printf("escolha o tenis");
    printf("\n 1 Hoops mid R$319,99");
    printf("\n 2 Sapatenis Polo Joy Casual R$99,90");
    printf("\n 3 Mormaii Urban Free R$142,90");
    scanf("%d", &opcao2);
    break;

case 2:
    printf("escolha o tenis");
    printf("\n 1 Hoops mid R$319,99");
    printf("\n 2 Sapatenis Polo Joy Casual R$99,90");
    printf("\n 3 Mormaii Urban Free R$142,90");
    scanf("%d", &opcao2);
    break;

case 3:
    printf("escolha o tenis");
    printf("\n 1 Hoops mid R$319,99");
    printf("\n 2 Sapatenis Polo Joy Casual R$99,90");
    printf("\n 3 Mormaii Urban Free R$142,90");
    scanf("%d", &opcao2);
    break;

case 4:
    printf("escolha o tenis");
    printf("\n 1 Hoops mid R$319,99");
    printf("\n 2 Sapatenis Polo Joy Casual R$99,90");
    printf("\n 3 Mormaii Urban Free R$142,90");
    scanf("%d", &opcao2);
    break;
}
}

if (contador==3 && contador2==1){
printf("\n qual o seu tamanho?");
printf("\n 1 20 a 27");
printf("\n 2 28 a 35");
printf("\n 3 42 a 49");
printf("\n 4 maior que 50");
scanf("%d", &tamanhoM3);

switch(tamanhoM3)
{
case 1:
    printf("escolha o tenis");
    printf("\n 1 Sapato Casual Pegada R$189,90");
    printf("\n 2 Sapato Masculino Microfibra Nobucado R$179,90");
    printf("\n 3 Ângelo R$490,00");
    scanf("%d", &opcao3);
    break;

case 2:
    printf("escolha o tenis");
    printf("\n 1");
    printf("\n 2");
    printf("\n 3");
    scanf("%d", &opcao3);
    break;

case 3:
    printf("escolha o tenis");
    printf("\n 1");
    printf("\n 2");
    printf("\n 3");
    scanf("%d", &opcao3);
    break;

case 4:
    printf("escolha o tenis");
    printf("\n 1");
    printf("\n 2");
    printf("\n 3");
    scanf("%d", &opcao3);
    break;
}
}


if (contador==1 && contador2==2){
printf("qual o seu tamanho?");
printf("\n 2 13 a 20");
printf("\n 2 21 a 28");
printf("\n 3 29 a 35");
printf("\n 4 maior que 36");
scanf("%d", &tamanhoF);

switch(tamanhoF)
{
case 1:
    printf("escolha o tenis");
    printf("\n 1 Ortopé bliss boot R$139,90");
    printf("\n 2 Bambuche infantil margarida R$39,90");
    printf("\n 3 Cano alto gatinha R$79,90");
    scanf("%d", &opcao4);
    break;

case 2:
    printf("escolha o tenis");
    printf("\n 1 Ortopé bliss boot R$139,90");
    printf("\n 2 Bambuche infantil margarida R$39,90");
    printf("\n 3 Cano alto gatinha R$79,90");
    scanf("%d", &opcao4);
    break;

case 3:
    printf("escolha o tenis");
    printf("\n 1 Ortopé bliss boot R$139,90");
    printf("\n 2 Bambuche infantil margarida R$39,90");
    printf("\n 3 Cano alto gatinha R$79,90");
    scanf("%d", &opcao4);
    break;

case 4:
    printf("escolha o tenis");
    printf("\n 1 Ortopé bliss boot R$139,90");
    printf("\n 2 Bambuche infantil margarida R$39,90");
    printf("\n 3 Cano alto gatinha R$79,90");
    scanf("%d", &opcao4);
    break;
}
}

if (contador==2 && contador2==2){
printf("\n qual o seu tamanho?");
printf("\n 1 20 a 27");
printf("\n 2 28 a 35");
printf("\n 3 42 a 49");
printf("\n 4 maior que 50");
scanf("%d", &tamanhoF2);

switch(tamanhoF2)
{
case 1:
    printf("escolha o tenis");
    printf("\n 1 AlL star wandinha R$124,06");
    printf("\n 2 R2000 R$80,90");
    printf("\n 3 Tênis Infantil Molekinha Para Adolescentes Moderno Original R$179,99");
    scanf("%d", &opcao5);
    break;

case 2:
    printf("escolha o tenis");
    printf("\n 1 AlL star wandinha R$124,06");
    printf("\n 2 R2000 R$80,90");
    printf("\n 3 Tênis Infantil Molekinha Para Adolescentes Moderno Original R$179,99");
    scanf("%d", &opcao5);
    break;

case 3:
    printf("escolha o tenis");
    printf("\n 1 AlL star wandinha R$124,06");
    printf("\n 2 R2000 R$80,90");
    printf("\n 3 Tênis Infantil Molekinha Para Adolescentes Moderno Original R$179,99");
    scanf("%d", &opcao5);
    break;

case 4:
    printf("escolha o tenis");
    printf("\n 1 AlL star wandinha R$124,06");
    printf("\n 2 R2000 R$80,90");
    printf("\n 3 Tênis Infantil Molekinha Para Adolescentes Moderno Original R$179,99");;
    scanf("%d", &opcao5);
    break;
}
}

if (contador==3 && contador2==2){
printf("\n qual o seu tamanho?");
printf("\n 1 20 a 27");
printf("\n 2 28 a 35");
printf("\n 3 42 a 49");
printf("\n 4 maior que 50");
scanf("%d", &tamanhoF3);

switch(tamanhoF3)
{
case 1:
    printf("escolha o tenis");
    printf("\n 1 Oxford Couro Confortavel R$304,90");
    printf("\n 2 Confortflex R$199,90");
    printf("\n 3 dois Pares Pares Sapatilha Femininas Sandalia Scarpin Rasteirinha Kit Atacado Sapato Feminino Mule Cores Da Moda Lançamento R$78,99");
    scanf("%d", &opcao6);
    break;

case 2:
    printf("escolha o tenis");
    printf("\n 1 Oxford Couro Confortavel R$304,90");
    printf("\n 2 Confortflex R$199,90");
    printf("\n 3 dois Pares Pares Sapatilha Femininas Sandalia Scarpin Rasteirinha Kit Atacado Sapato Feminino Mule Cores Da Moda Lançamento R$78,99");
    scanf("%d", &opcao6);
    break;

case 3:
    printf("escolha o tenis");
    printf("\n 1 Oxford Couro Confortavel R$304,90");
    printf("\n 2 Confortflex R$199,90");
    printf("\n 3 dois Pares Pares Sapatilha Femininas Sandalia Scarpin Rasteirinha Kit Atacado Sapato Feminino Mule Cores Da Moda Lançamento R$78,99");
    scanf("%d", &opcao6);
    break;

case 4:
    printf("escolha o tenis");
    printf("\n 1 Oxford Couro Confortavel R$304,90");
    printf("\n 2 Confortflex R$199,90");
    printf("\n 3 dois Pares Pares Sapatilha Femininas Sandalia Scarpin Rasteirinha Kit Atacado Sapato Feminino Mule Cores Da Moda Lançamento R$78,99");
    scanf("%d", &opcao6);
    break;
}
}
if (opcao == 1)
    printf("R$149,00");

if (opcao == 2)
    printf("R$349,00");

if (opcao == 3)
    printf("R$71,16");

if (opcao2 == 1)
    printf("R$319,99");

if (opcao2 == 2)
    printf("R$99,90");

if (opcao2 == 3)
    printf("R$142,90");

if (opcao3 == 1)
    printf("189,90");

if (opcao3 == 2)
    printf("179,90");

if (opcao3 == 3)
    printf("490,00");

if (opcao4 == 1)
    printf("R$139,90");

if (opcao4 == 2)
    printf("R$39,90");

if (opcao4 == 3)
    printf("R$79,90");

if (opcao5 == 1)
    printf("R$124,06");

if (opcao5 == 2)
    printf("R$80,90");

if (opcao5 == 3)
    printf("R$179,99");

if (opcao6 == 1)
    printf("R$304,90");

if (opcao6 == 2)
    printf("R$199,90");

if (opcao6 == 3)
    printf("R$78,99");
}

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
