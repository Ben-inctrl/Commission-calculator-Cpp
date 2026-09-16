# Commission-calculator-Cpp
A program that calculates commission of an agent and outputs the agent name and commission earned.

#include <iostream> 
using namespace std;
int main(){
    string agentName;
    long salesVol;
    float commission;
    cout<<"Enter the agent name:"<<endl;
    getline (cin,agentName);
    cout<<"\nEnter the sales volume:"<<endl;
    cin>>salesVol;
    switch(salesVol){ 
        case 0 ... 1999:
        commission = (0.03*salesVol); 
        break;
        case 2000 ... 2999:
        commission = (0.06*salesVol);
        break;
        case 3000 ... 3999:
        commission = (0.09*salesVol);
        break;
        case 4000 ... 4999:
        commission = (0.12*salesVol);
        break;
        case 5000 ... 1000000000:
        commission = (0.15*salesVol);
        break;
        default:
        cout<<"Invalid input:"<<endl;
        break; }
    cout<<"\nThe agent name is:"<<agentName<<endl;
    cout<<"\nThe commission is:"<<commission<<endl;
return 0;
}

