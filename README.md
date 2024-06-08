#include <iostream>
#include <string>
using namespace std;

class BankAccount{
   public:
    BankAccount(string n,int d):name(n)
    {
        Setdeposite (d);
    }
    
  void  Setdeposite (int d){
      balance+=d;
      cout <<"Your current balance is "<<balance<<endl;
  }
  
  void withdraw (int w){
      if(balance<w)
      cout<<"There is not the amount of money in your balance.";
      else
      balance-=w;
  }
    private:
    int balance=0;
    string name;
    
};

https://youtu.be/Tz7FsunBbfQ?si=ap8NU7lTWbN4TizK


int main() {
BankAccount b("Fidan",10000);
b.withdraw(1000);
b.Setdeposite(500);


    return 0;
}
