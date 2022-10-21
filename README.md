#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main(){
	setlocale(LC_ALL, "Portuguese");
	
	int opcao, m1, m2, resultado, md1, md2, md3, media; 
	
	
	printf("\tCALCULADORA DE MULTIPLICACAO OU MEDIA DE 3 NUMEROS\n");
	
	printf("\n\nDigite 1 para multiplicar:\nDigite 2 para media de 3 numeros:\n");
	scanf("%d", &opcao);
	
	
	if(opcao==1){
		fflush(stdin);
		system("cls");
		
		
		printf("\tCALCULADORA DE MULTIPLICACAO.\n");
		
		printf("\nDigite um numero:\n");
		scanf("%d", &m1);
		fflush(stdin);
		
		printf("\nDigite o segundo numero:\n");
		scanf("%d", &m2);
		fflush(stdin);
		
		resultado = m1*m2;
		printf("\nO resultado na multiplicacao dos numeros %d x %d e:\n%d", m1, m2, resultado);
	
		
	}else{
		if(opcao==2){
			fflush(stdin);
			system("cls");
			
			printf("\tCALCULADORA DA MEDIA DE 3 NUMEROS.\n");
			
			printf("\nDigite o primeiro valor:\n");
			scanf("%d", &md1);
			fflush(stdin);
			
			printf("\nDigite o segundo valor:\n");
			scanf("%d", &md2);
			fflush(stdin);
			
			printf("\nDigite o terceiro valor:\n");
			scanf("%d", &md3);
			fflush(stdin);
			
			media = md1+md2+md3/3;
			printf("\nA media dos numeros %d - %d - %d e:\n%d", md1, md2, md3, media);
			
		}else{
			printf("\n\tOpcao Invalida.");
		}
	}
}
