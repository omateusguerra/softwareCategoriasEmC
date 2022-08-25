# softwareCategoriasEmC
Seguindo os primeiros passos na linguagem C, esse software recebe o ano de nascimento do usuário (nadador) e informa a categoria a qual pertence.

#include <stdio.h>
#include <locale.h>


int main()
{
    int anoNascimento = 0;

    setlocale(LC_ALL,"Portuguese");
   
    printf("SOFTWARE DE CATEGORIAS DE NATAÇÃO POR IDADE! \n");

    printf("Digite o ano de nascimento: \n");
    scanf("%d",&anoNascimento);

    int idade = 2023 - anoNascimento;

    if(idade >= 5 && idade <= 7){
        printf("Sua categoria é: Infantil A!");
    }else if(idade >= 8 && idade <= 10){
        printf("Sua categoria é: Infantil B!");
    }else if(idade >= 11 && idade <= 13){
        printf("Sua categoria é: Juvenil A!");
    }else if(idade >= 14 && idade <= 17){
        printf("Sua categoria é: Juvenil B!");
    }else if(idade > 17){
        printf("Sua categoria é: Sênior!");
    }else {
        printf("Sua idade não atende a nenhuma categoria!");
    };
   
    return 0;
};
