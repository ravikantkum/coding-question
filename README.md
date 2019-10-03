# coding-question
code for xor opreation


#include<bits/stdc++.h>
using namespace std;
int main(){

    //code for anagrame string in c++.
  string str,str1;
  cin>>str>>str1;
  int x=0;
  for (int i = 0; i < str.size(); ++i)
  {
      cout<<x <<" "<<"xor"<<" "<<str[i]<<endl;
      x^=str[i] ;
      cout<<x <<" "<<"xor"<<" "<<str1[i]<<endl;
      x^=str1[i];
  }
  if(x==0)
    cout<<"y";
   else
       cout<<"n";

    int n,val;
    cin>>n;
  code for missing one copy  

vector<int>A,B;
        for(int i=0;i<n;i++){
            cin>>val;
            A.push_back(val);
        }
int val1=0;
for (int i = 0; i < n; ++i)
{
    val1^=A[i];
}
cout<<val1<<endl;



code for missing number



int n,val; cin>>n;
vector<int>A,B;
        for(int i=0;i<n;i++){
            cin>>val;
            A.push_back(val);
        }
int val1=A[0];
int val2=1;
for (int i = 1; i <n; ++i)
{
    val1^=A[i];
}
for (int i = 2; i <=n+1 ; ++i)
{
    val2^=i;
}
cout<< (val1^val2)<<endl;

return 0;
}
