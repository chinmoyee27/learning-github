# learning-github
this is the trial ....
by chinmoyee paul

//modular arithmatic
#include<bits/stdc++.h>
#define ll long long 
#define optimize() ios_base::sync_with_stdio(0);cin.tie(0);cout.tie(0);
using namespace std;

//mod kore final ans ; mod related kisu hoile doble float ashbe na,m prime nmbr


int main()
{
    optimize();
    long long bigmod(long long a, long long b, ll m){
     if(b == 0){
          return 1;
     }
     if(b&1){
          return ((a%m)* ((bigmod(a,b-1,m)%m)%m))
     }
     else {
          long long x = bigmod(a,b/2,m);
     }
     x = (x*x)%m; return x;
    }
}
