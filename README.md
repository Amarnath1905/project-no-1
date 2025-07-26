#include <iostream>
using namespace std;

int main()
{   char op;
    float num1,num2;
    cout<<"enter the operator:";
    cin>>op;
    cout<<"enter the numbers:";
    cin>>num1>>num2;      //here i was used cin>>num1,num2 but via this only input of one number will be taken so i used << again to yake input for both the numbers
    switch(op){
        case '+':  // in cpp : says now begin the values for this case
            cout<<"result:"<<num1+num2;
            break;
        case '-':
                cout<<"result:"<<num1-num2;
            break;     // in cpp ; is used as a full stop so after break we have to stop this case here 
        case '*':
            cout<<"result:"<<num1*num2;
            break;
        case '/':
            if(num2 != 0)
                cout<<"result:"<<num1/num2;
            else
                cout<<"not defined";
            break;
        default:            //used when the condition is if all the above conditions are not fitting in ur input then this will be the out put
            cout<<"invalid operation";
    
    }
    
    

    return 0;
}
