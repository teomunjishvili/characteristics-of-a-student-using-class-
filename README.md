#include<iostream>
#include<string>
using namespace std;
class student
{
        int age;
        string forename;
        string lastname;
        string email;
        float height;
    public:
        student () /*no arguments passed to the constructor*/
        {
            age = 20;
            forename = "Teo";
            lastname = "Munjishvili";
            email = "teomunjishvili@gmail.com";
            height = 1.60;
        }
        
        student (int a) /*one argument is passed to the constructor*/
        {
            age = a;
            forename = "Natia";
            lastname = "Metonidze";
            email = "n.metonidze@gmai.com";
            height = 1.75;
            cout<<"Different constructor is used"<<endl;
        }
        
        student (int a, string b) /*two arguments are passed to the constructor*/
        {
            age = a;
            forename = b;
            lastname = "Okruashvili";
            email = "n.okruashvili@gmail.com";
            height = 1.85;
            void exit(int); /*stop execution*/
        }
        
        
        void get_values()
        {
            cout<<"Age: "<<age<<endl;
            cout<<"Forename: "<<forename<<endl;
            cout<<"Lastname: "<<lastname<<endl;
            cout<<"Email: "<<email<<endl;
            cout<<"Height: "<<height<<endl;
            
        }
};

int main()
{
    student obj1(), obj2(19), obj3(21, "Nana");
    obj1.get_values();
    obj2.get_values();
    obj3.get_values();
    return 0;
}
