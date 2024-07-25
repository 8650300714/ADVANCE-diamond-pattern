# ADVANCE-diamond-pattern
#include <iostream>
using namespace std;
void Diamondpattern (int n)
{	//first half of pattern
	for(int i=0; i<n; i++)
	{
		for(int j=0; j<(2*n); j++)
		{
			if((i+j)<=n-1)// upper left side triangle
			{
				cout<<"*";
			}
			else {
				cout<<" ";
			}
			if((n+i)<=j)// upper right side triangle
			{
				cout<<"*";
			}
			else
			{
				cout<<" ";
			}
		}
		cout<<endl;
	}
	//second part of pattern
	for(int i=0; i<n; i++)
	{
		for(int j=0; j<=(2*n); j++)
		{
			if(i>=j)//bottom left side
			{
				cout<<"*";
			}
			else
			{
				cout<<" ";
			}
			if(i>=(2*n-1)-j)//bottom right side
			{
				cout<<"*";
			}
			else
			{
				cout<<" ";
			}
		}
		cout<<endl;
	}
}
int main()

{
	int n;
	cout<<"enter the value you want to print the pattern"<<endl;
	cin>>n;
	Diamondpattern(n);
	cout<<endl;
	return 0;
}

OUTPUT
![image](https://github.com/user-attachments/assets/dd4e0082-7cf7-4ba3-8d75-3085e6c520bd)
