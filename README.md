# primeiros-codigos-


#include <stdio.h>

int main() {
    int idade;
    char categoria;
    float preco;
    int quantidade;

    printf("Informe a sua idade: ");
    scanf("%d", &idade);

    printf("Informe a categoria do ingresso (1 para estudante, 2 para idoso, 3 para outra categoria ): ");
    scanf(" %c", &categoria);

    printf("Informe a quantidade de ingressos que deseja comprar: ");
    scanf("%d", &quantidade);

    if (categoria == '1') {
        if (idade < 12) {
        } else {
            preco = 15.0;
        }
    } else if (categoria == '2') {
        if (idade >= 60) {
            preco = 15.0;
        } else {
            printf("Categoria invalida para a sua idade!\n");
            return 0;
        }
    } else if (categoria == '3') {
        preco = 30.0;
    } else {
        printf("Categoria invalida!\n");
        return 0;
    }

    float total = preco * quantidade;
    printf("O preco total dos ingressos e: R$ %.2f\n", total);

    return 0;
}
  
