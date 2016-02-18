# Tugas

#include<stdio.h>

int main(){
    int in1, in2, in3;
    char in_1,in_2;

    printf("Demo Struktur Kondisi\n");
    printf("======================\n");
    printf("Masukkan Bilangan Asli 1 : ");
    scanf("%c", &in_1);
    getchar();
    in1 = (int)in_1;
    if (in1 >= 48 && in1 <= 57)
        in1-=48;
    else{
        printf("Bilangan 1 yang anda salah");
        return 0;
    }
    printf("Masukkan Bilangan Asli 2 : ");
    scanf("%c", &in_2);
    getchar();
    in2 = (int)in_2;
    if (in2 >= 48 && in2 <= 57)
        in2-=48;
    else{
        printf("Bilangan 2 yang anda masukkan salah");
        return 0;
    }
    printf("\nJenis Operator");
    printf("\n===============\n");
    printf("1. Contoh Operator Aritmatika\n");
    printf("2. Contoh Operator Relasional\n");
    printf("3. Contoh Operator Logikal\n");
    printf("Pilihan [1-3] : ");
    scanf("%d", &in3);
    if(in3==1){
        printf("\nContoh Operator Aritmatika");
        printf("\nPenjumlahan : %d + %d = %d",in1, in2, in1+in2);
        printf("\nPerkalian : %d x %d = %d", in1, in2, in1*in2);
    }
    else if(in3==2){
        printf("\nContoh Operator Relasional");
        printf("\nPersamaan : %d == %d = ",in1, in2);
        if(in1 == in2)
            printf("TRUE");
        else
            printf("FALSE");
        printf("\nPertidaksamaan : %d != %d = ", in1, in2);
        if(in1 == in2)
            printf("FALSE");
        else
            printf("TRUE");
    }
    else if(in3==3){
        printf("\nContoh Operator Logical");
        printf("\nLogika AND : %d && %d = %d", in1, in2, in1&&in2);
        printf("\nLogika OR : %d || %d = %d", in1, in2, in1||in2);
    }
    else
        printf("\nPilihan tidak valid harap masukkan nilai 1, 2, dan 3");
    getch();
    return 0;
}
