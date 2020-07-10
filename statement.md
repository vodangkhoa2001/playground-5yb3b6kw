#include<iostream>
#include<string>
using namespace std;
int main()
{
    string s;
    getline(cin,s);cin>>.ignore();
    for(int i=0;i<=s.length;i++)
    {
        s[i]+=(s[i]>='a'&& s[i]<='z')?-32:(s[i]>='A'&&s[i]<='Z') ?32:0;
    }
    cout<<s;
    system("pause");
}
