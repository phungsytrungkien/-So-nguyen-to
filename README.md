
#include <stdio.h>

int main(){
	int n,i,SNT=1;
	printf("Nhap so N: ");
	scanf("%d", &n);
	
	if(n<2){
		SNT=0;		
	}else{
		for(i=2; i<=sqrt(n); i++){
			if(i%2==0){
				SNT=0;
               break;
			}
		}
	}
	if(SNT)
		printf("%d La so nguyen to\n", n);
	else 
		printf("%d Khong phai la so nguyen to", n);
	
	return 0;
}
