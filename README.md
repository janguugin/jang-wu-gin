#include <iostream>
using namespace std;

int main() {
    char op;
    float num1, num2;

    cout << "첫 번째 숫자를 입력하세요: ";
    cin >> num1;

    cout << "두 번째 숫자를 입력하세요: ";
    cin >> num2;

    cout << "연산자를 입력하세요 (+, -, *, /): ";
    cin >> op;

    switch (op) {
        case '+':
            cout << "결과: " << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << "결과: " << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << "결과: " << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << "결과: " << num1 << " / " << num2 << " = " << num1 / num2 << endl;
            else
                cout << "0으로 나눌 수 없습니다." << endl;
            break;
        default:
            cout << "유효하지 않은 연산자입니다." << endl;
            break;
    }

    return 0;
}
