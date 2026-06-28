#include <stdio.h>

int main() {
    int yellowLeaves, brownSpots, whitePowder, holes, curling;

    printf("=========\n");
    printf("   Plant Leaf Disease Prediction System\n");
    printf("=========================================\n\n");

    printf("Answer with 1 for Yes and 0 for No\n\n");

    printf("Are the leaves yellow? ");
    scanf("%d", &yellowLeaves);

    printf("Are there brown spots? ");
    scanf("%d", &brownSpots);

    printf("Is there white powder on leaves? ");
    scanf("%d", &whitePowder);

    printf("Are there holes in leaves? ");
    scanf("%d", &holes);

    printf("Are the leaves curling? ");
    scanf("%d", &curling);

    printf("\n=========================================\n");
    printf("Prediction Result\n");
    printf("=========================================\n");

    if (whitePowder) {
        printf("Disease: Powdery Mildew\n");
        printf("Recommendation: Apply sulfur or neem oil fungicide.\n");
    }
    else if (brownSpots && yellowLeaves) {
        printf("Disease: Leaf Spot Disease\n");
        printf("Recommendation: Remove infected leaves and apply fungicide.\n");
    }
    else if (yellowLeaves && curling) {
        printf("Disease: Leaf Curl Virus\n");
        printf("Recommendation: Control insects and remove infected plants.\n");
    }
    else if (holes) {
        printf("Disease: Insect Attack\n");
        printf("Recommendation: Use suitable insecticide or neem spray.\n");
    }
    else if (yellowLeaves) {
        printf("Disease: Nutrient Deficiency\n");
        printf("Recommendation: Apply nitrogen-rich fertilizer.\n");
    }
    else {
        printf("Plant appears Healthy.\n");
        printf("Recommendation: Continue regular watering and care.\n");
    }

    printf("\nThank you for using the Plant Leaf Disease Prediction System.\n");

    return 0;
}
