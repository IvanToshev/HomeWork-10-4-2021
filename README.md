# HomeWork-10-4-2021
Define Variable

#include <stdio.h>

    int main()
    {
        signed char iNum = - 127;
        unsigned short iNum1 = 255;
        unsigned short iNum2 = 63498;
        unsigned int iNum3 = 4294967292;
        signed long long iNum4 = -9000000000000775845;

        printf("\n%i, %d, %d, %u,%lli", iNum,iNum1,iNum2,iNum3,iNum4);
        return 0;


    }
    
    /*7. Дефинирайте променливи със стойност 24 212, -1 357 674, 1 357 674, -1 357 
674 000, 3 657 895 000.
Изведете всяка променлива на екрана със printf()*/

#include <stdio.h>

    int main()
    {

        unsigned short int iNum =  24212;
        int iNum1 = -1357674;
        int iNum2 = 1357674;
        long int iNum3 = -1357674000;
        unsigned long int iNum4 = 3657895000;

        printf("\n %hu, %d, %d, %ld, %lu", iNum, iNum1, iNum2, iNum3, iNum4);
    }
    
    
/*8. Да прочетем какво се случва със стойността на променливата x:
char x = 8;
x = x -2;
x= x+ 6;
x= x – 10 + 2;
Каква ще бъде стойността на x, ако я отпечатаме на екрана след последната 
калкулация?*/

#include <stdio.h>

int main()
{

    char x = 8;
    x = x - 2; //8 = 8-2 = 6
    x = x + 6; // 6 = 6+6
    x = x - 10 + 2; //12 = 12- 10+2


    printf("%d", x);
    return 0;
}


#include <stdio.h>
/*9. Дефинирайте променливи със стойност
4.9876543, 7.123456789012345678890, 18 398 458 438 583 853.28, 18 398 458 438 
583 853.39875937284928422.
 */
int main()
{
    double fNum = 4.9876543;
    double fNum1 = 7.123456789012345678890;
    long double fNum2 = 18398458438583853.28;
    long double fNum3 = 18398458438583853.39875937284928422;

    printf("%.7f,%.20lf, %.10le, %.10le", fNum, fNum1, fNum2, fNum3);
    return 0;
}
/*double var2 = 7.1234567890123456789123456789;
    printf("\n normal:%.30lf\n sci:%.30le \n or \n sci:%.30E   \n",var2,var2 ,var2);
    return 0;
} */

/* 3.1728816725e-317*/
// 3.172882e-317


/*10. Представете си, че имате фирма за отдаване на каравани и кемпери под 
наем, за която трябва да разработите софтуер. Вие сте малка фирма и имате 
общо 3 каравани на цена 90 лв. на ден и 3 кемпера на цена 100 лв. на ден. 
Декларирайте променливи за броя на караваните, цената на караваните, броя на 
кемперите и цената им. Направете меню, което пита клиента каравана или 
кемпер ще иска. Направете променлива, в която да се събират парите, които 
клиента дължи на компанията. Принтирайте резултата */

#include <stdio.h>

    int main()
    {
        int caravans = 3; 
        int campers = 3;
    

        float pricePerCaravan = 90;
        float pricePerCamper = 100;

        int choice = 0;

        int days = 0;
        float totalPrice = 0;

        printf("\n Pleace enter type of vehicle.If caravan, press 1, if camper press 2: ");
        scanf("%d", &choice);

        if (choice == 1 )
        {
            printf("\n For how may days ?:");
            scanf("%d", &days);
            totalPrice = days * (pricePerCaravan / caravans);
            printf("Your price will be: %.2f lv. ", totalPrice);

        }
        else if(choice == 2)
        {
            printf("\n For how many days ?:");
            scanf("%d", &days);
            totalPrice = days * (pricePerCamper / campers);
            printf("Your price will be: %.2f lv. ", totalPrice);

        }
        else if(choice > 2 || choice < 1 )
        { 
            printf("Wrong choice ! Try again !");

        }

    }
    
   /* 12. Напишете програма PrintPatterns, която отпечата следните текстови графики 
на екрана. Графиките една под друга: */

#include <stdio.h>

int main() {

    printf("# # # # # # # # # # #\n");
    printf("  # # # # # # # # # \n");
    printf("    # # # # # # #\n");
    printf("      # # # # #\n");
    printf("        # # #\n");
    printf("          #\n");
    printf("         (a)    \n\n\n");

printf("\n");
printf("\n");
printf("\n");

    printf("            #\n");
    printf("          # # #\n");
    printf("        # # # # #\n");
    printf("      # # # # # # #\n");
    printf("    # # # # # # # # #\n");
    printf("  # # # # # # # # # # #\n");
    printf("           (b)");

printf("\n");
printf("\n");
printf("\n");


    printf("            #\n");
    printf("          # # #\n");
    printf("        # # # # #\n");
    printf("      # # # # # # #\n");
    printf("    # # # # # # # # #\n");
    printf("  # # # # # # # # # # #\n");
    printf("    # # # # # # # # #\n");
    printf("      # # # # # # #\n");
    printf("        # # # # #\n");
    printf("          # # #\n");
    printf("            #\n");
    printf("           (c)");
    return 0;

}
