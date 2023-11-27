#include <stdio.h>
#include <stdlib.h>
#include<math.h>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main() {
	printf("Ax^2+Bx+C=D\n***SEKLINDEKI IKINCI DERECEDEN BIR DENKLEMIN KOKLERINI BULMA UYGULAMASI***\n");
	int a,b,c,d;
	float dis,dis2,byk1,byk2,est,kck1,kck11,kck2,kck22,kck3;
	printf("A degerini giriniz: ");
	scanf("%d",&a);
	printf("\n%dx^2+Bx+C=D",a);
	printf("\nB degerini giriniz: ");
	scanf("%d",&b);
	printf("\n%dx^2+%dx+C=D",a,b);
	printf("\nC degerini giriniz: ");
	scanf("%d",&c);
	printf("\n%dx^2+%dx+%d=D",a,b,c);
	printf("\nD degerini giriniz: ");
	scanf("%d",&d);
	printf("\nDenklemimiz= %dx^2+%dx+%d=%d",a,b,c,d);
	
	dis=sqrt((b*b)-(4*a*c));
	dis2=sqrt(-1*((b*b)-(4*a*c)));
	
	if(dis>0)
	{
	printf("\n\nIki Reel Kok Vardir!\nBu Kokler:\n");
	byk1=(-(b)+dis)/(2*a);
	byk2=(-(b)-dis)/(2*a);
	printf("\nBirinci Kok=(%f)",byk1);
	printf("\nIkinci Kok=(%f)",byk2);
	}
	if(dis==0)
	{
	est=((-(b))/(a));
	printf("\n\nKok=%f",est);
	}
	if(dis2>0)
	{
    printf("\n\nReel kok yoktur!\nImajiner Kokler vardir. \nBu Kokler:");

    kck1=(-(b));
    kck11=(2*a);
    kck2=(-(b));
    kck22=(2*a);
	printf("\n\n Kok1=(%f)-(%fi)/(%f)",kck1,dis2,kck11);
	printf("\n\n Kok2=(%f)+(%fi)/(%f)",kck2,dis2,kck22);
		
    }
	return 0;
}
