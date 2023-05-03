# Read-number-in-array.cpp
#include <iostream>
using namespace std;

int main() {
	int t,i,a,b,n,c,count,g;
	cin>>n;
	for(t=0;t<n;t++)
	{
	    count=0;
	    g=0;
	    cin>>a;
	    b=a;
	    do
	    {
	        count++;
	        b/=10;
	    }while(b!=0);
	    int c[10];
	    for(i=count;i>0;i--)
	    {
	        c[i] = a % 10;
	        if(c[i]==4)
	        {
	            g++;
	        }
	        a /= 10;
	    }
	    cout<<g<<"\n";
	}
	return 0;
}
