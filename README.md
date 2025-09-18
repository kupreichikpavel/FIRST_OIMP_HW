#include <iostream>
using namespace std;


using namespace std;

int main() {
    int n;
    cin >> n;
    int myN =n;
    int reverse = 0;
    while (n != 0) {
        reverse = reverse * 10 + (n % 10);
        n /= 10;
    }
    if (reverse==myN) {
        cout << "polindrom";
    }else {
        cout << "not polindrom";
    }
    return 0;
}

/*№1
int number;
cout << "Please enter a number:" << endl;
cin >> number;
for (int i = 0; i < number; i++) {
    if (number % i == 0) {
        cout << i << " ";
    }
}
return 0;
}
-----------------------
№ 3
int main() {
    int n;
    cin >> n;
    if (n < 1) {
        cout << "Error" << endl;
    }
    int printed = 0;
    int x = 2;
    while (printed < n) {
        bool prime = true;
        for (int d = 2; d * d <= x; ++d) {
            if (x % d == 0) {
                prime = false;
                break;
            }
        }
        if (prime) {
            cout << x << ' ';
            ++printed;
        }
        ++x;
    }
    cout << '\n';
    return 0;
}
*/
