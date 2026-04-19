# calculator.cpp
A simple calculator in c++ that performs basic arithmetic operations
#include<iostream>
using namespace std;
int main()
{
char op;
    double num1, num2;
    std::cout << "Enter operator (+, -, *, /): ";
    std::cin >> op;
    std::cout << "Enter two operands: ";
    std::cin >> num1 >> num2;

    switch (op) {
        case '+':
            std::cout << num1 << " + " << num2 << " = " << num1 + num2 << std::endl;
            break;
        case '-':
            std::cout << num1 << " - " << num2 << " = " << num1 - num2 << std::endl;
            break;
        case '*':
            std::cout << num1 << " * " << num2 << " = " << num1 * num2 << std::endl;
            break;
        case '/':
            if (num2 != 0) {
                std::cout << num1 << " / " << num2 << " = " << num1 / num2 << std::endl;
            } else {
                std::cout << "Error! Division by zero." << std::endl;
            }
            break;
        default:
            std::cout << "Error! Invalid operator." << std::endl;
            break;
    }
    return 0;
    }
