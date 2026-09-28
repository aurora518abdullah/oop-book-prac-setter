#include<bits/stdc++.h>
using namespace std;
class Book{
private:
    string tital;
    double price;
public:
    Book(string tital,double price)
    {

        this->tital=tital;
        this->price = price;
    }
    Book( const Book &o)
    {
        this->tital=o.tital;
        this->price=o.price;
    }

    void display()
    {
        cout<<"Tital: "<<tital<<" | Price: "<<price<<endl;
    }
    void setp(double price)
    {
        this->price=price;
    }

};
int main()
{

    Book ob1("c++ primer",49.99);
    Book ob2(ob1);
    ob1.display();
    ob2.display();
    ob2.setp(98.3);
    ob2.display();
}
