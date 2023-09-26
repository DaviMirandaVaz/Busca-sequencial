#include <stdio.h>
#include <stdlib.h>

int main(){
	int i, tam, n, num, numencontrado = 0;
	printf("Quantas posicoes o vetor tera?\n");
	scanf("%d", &tam);
	int vet[tam];
	for(i = 0; i < tam; i++){
		system("cls");
		printf("Qual o %d valor do vetor:", i+1);
		scanf("%d", &vet[i]);
	}
	system("cls");
	printf("Qual o numero a ser buscado?");
	scanf("%d", &num);
	for(i=0;i<tam;i++){
		if(num == vet[i]){
			numencontrado = i;
			break;
		}
	}
	system("cls");
	if(numencontrado == 0){
		printf("\nNumero nao esta no vetor");
		
	}else{
	printf("A posicao do valor buscado e %d", numencontrado+1);
	}
	return 0;
}
