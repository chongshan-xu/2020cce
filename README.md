# 2020CCE

# 第一週的實習課程式

## 第一題 進階題：分式化簡
#include <stdio.h>
int main ()
{
	int a,b;
	int ans=0;
	scanf("%d%d",&a,&b);
	for (int i=1 ; i<=b; i++)
	{
		if (a%i==0 && b%i==0) ans=i;
	}
	printf("%d %d\n",a/ans,b/ans);
}
## 第二題 進階題：讀入整數反序列印
#include <stdio.h>
int main ()
{
	int a[11];
	int ans=0;
	for (int i=1 ; i<=10 ; i++)
	{
		 scanf("%d",&a[i]);
		 ans++;
		 if(a[i]==0) break;
	}
	for (int k=ans-1; k>=1 ; k--)
	{
		printf("%d ",a[k]);
	}
	printf("\n");
}
## 第三題 進階題：A的B次方函數
#include <stdio.h>
int MYPOWER(int A,int B)
{
	int ans=1;
	for (int i=1 ; i<=B ; i++)
	{
		ans*=A;
	}
	return ans;
}
int main(void)
{
	int a,b;
	scanf("%d%d",&a,&b);
	printf("[%d]",MYPOWER(a,b));
	return 0;
}
## 第四題 進階題：漸增數列相加
#include <stdio.h>
int main ()
{
	int a;
	int ans=0;
	scanf("%d",&a);
	for(int i=1 ; i<=a-1 ; i++)
	{
		ans=i*(i+1)+ans;
	}
	printf("%d\n",ans);
}
## 第五題 基礎題：找零錢 
#include <stdio.h>
int main ()
{
	int a;
	scanf("%d",&a);
	printf("%d=50*%d+5*%d+1*%d\n",a,a/50,a%50/5,a%50%5/1);
}
## 第六題 基礎題：因數個數 
#include <stdio.h>
int main ()
{
	int a;
	int b=0;
	scanf("%d",&a);
	for (int i=1 ; i<=a ; i++)
	{
		if (a%i==0) b++;
	}
	printf("%d\n",b);
}
## 第七題 基礎題：找倍數 
#include <stdio.h>
int main ()
{
	int a[10];
	int b=0;
	for (int i=1 ; i<=10 ; i++)
	{
		scanf("%d",&a[i]);
	}
	for (int k=1 ; k<=10 ; k++)
	{
		if (a[k]%3==0) b++;
		
	}
	printf("%d\n",b);
}
## 第八題 基礎題：整數轉換為等級
#include <stdio.h>
int main()
{
	int a;
	scanf("%d",&a);
	if(a>=90) printf("A\n");
	else if(a>=80) printf("B\n");
	else if(a>=60) printf("C\n");
	else printf("F\n");
}
