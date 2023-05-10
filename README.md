
#include <stdio.h>
#include <stdlib.h>

void insertionsort( int *v, int tam){
    for ( int i = 1; i< tam; i++){
        for( int j = i;j > 0 && v[j-1] > v[j]; j--){
            int aux = v[j-1];
                v[j-1] = v[j];
                v[j] = aux;
        }
    }

}

 void ImprimeVetor(int V[], int n) {
    printf("[%d", V[0]);
    int i;
        for (i = 1; i < n; i++) {
            printf(", %d",V[i]);
        }
    printf("]\n");
}

int main(){

    int v[] = {5,2,4,8,1,0,7,11,23,3};
    int n = 10;
        
        insertionsort ( v, n);
        ImprimeVetor ( v , n);
        
         return 0;

}





