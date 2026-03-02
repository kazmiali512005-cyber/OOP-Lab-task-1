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
TASK #include <iostream>
using namespace std;

struct Student {
    string firstName;
    string lastName;
    int rollNumber;
    float marks;

    // Member function
    void displayStudentInfo() {
        cout << "\nFull Name: " << firstName << " " << lastName << endl;
        cout << "Roll Number: " << rollNumber << endl;
        cout << "Marks: " << marks << endl;
    }
};

int main() {
    int n;

    cout << "Enter number of students: ";
    cin >> n;

    // Array of structures
    Student students[n];

    // Input details
    for(int i = 0; i < n; i++) {
        cout << "\nEnter details for Student " << i + 1 << endl;

        cout << "First Name: ";
        cin >> students[i].firstName;

        cout << "Last Name: ";
        cin >> students[i].lastName;

        cout << "Roll Number: ";
        cin >> students[i].rollNumber;

        cout << "Marks: ";
        cin >> students[i].marks;
    }

    // Display details
    cout << "\n----- Student Information -----" << endl;

    for(int i = 0; i < n; i++) {
        students[i].displayStudentInfo();
    }

    return 0;
}2

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

