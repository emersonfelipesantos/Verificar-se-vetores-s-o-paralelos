#include <stdio.h>


int saoParalelos(int u1, int u2, int v1, int v2) {

    return (u1 * v2 == u2 * v1);
}

int main() {
    int u1, u2, v1, v2;
    printf("Digite os componentes do vetor u (u1, u2): ");
    scanf("%d %d", &u1, &u2);

    printf("Digite os componentes do vetor v (v1, v2): ");
    scanf("%d %d", &v1, &v2);


    if (saoParalelos(u1, u2, v1, v2)) {
        printf("Os vetores são paralelos.\n");
    } else {
        printf("Os vetores não são paralelos.\n");
    }

    return 0;
}
