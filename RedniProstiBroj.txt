#include <stdio.h>
#include <stdlib.h>

int jeliprost(int num){

 int dailine=1;

  int brojac;

   for(brojac=2; brojac<=num/2; brojac++ )
   {
       if(num%brojac==0){dailine=0;break;}
   }

return dailine;}

int redniprostibr(int n){

    int brojac;

    int glavnibrojac=0;

       for(brojac=2; brojac>=1; brojac++)

        if( jeliprost(brojac)){

                glavnibrojac++;

        if(glavnibrojac==n)  break;

    } return brojac;

}

int main()
{
    int n;

    //Ucitaj n

    scanf("%d", &n);


    printf("%d", redniprostibr(n));

    return 0;
}
