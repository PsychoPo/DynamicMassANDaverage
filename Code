#include <stdio.h>
#include <windows.h>
#include <malloc.h>

int main() {
	int j,i,k,sum,ave,N;

	j = 0;
	k = 0;
	sum = 0;
	ave = 0;

	printf("Enter the size of the array - ");
	scanf_s("%i", &N);
	int *pX = (int*)malloc(N * sizeof(int));

	for (int i = 0; i < N; i++) {
		pX[i] = rand() % 10;
		//printf("Enter a number:");
		//scanf_s("%i", &pX[i]);
	}

	for (int i = 0; i < N; i++) {
		printf("A[%i] = %i\n", i ,pX[i]);
	}

	for (int i = 0; i < N; i++) {
		k++;
		sum += pX[i];
	}

	ave = sum / k;
	printf("Average of default array = %i\n", ave);

	k = 0;
	sum = 0;
	ave = 0;

	int *pY = (int*)malloc((N * 2) * sizeof(int));
	for (int i = 0; i < (N * 2); i++) {
		if (i % 2 == 0) {
			pY[i] = pX[j];
			j++;
		}
		else {
			printf("Enter a number:");
			scanf_s("%i", &pY[i]);
		}
	}

	free(pX);

	for (i = 0; i < (N * 2); i++) {
		printf("A[%i] = %i\n", i ,pY[i]);
	}

	for (int i = 0; i < (N * 2); i++) {
		k++;
		sum += pY[i];
	}

	free(pY);

	ave = sum / k;
	printf("Average of modified array = %i\n", ave);
}
