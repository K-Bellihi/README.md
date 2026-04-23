#include <stdio.h>
#include <stdlib.h>

/* ─── Fonction principale ─────────────────────────────── */

int* construct_transformed_array(int* nums, int n) {
    
    /* Allouer la mémoire pour le tableau résultat */
    int* result = (int*)malloc(n * sizeof(int));
    
    for (int i = 0; i < n; i++) {
        if (nums[i] == 0) {
            result[i] = 0;
        } else {
            int index = ((i + nums[i]) % n + n) % n;
            result[i] = nums[index];
        }
    }
    
    return result;
}

/* ─── Fonction utilitaire pour afficher un tableau ───── */

void
