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

Problem 2-

A Java abstract class is a class that can't be instantiated. That means you cannot create new instances of an abstract class.

ollowing is an example of abstract class:

abstract class Book{ String title; abstract void setTitle(String s); String getTitle(){ return title; } } If you try to create an instance of this class like the following line you will get an error:

Book new_novel=new Book(); You have to create another class that extends the abstract class. Then you can create an instance of the new class.

Notice that setTitle method is abstract too and has no body. That means you must implement the body of that method in the child class.

In the editor, we have provided the abstract Book class and a Main class. In the Main class, we created an instance of a class called MyBook. Your task is to write just the MyBook class.

Your class mustn't be public.

Sample Input

A tale of two cities Sample Output

The title is: A tale of two cities

Solution- 1-FIRSTLY WE CREATE A ABSTRACT CLASS BOOK WHICH CONTAINS A ATTRIBUTE TITLE, DECLARING A PURE VIRTUAL MEMBER FUNCTION SETTITLE SETTING THE TITLE AND A MEMBER FUNCTION GETTILE RETURNING TITLE VALUE.

2-THEN WE MOVE ON TO CRETAE A CHILD CLASS EXTENDING BASE ABSTRACT CLASS IMPLEMENTING THE BASE CLASS VIRTUAL FUNCTION SETTITLE INSIDE IT.

3-IN MAIN FUNCTION AN OBJECT OF CHILD CLASS IS CREATED.

4-IT SETS THE TITLE USING OBJ.SETTITLE(PARAMETER).

5-FINALLY IT PRINTS THE TITLE NAME USING GETTITLE MEMBER FUNCTION.

PROBLEM 3-

Write the following code in your editor below:

A class named Arithmetic with a method named add that takes integers as parameters and returns an integer denoting their sum. A class named Adder that inherits from a superclass named Arithmetic.

SOLUTION- 1-MADE A BASE CLASS NAMED ARITHMETIC.
2-THEN INCLUDED MEMBER FUNCTION TO RETURN THE SUM OF TWO INTEGERS PASSED BY USER
3-INHERITED THE BASED CLASS AND NAMED IT ADDER 
4-CREATED CHILD CLASS OBJECT IN MAIN FUNCTION AND CALLED BASE CLASS METHOD USING INHERITANCE 
5-OUTPUT WAS SCUCCESFULLY GENERATED



PROBLEM 4-Write a C++ program to create a class called Triangle that has private member variables for the lengths of its three sides. Implement member functions to determine if the triangle is equilateral, isosceles, or scalene.

SOLUTION- 1-The program defines a Triangle class to determine the type of a triangle based on its three side lengths.

2- It uses a constructor to initialize the side lengths of the triangle.

3- The triangletype() method returns one of the three types of triangles: Equilateral Triangle (all three sides are equal) Isosceles Triangle (two sides are equal) Scalene Triangle (all sides are different)

4- The main() function creates a Triangle object with predefined values and prints the triangle type.



PROBLEM-
Write a C++ program to implement a class called Date that has private member variables for day, month, and year. Include member functions to set and get these variables, as well as to validate if the date is valid.

SOLUTION-
This C++ program defines a Date class to handle date-related operations.

It includes member functions to set, retrieve, and validate a date.

The isValidDate() function checks if a given date is valid, considering leap years and month-day constraints.

The main() function takes user input for day, month, and year, then validates and displays the date.

If the date is valid, a confirmation message is displayed; otherwise, an invalid date message is shown.



// Problem 10.
//  Write a C++ program to implement a class called Shape with virtual member functions for calculating area and perimeter. Derive classes such as Circle, Rectangle, and Triangle from the Shape class and override virtual functions accordingly.


Solution-

1-Implements an abstract base class Shape with pure virtual functions (area() and perimeter()).

2-Uses constructors to accept shape dimensions dynamically.

3-Circle, Rectangle, and Triangle classes override area() and perimeter() functions.

4-Heron's formula is used for triangle area calculation.

5-Demonstrates polymorphism by enforcing method implementation in derived classes.

PROBLEM 9- Eligibility Checker for Students You are tasked with designing a simple program that determines the eligibility of students based on their scores and ages.

Class Definitions:

Student class: Attributes: name (String): The name of the student. score (int): The student's academic score. age (int): The age of the student. Methods: eligible(): A method that checks the student's eligibility and prints "YES" if the score is greater than 10 and the age is greater than 20. Otherwise, it prints "NO."

SOLUTION-

1-Student Class Implementation - Defines a Student class with attributes: name, score, and age.

2-Eligibility Check - The eligible() method checks if a student qualifies based on a score greater than 10 and age above 20.

3-Object Creation & Initialization - Creates a Student object in main(), assigning values to name, score, and age.

4-Output Behavior - Prints "YES" if the student meets the criteria, otherwise prints "NO".

5-Simple OOP Concept - Demonstrates basic class, object, and method usage in C++.

