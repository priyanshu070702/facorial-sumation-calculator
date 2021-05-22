# facorial-sumation-calculator

#include <iostream>

using namespace std;

int sum(int n){
    if(n==0){
        return 0;
    }
    else{
        return sum(n-1)+n;
    }
}
int fac(int m){
    if(m==0){
        return 1;
    }
    else{
        return fac(m-1)*m;
    }
}

int main()
{
    int choice,a,b;
    cout<<"choices are"<<endl;
    cout<<"press 1 for sum till a given number"<<endl;
    cout<<"press 2 for factorial of a number"<<endl;
    cout<<"for exit"<<endl;
    cout<<endl;
    do{
    cout<<"enter thr choice"<<endl;
    cin>>choice;
    
    
    switch(choice){
        case 1: cout<<"enter the number"<<endl;
        cin>>a;
        cout<<sum(a)<<endl;
        break;
        
        case 2: cout<<"enter the number"<<endl;
        cin>>b;
        cout<<fac(b)<<endl;
        break;
        
        default: cout<<"exited"<<endl;
    }
    }while(choice!=3);
    return 0;
}
