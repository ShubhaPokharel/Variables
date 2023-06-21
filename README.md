# Variables

Variables are used to store the data. It is like a placeholder.

## Three types of Variables: 

1 - Local Variables

2 - Instance Variables

3 - Static variables


### Local Variables...

Local variables are declared inside the method or constructor or blocks.

We can access the local variables inside the method, constructor or block dierectly .


## Instance Variable...

Instance Variables are declared inside the class.

We can access Instance variables with in the object name. To create the object we use the class name. All methods that are in the class access the Instance variables.

Memory of Instance variable is created ( allocated ) when the object is created.

When object is created seperate seperate memory is created for each Instance variable.

## Static Variable..

Static variables are declared inside the class. We use the static modifier to make the variable static.

We can access the static variable using the class name.

The memory of Static variable is allocted ( created ) when the class is loaded.

## When to use Static variables and Instance variables?

When the data is common to all objects we use the Static variable.

When the data is specific ( different ) to the object we use the Instance variable.


### Example: 

package com.pnc.model;

public class Test {

    //Instance variables

    int num1 = 10;

    int num2 = 20;


    //static variables

    static int val1 = 100;

    static int val2 = 200;

    public static void main(String[] args){

    // local variables

    int l = 1000;

    int j = 2000;

    System.out.println("Local var - " + (l + j));

    Test t = new Test();

    System.out.println("Instance var - " + (t.num1 + t.num2));

    System.out.println("Static var - " + (Test.val1 + Test.val2));

   }

}
