# Ex-6-IMPLEMENTATION-OF-THE-BACK-END-OF-THE-COMPILER-
IMPLEMENTATION OF THE BACK END OF THE COMPILER 
# Aim :
To write a program to implement the back end of the compiler.
# ALGORITHM
1. Start the program.
2. Get the three variables from statements and stored in the text file k.txt.
3. Compile the program and give the path of the source file.
4. Execute the program.
5. Target code for the given statement is produced.
6. Stop the program.
# PROGRAM
```
Name: ELAMARAN S E
REG NO: 212222230036
#include <stdio.h>
#include <ctype.h>
#include <stdlib.h>
int main()
{
    int i = 2, j = 0, k = 2, k1 = 0;
    char ip[10], kk[10];
    FILE *fp;
    printf("Enter the filename of the intermediate code: ");
    scanf("%s", kk);
    fp = fopen(kk, "r");
    if (fp == NULL) {
        printf("\nError in opening the file\n");
        return 1;
    }
    printf("\nStatement\tTarget Code\n\n");
    while (fscanf(fp, "%s", ip) != EOF)
    {
        printf("%s\tMOV %c,R%d SUB ", ip, ip[i + k], j);
        if (ip[i + 1] == '+')
            printf("ADD ");
        else
            printf("SUB ");
        if (islower(ip[i]))
            printf("%c,R%d\n", ip[i + k1], j);
        else
            printf("%c,%c\n", ip[i], ip[i + 2]);
        j++;
        k1 = 2;
        k = 0;
    }
    fclose(fp);
    return 0;
}
```
# OUTPUT
![382996626-ce4f5f97-5466-45e6-bac2-e5e722b98ce1](https://github.com/user-attachments/assets/035e7902-d489-4970-b12e-235f8f26409b)
# PROGRAM OUTPUT
![382996928-4484a98a-b634-4ae2-a239-0f55d32b5483](https://github.com/user-attachments/assets/a97912fb-53f2-42ae-a5ed-f39032e26df6)

# Result
The back end of the compiler is implemented successfully, and the output is verified.
