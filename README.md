# OOP-Lab-task-1
TASK 1#include <iostream>
using namespace std;

struct Student {
    string firstName;
    string lastName;
    int rollNumber;
    float marks;

    // Member function
    void displayStudentInfo() {
        cout << "Full Name: " << firstName << " " << lastName << endl;
        cout << "Roll Number: " << rollNumber << endl;
        cout << "Marks: " << marks << endl;
    }
};

int main() {
    // Structure variable
    Student s1;

    // Assign values to data members
    s1.firstName = "Ali";
    s1.lastName = "Khan";
    s1.rollNumber = 101;
    s1.marks = 85.5;

    // Call member function
    s1.displayStudentInfo();

    return 0;
}

