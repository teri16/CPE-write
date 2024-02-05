```cpp=
#include<iostream>
using namespace std;
int main()
{
	double a,b,c;
	cin>>a>>b;
	c=b/(a*a);

	cout<<c<<endl;
	if(c<18.5)
		cout<<"too thin";
	else if(c>=18.5&&c<24)
		cout<<"standard";
	else
		cout<<"too fat";
		
	return 0;
	
}
```
+ `if`語法使用