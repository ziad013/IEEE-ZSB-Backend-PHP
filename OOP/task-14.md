1-Class vs Object:
Class => a blueprint
Object => actual thing
like this
class Car {
public:
    string color;
    int speed;
};
Car car1;
car1.color = "Red";
car1.speed = 120;

---------------------------------------------------------------------------------
2-$this vs. self:: :
self:
-Refer to current class
-Access static members
-Not use ($) because its not represent a variable But present class constructoin
this:
-Refer to current object
-Access not static members
-Not use ($) because its represent a variable 

----------------------------------------------------------------------
3-Access Modifiers (Encapsulation):
public => Accessible from anywhere
private => Accessible only inside the class
protected => Accessibl in derived classes

 why you would make a property private??
 --> to Protect data and Prevent incorrect usage
 example:
 class Student {
private:
    int grade;

public:
    void setGrade(int g) {
        if (g >= 0 && g <= 100) {
            grade = g;
        }
    }
};

if public => This breaks the system because grades should be within a valid range

----------------------------------------------------------------
4-Typed Properties:

Typed Properties =>define the data type of class properties like string and int

how do they help prevent bugs ??
-Prevent wrong data from being assigned
-Catch errors early
-Make code more predictable
-Improve code readability

-------------------------------------------------------------
5-Constructor Methods:
What is __construct() used for??
-to initialize the properties of object

Why is passing arguments to the constructor useful?>
-Initialize the object immediately
-Make code cleaner and shorter
-Enforce required data


























