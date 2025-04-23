#include <iostream>
using namespace std;

class AddAmount {
private:
    double amount;

public:
    AddAmount() { amount = 50; } // Default constructor (no amount added)
    AddAmount(double addAmt) { amount = 50 + addAmt; } // Parameterized constructor

    void display() { cout << "Final amount in Piggie Bank: $" << amount << endl; }
};

int main() {
    AddAmount a1;      // No amount added
    AddAmount a2(30);  // Adding $30

  a1.display();
    a2.display();

  return 0;
}
