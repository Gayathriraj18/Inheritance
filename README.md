# Inheritance

## Aim:

To write a C# program to print some messages using hierarchical inheritance.

## Algorithm:

# Step 1:
Create a base class.

# Step 2:
Create two child class.

# Step 3:
Create a constructor in the base class and print a message.

# Step 4:
create a function in child class to print a message.


## Program:
```
using System;

namespace ex_8
{
    class tyre
    {
        public tyre()
        {
            Console.WriteLine("Tyre Constructor");
        }
        public virtual void display()
        {
            Console.WriteLine("Methods in Tyre class");
        }
    }
    class scooter : tyre
    {


        public scooter()
        {
            Console.WriteLine("scooter Constructor");
        }
        public override void display()
        {
            base.display();
        }
    }
    class car : tyre
    {

        public car()
        {
            Console.WriteLine("Car Constructor");
        }
        public override void display()
        {
            base.display();
        }
    }
    class program
    {
         static void Main(string[]args)
        {
            scooter s= new scooter();
            s.display();
            car c = new car();
            c.display();

        }
    }
}
```

## Output:

![c#8](https://github.com/Gayathriraj18/Inheritance/assets/94154854/222d6f0b-9495-4fdd-9f20-0f61adab4ef9)


## Result :

Thus C# program to print some messages using hierarchical inheritance is written and executed sucessfully.
