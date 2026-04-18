1-Inheritance:
What is the main benefit of Inheritance in OOP??
-It allows a class (Child) to reuse properties and methods from another class (Parent)
-so you don’t have to rewrite the same code again
-helps organize code and makes it easier to maintain and extend.

Give a simple example of a Parent class and a Child class??

class Person {
    public $name;
    public $age;
    public function introduce() {
        return "My name is " . $this->name;
    }
}
class Student extends Person {
    public $grade;
    public function study() {
        return $this->name . " is studying";
    }
}
$student = new Student();
$student->name = "Ziad";
$student->age = 20;
$student->grade = "A";

echo $student->introduce(); // My name is Ziad
echo $student->study();     // Ziad is studying



--------------------------------------------------------------------
2-The final Keyword:

What happens if you put the final keyword before a class or a method?? 

final before a class ==> No other class can extend it.
final before a method ==>the method cannot be overridden in any child class.

Why would a developerwant to use this??

-Protection 
-Prevent modification
-Avoid bugs 


--------------------------------------------------------------------------
3-Overriding Methods:

What does it mean to "override" amethod in a child class??
-Means a child class provides its own implementation of a method that already exists in the parent class.

How can you call the original parent method from inside the child's overridden method??
-With parent::method().

----------------------------------------------------------------------------
4-Abstract Class vs. Interface:

Abstract Class:
-Have Abstract methods without body
-Have Properties
-Have Methods with implementation

Interface:
-Not Have Properties
-Not Have Methods implementation
-Only defines what methods


Can a class implement multiple interfaces??
-A class can implement MULTIPLE interfaces

--------------------------------------------------------------------------
5-Polymorphism:

what is Polymorphism??
-Different objects can use the same method name, but each one does something different.

Example:

class Person {
    public function cut() {
        return "Person is cutting";
    }
    class Doctor extends Person {
    public function cut() {
        return "Doctor performs surgery";
    }
}

class Barber extends Person {
    public function cut() {
        return "Barber cuts hair";
    }
}

class Actor extends Person {
    public function cut() {
        return "Actor cuts the scene";
    }
}

-->Each one has a function called cut with the same name, but each one uses it according to their job.






















    
}




























































