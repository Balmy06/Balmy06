
#include <stdio.h>

double CalcularF(int op, double T);

int main()
{
    int op;
    double T, F;

    printf("   Calculo de F.\n\n");
    printf("1. F = T / 5\n");
    printf("2. F = T^2\n");
    printf("3. y 4. F = (6 * T) / 2\n");
    printf("\nSelecciona una operacion: "); scanf("%d", &op);

    printf("\nIngrese el valor de T: "); scanf("%lf", &T);

    switch (op)
    {
        case 1:
            {
            F = CalcularF(op, T);
            printf("\nEl valor de F es: %lf\n", F);
            break;
            }
        case 2:
            {
            F = CalcularF(op, T);
            printf("\nEl valor de F es: %lf\n", F);
            break;
            }
        case 3:
            {
            F = CalcularF(op, T);
            printf("\nEl valor de F es: %lf\n", F);
            break;
            }
        case 4:
            {
            F = CalcularF(op, T);
            printf("\nEl valor de F es: %lf\n", F);
            break;
            }
        default:
            {
            printf("\nF = 1\n");
            break;
            }
    }

    return 0;
}

double CalcularF(int op, double T)
{
    double F;

    if (op == 1)
    {
        F = T / 5.0; // Asegurarse de que la división sea en punto flotante
    }
    else if (op == 2)
    {
        F = T * T;
    }
    else
    {
        F = (6.0 * T) / 2.0; // Asegurarse de que la multiplicación y división sean en punto flotante
    }
    return F;
}
