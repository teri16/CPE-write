![image](https://github.com/teri16/CPE-write/assets/144236243/abd15e9e-5115-4fbc-9ebb-260607e5695c)


## 需要判斷數字是否可以被整除 並列出


```cpp
#include<iostream>
#include<vector>
using namespace std;

int main()
{
	vector <int>ans;
	int n,m;
	while(cin>>n>>m)
	{
		bool boring = false;
		if(n==0||m==0)boring = true; //不為0
		if(m==1)boring = true;		//除數為1
		while(n>1)
		{
		if(n%m==0)
		{
			ans.push_back(n);
			n/=m;
		}
		else 
		{
		boring = true;
		break;
		}
		}
		if (boring==1)
		{
			cout<<"Boring!"<<endl;
		}
		else
		{
		for (auto i : ans)cout<<i<<" ";
		cout <<1<<endl;
		}
		ans.clear();
	}
	
	return 0;
}
```
## 解題重點
+ for(auto i:vector)很好用
+ bool來進行判斷

