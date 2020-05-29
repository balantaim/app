// # C++ app

#define _USE_MATH_DEFINES
#include <iostream>
#include <math.h>
#include <cmath>

using namespace std;
double triangle(double &a, double &b, double &c)
{
    double P = 0;
    P = a + b + c;
    return P;
}

double rectangle(double& a, double& b)
{
    double P = 0;
    P = (2*a) + (2*b);
    return P;
}
double circle(double &d)
{
    double C = 0;
    
    C = d* M_PI;
    return C;
}







int main()
{
    int stage1;

    cout << "You could calculate the perimeter/length of the figure\n";
    cout << "Choice one figure\n for triangle press '1'\n for rectangle press '2'\n for circle press '3'\n";
    cin >> stage1;
    if (stage1 == 1) {
        double a, b, c;
        cout << "Insert three sides\n";
        cin >> a >> b >> c;
        cout << "P=" <<  triangle(a, b, c) << endl; }
    else if (stage1 == 2) {
        double a, b;
        cout << "Insert two sides\n";
        cin >> a >> b;
        cout << "P=" << rectangle(a, b) << endl; }
    else if (stage1 == 3) {
        double d;
        cout << "Insert diameter\n";
        cin >> d;
        cout << "C=" << circle(d) << endl;}
    else {
        cout << "The number is incorrect";
    }
    cin.ignore();
    cout << "Have a nice day!";
    cin.get();






}

