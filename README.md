# repo
#include <iostream>

using namespace std;

int main()
{
   int n,m,i,j,a[20][20],sum1=0,sum2=0;
   cin>>n;
   cin>>m;
   for(i=0;i<n;i++){
       for(j=0;j<m;j++){
           cin>>a[i][j];
       }
   }
   for(i=0;i<n;i++){
       for(j=0;j<n;j++){
           if(i==j){
               sum1+=a[i][j];
           }
           if(i+j==n-1){
               sum2+=a[i][j];
           }
       }
   }
   cout<<abs(sum1-sum2);
}
