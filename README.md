#include <iostream>
using namespace std;

void checkAge(int age) {
    if (age < 18 || age > 70) {
        cout << "Error: Age is not within the acceptable range for entry." << endl;
        // Additional code for denying entry or providing an alternative action
        exit(0); // Exit the program if age is not within the acceptable range
    }
}

int main() {
    int clientAge;

    cout << "Welcome to Nii's Avenue Club!" << endl;
    cout << "Please enter your age: ";
    cin >> clientAge;

    checkAge(clientAge);
    cout << "Congratulations! You are eligible for entry." << endl;
    // Additional code for allowing the client to enter the facility

    return 0;
} 