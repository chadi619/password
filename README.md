#include<stdio.h>
#include<conio.h>
#include<windows.h>
main(){
char pass[55],ch;
int i,dlt=strlen(pass);
	printf("enter the password:");	
	i=0;
	while(1){
	ch=getch();
	if(ch==13){ //enter key = 13 in ascii
		pass[i]='\0';
		break;
	}if(ch==8){ //delete key=8 in ascii
		pass[--i];
		printf("\b \b");
    
	continue;
	}
	pass[i++]=ch;
	printf("*");	
	}	
	printf("\nthe password you enterd is:%s",pass);
}
