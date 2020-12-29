// decimal-conversion
//for binary to decimal cconversion put c* = 2
//for octal to decimal cconversion put c* = 8
#include <iostream>

using namespace std;
int decimal(int n){
    int temp,bin=0,c=1;
    while(n!=0){
        
        temp = n%10;
        bin=bin+temp*c;
        c*=2;
        n=n/10;
    }
    return bin;
}
int main()
{
    int n;
    cout<<"enter the binary number: ";
    cin>>n;
    cout<<decimal(n);

    return 0;
}
