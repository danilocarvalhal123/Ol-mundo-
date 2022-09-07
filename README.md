# Ol-mundo-
Estou começando a movimentar meu GitHub, por conseguinte, estou aprendendo a mexer na plataforma. 
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
// Faça um programa que leia um nome de usuário e a sua senha e não aceite a
// senha igual ao nome do usuário, mostrando uma mensagem de erro e voltando a
// pedir as informações.
int main(void) {

  char u[8], senha[8];
  int retorno;

  printf("insira seu usuário: ");
  scanf("%s", &u);
  printf("insira sua senha: ");
  scanf("%s", &senha);

  retorno = strcmp(u, senha);

  while (retorno == 0) {

    printf("\nA senha não pode ser igual ao usuário: \n");
    printf("insira seu usuário: ");
    scanf("%s", &u);
    printf("insira sua senha: ");
    scanf("%s", &senha);
    retorno = strcmp(u, senha);
  }

  printf("\nInformção salva com sucesso!");

  return 0;
}
