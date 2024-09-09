#include <stdio.h>

#define TAMANHO_VETOR 10

int main() {
    int vetor1[TAMANHO_VETOR];
    int vetor2[TAMANHO_VETOR];
    int vetorSoma[TAMANHO_VETOR];
    int i;

    // Leitura do primeiro vetor
    printf("Digite os %d números inteiros do primeiro vetor:\n", TAMANHO_VETOR);
    for (i = 0; i < TAMANHO_VETOR; i++) {
        scanf("%d", &vetor1[i]);
    }

    // Leitura do segundo vetor
    printf("Digite os %d números inteiros do segundo vetor:\n", TAMANHO_VETOR);
    for (i = 0; i < TAMANHO_VETOR; i++) {
        scanf("%d", &vetor2[i]);
    }

    // Soma dos elementos de mesmo índice
    for (i = 0; i < TAMANHO_VETOR; i++) {
        vetorSoma[i] = vetor1[i] + vetor2[i];
    }

    // Impressão do vetor resultante
    printf("Vetor resultante:\n");
    for (i = 0; i < TAMANHO_VETOR; i++) {
        printf("%d ", vetorSoma[i]);
    }

    printf("\n");

    return 0;
}
