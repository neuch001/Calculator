#include <iostream>
#include <Windows.h>
using namespace std;

int main() {
    setlocale(LC_ALL, "ru");

    double a, b;
    char op;

    cout << "Введите выражение (например: 5 + 3): ";
    cin >> a >> op >> b;

    if (op == '+') cout << "Результат: " << a + b << endl;
    else if (op == '-') cout << "Результат: " << a - b << endl;
    else if (op == '*') cout << "Результат: " << a * b << endl;
    else if (op == '/') {
        if (b == 0) cout << "Ошибка: деление на ноль!\n";
        else cout << "Результат: " << a / b << endl;
    }
    else cout << "Неудачная операция!\n";

    return 0;
}
