#include <iostream>
#include <string>
using namespace std;

template <class T>
class Stack
{
private:
    T arr[100];
    int top;

public:
    Stack()
    {
        top = -1;
    }

    void push(T value)
    {
        if (top == 99)
            cout << "Stack Overflow\n";
        else
            arr[++top] = value;
    }

    void pop()
    {
        if (top == -1)
            cout << "Stack Underflow\n";
        else
            cout << "Popped: " << arr[top--] << endl;
    }

    void display()
    {
        if (top == -1)
        {
            cout << "Stack is empty\n";
            return;
        }

        cout << "Stack: ";
        for (int i = top; i >= 0; i--)
            cout << arr[i] << " ";
        cout << endl;
    }
};

int main()
{
    // Integer Stack
    Stack<int> s1;
    s1.push(10);
    s1.push(20);
    s1.push(30);

    cout << "Integer Stack:\n";
    s1.display();
    s1.pop();

    // Float Stack
    Stack<float> s2;
    s2.push(1.5);
    s2.push(2.5);
    s2.push(3.5);

    cout << "\nFloat Stack:\n";
    s2.display();
    s2.pop();

    // String Stack
    Stack<string> s3;
    s3.push("Apple");
    s3.push("Banana");
    s3.push("Mango");

    cout << "\nString Stack:\n";
    s3.display();
    s3.pop();

    return 0;
}
