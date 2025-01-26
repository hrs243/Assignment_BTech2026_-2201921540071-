# Assignment_BTech2026_-2201921540071-
# Problem 1: Using inheritance, one class can acquire the properties of others. Consider the following Animal class:
# Platform Used : HackerRank

In C++, we can achieve similar functionality by using inheritance. We start with an "Animal" class that has only one method, "walk":

class Animal{
public:
    void walk(){
        cout <<"I am walking"<<endl;
    }
};

Next, we create a "Bird" class that inherits from the "Animal" class and adds a "fly" method. This is done using the "public" inheritance specifier:

class Bird : public Animal{
public:
    void fly(){
        cout <<"I am flying"<<endl;
    }
};

Now, a "Bird" object can both "walk" and "fly", since it inherits all the properties and behaviors of the "Animal" class.

Finally, we add a "sing" method to the "Bird" class and modify the "main" function to demonstrate the functionality:

#include<iostream>
using namespace std;

class Animal{
public:
    void walk(){
        cout<<"I am walking"<<endl;
    }
};

class Bird:public Animal{
public:
    void fly(){
        cout<<"I am flying"<<endl;
    }
    void sing(){
        cout <<"I am singing"<<endl;
    }
};

int main(){
    Bird bird;
    bird.walk();
    bird.fly();
    bird.sing();
    return 0;
}


The output of this C++ code will be:

I am walking
I am flying
I am singing

This demonstrates that the "Bird" class has all the properties of the "Animal" class and also has its unique methods.
