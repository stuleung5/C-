# C-
Coding I’ve uploaded. I copied and paste many of them from the Sololearn App. I’ve also copied and pasted some from my Arduino projects.

Car Project: 


#include <iostream>
#include <string>
using namespace std;
int Speed=50;
int x=0;
class Car {
    //complete the class, add makeSound() method
    public: 
		void haveColor() {
			cout<<"Blue"<<endl;
		}
		void haveName(string x) {
			name = x;
		}
		string getName() {
			return name;
		}
       void use() {
          Speed-=50;
            }
       void getSpeed() { 
       	for (x; x<10; x++) {
       		if (x!=9) {
          		cout << Speed+x*1+2<<" mph vroom"<<endl;
          		Speed=Speed+x*1+2;
          	}
          	else {
          		cout << "0"<<" mph brrr"<<endl;
          		Speed=0;
          	}
          }
        }
		private: 
    		string name;
};



int main() {
    
    //instantiation
    Car test;
    
    //function call
    test.haveColor();
    Car myObj;
	 myObj.haveName("Honda");
	 cout << myObj.getName()<<endl;
	 Car p;
    p.use();
    Car *ptr = &p;
    ptr->getSpeed();
    
    return 0;
}
