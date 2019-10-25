#include
#include
using namespace std;
int main()
{
int a,b,c,num,sum,n,t=0;
for(num=100;num<=999;num++)
{
a=num;//求位数
b=num;//求每位的数字
n=0;//用于储存位数
//计算位数
while(a!=0)
{
a=a/10;
n++;
}
// 计算 各位的n次方之和
while(b!=0)
{
c=b%10;
sum +=pow(c,n);
b/=10;

	 }
	 if(num==sum) cout<<num<<endl;//判断是否为水仙数 
	 
sum=0;//初始化sum	 
}
return 0;
}
