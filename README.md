# test





#include<iostream>
using namespace std;

void main()
{
	char a[21], b, key;
	cout << "请输入字符串和密钥: ";
	cin >> a >> b;
	for (int i = 0; a[i] != 0; i++)
	{
		a[i] = a[i] ^ b;
	}
	cout << "加密后: ";
	for (int k = 0; a[k] != 0; k++)
	{
		cout << a[k];
	}
	cout << endl << "请输入密码: ";

	cin >> key;
	for (int j = 0; a[j]!= 0;j++)
	{
		a[j] = a[j] ^ key;
	}
	for (int g = 0; a[g] != 0; g++)
	{
		cout << a[g];
	}
	cout << endl;
}
