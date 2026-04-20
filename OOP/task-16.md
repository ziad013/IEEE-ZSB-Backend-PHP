1-Traits:

How do "Traits" solve this problem??
-Trait is basically a group of methods that you can “inject” into a class with use keyword

when should you use them??
-You have common methods shared across multiple unrelated classes
-to compine with pros alot of classes

------------------------------------------------------------------------
2-Namespaces:

What is a Namespace in PHP??
-A Namespace in PHP is a way to organize your code and avoid conflicts by grouping classes, functions, or constants under a unique name.

Explain how it prevents "naming collisions" when you have two classes with the same name?

class Student {
    public function info() {
        echo "University Student";
    }
}

class Student {
    public function info() {
        echo "Course Student";
    }
}
solution ==> put each class in a different namespace like this

namespace University;

class Student {
    public function info() {
        echo "University Student";
    }
}
namespace Course;

class Student {
    public function info() {
        echo "Course Student";
    }
}

-----------------------------------------------------------------
3-Autoloading:

What is Autoloading??
-Autoloading is a feature in PHP that automatically loads class files when they are needed, instead of requiring you to manually include them using require.

How does it save time??
-No need to write require for every class
-Reduces repetitive code
-Prevents errors from missing requires

----------------------------------------------------------------------
4-Magic Methods (__get and __set): 

What are the __get and__set magic methods used for??
-__get and __set are magic methods used to control access private properties or properties that don’t exist.

__set ==> triggered when you try to assign a value to a property.
__get ==> triggered when you try to access a property.

-----------------------------------------------------------------------
5-Static Methods and Properties:

What does it mean when a method or property is declared as static??
-Static Property ==> Can be called without creating an object
-Static Method ==> Can be called without creating an object

Do you need to create an object using the new keyword to access a static method??
-No






































