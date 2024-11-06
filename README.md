#include<stdio.h>
void main()
{
  int i,j,a[3][3],m,n,b[3][3];
  printf("enter the number of rows in the matrix\n");
  scanf("%d",&m);
  printf("enter the numbe of coloumns in the matrix\n");
  scanf("%d",&n);
  printf("enter the elements of the matrix\n");
  for(i=0;i<m;i++)
    {
    for(j=0;j<n;j++)
      {
      scanf("%d",&a[i][j]);
      }
    }
  printf("elements of the matrix are\n");
  for(i=0;i<m;i++)
    {
    for(j=0;j<n;j++)
      {
      printf("%d",a[i][j]);
      }
    printf("\n");
    }
  for(i=0;i<m;i++)
    {
    for(j=0;j<n;j++)
      {
      b[i][j]=a[j][i];
      }
    }
  printf("transpose of a matrix\n");
  for(i=0;i<m;i++)
    {
    for(j=0;j<n;j++)
      {
      printf("%d",b[i][j]);
      }
    printf("\n");
    }
