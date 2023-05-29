# insert
#include<stdio.h>
int main()
{
	int arr[50];
	int i,pos,len,ele;
	scanf("%d",&len);
	for(i=0;i<len;i++)
	scanf("%d",&arr[i]);
	scanf("%d%d",&pos,&ele);
	if(pos>=0&&pos<50)
	{
		for(i=len;i>pos;i--)
		arr[i]=arr[i-1];
		arr[pos]=ele;
		len++;
		for(i=0;i<len;i++)
		printf("%d",arr[i]);
	}
	else
	printf("\nout of bounds");
}

