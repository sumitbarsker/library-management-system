#include <iostream>
#include <string>
using namespace std;

// simple library class
class Library {
    int id[5];
    string name[5];
    int qty[5];
    int n;

public:
    Library() {
        n = 3;

        id[0] = 101;
        name[0] = "C++";
        qty[0] = 5;

        id[1] = 102;
        name[1] = "DS";
        qty[1] = 3;

        id[2] = 103;
        name[2] = "OOP";
        qty[2] = 4;
    }

    void show() {
        cout << "\nBook List:\n";
        for (int i = 0; i < n; i++) {
            cout << "Book ID: " << id[i] << endl;
            cout << "Book Name: " << name[i] << endl;
            cout << "Quantity: " << qty[i] << endl;
            cout << "--------------\n";
        }
    }

    void issue() {
        int b;
        cout << "Enter book id: ";
        cin >> b;

        for (int i = 0; i < n; i++) {
            if (id[i] == b) {
                if (qty[i] > 0) {
                    qty[i] = qty[i] - 1;
                    cout << "Book issued\n";
                } else {
                    cout << "Book not available\n";
                }
                return;
            }
        }
        cout << "Wrong book id\n";
    }

    void giveBack() {
        int b;
        cout << "Enter book id: ";
        cin >> b;

        for (int i = 0; i < n; i++) {
            if (id[i] == b) {
                qty[i] = qty[i] + 1;
                cout << "Book returned\n";
                return;
            }
        }
        cout << "Wrong book id\n";
    }
};

int main() {
    Library l;
    int ch;

    do {
        cout << "\n1. Show Books";
        cout << "\n2. Issue Book";
        cout << "\n3. Return Book";
        cout << "\n4. Exit";
        cout << "\nEnter choice: ";
        cin >> ch;

        if (ch == 1)
            l.show();
        else if (ch == 2)
            l.issue();
        else if (ch == 3)
            l.giveBack();
        else if (ch == 4)
            cout << "Exit\n";
        else
            cout << "Invalid choice\n";

    } while (ch != 4);

    return 0;
}
